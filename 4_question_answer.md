# memo:修正点 11/2 11:04
- マークダウンの強調、赤文字を使って読みやすくする
- rake routes ではなく rails routes を使う（テキストではそちらに統一済み）

## 質問（ワークサンプルから転載）
Railsにおける、「単数」と「複数」の使い分けについての説明です。

例えばコントローラー作成時は"blogs"と、モデル作成時は"blog”とそれぞれパラメーター指定させています。それに基づいて様々な変数等が自動的に作成されているようなので、"blogs"と"blog"を使い分けることに意味があるのだと思うのですが、何処にも記載が無いので未だに混乱しています。

rake routes"を行ってみても、Prefixに"blog"　”new_blog"もあれば、"blogs" "confirm_blogs"もあります。何故こうなっているのか全く理解できていません。

---

## 回答
その場面で扱う対象、つまりリソース（今回の場合は"blog"）が"複数"か"単数"かによって使い分けます。

例えば、モデルはこれから作られていくBlogクラスのインスタンスの雛形であり、いわば設計図です。これは複数存在するものではなく、単一のものです。

対して、コントローラでは複数のblogクラスのインスタンスを扱うことが想定されているため、複数形の"blogs"を使うのだと考えることができます。

またPrefixにおける単数・複数の使い分けですが、これはRailsがWebAPIの設計思想の一つである"RESTful"を前提に作られていることが背景にあります。

RESTfulとは、簡単に言うと「操作したいリソースをURLで指定し、GET/POST/PUT/PATCH/DELETEなどのhttpメソッドとともにWebサーバに送信することで操作を実現する」仕組みです（詳しくはぜひ調べてみてください）。
この「操作したいリソース」が単一のものか複数かによって使い分けられているのです。

次の例をご覧ください。
```ruby
Rails.application.routes.draw do
  # ルーティングを定義
  resources :blogs
end
```

```
$ rake routes
   Prefix Verb   URI Pattern                 Controller#Action
    blogs GET    /blogs(.:format)            blogs#index
          POST   /blogs(.:format)            blogs#create
 new_blog GET    /blogs/new(.:format)        blogs#new
edit_blog GET    /blogs/:id/edit(.:format)   blogs#edit
     blog GET    /blogs/:id(.:format)        blogs#show
          PATCH  /blogs/:id(.:format)        blogs#update
          PUT    /blogs/:id(.:format)        blogs#update
          DELETE /blogs/:id(.:format)        blogs#destroy
```
この中でPrefixに複数形が使われているのはindex, createです。
これらは、リソースblogの集合を一覧したり（index）、集合に対し新たな要素を追加する（create）操作だといえます。故にリソース名は複数形となるのが自然とされています。

対して、その他のアクションは単数形が使われています。これは、URLにidを付与し単一のリソースを指定していることからわかるように、操作の対象が単一のものだからだと考えることができます。
new_blogはid指定されていませんが、これは呼ばれた時点ではまだリソースが存在しないためで、扱う対象としてはこれから作成される単一のリソースを想定しているため単数形となっています。

日本語には名詞に単数形と複数形の区別がないので少し馴染みにくいかもしれませんが、Railsは英語の慣習に基づいて作られています。慣れておくと今後の学習に役立つはずです。
