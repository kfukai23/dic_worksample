進捗状況

- [x] 1_create_heading.mdに見出しを記述した
- [ ] 2_fleshed_out_headline.mdに見出しに肉付けを行った文章を記述した
- [x] 3_improve_sentences.mdに修正文を記述して、プルリクエストを送信した
- [x] 4_question_answer.mdに回答を記述した

※ 以下 https://github.com/DiveintoCode-corp/worksample/blob/master/educational_mentor_web.md から転載

---

# ワークサンプル for 教育メンター（Webエンジニアコース）

## 概要

教育メンター（Webエンジニアコース）のワークサンプルでは、業務内容と同じ以下の内容を体験していただきます。  

1. テキスト開発
2. テキスト修正
3. オンライン質問回答

重要なことは、本当に自分がメンバーになったかのように体験することです。これは、ただの筆記テストではありません。  
あなたと私たちの双方にとって、とても大切なことです。  

### 必要な前提知識

DIVE INTO CODEは未経験であっても必要な知識をキャッチアップできる人、それをずっと続けることができる人を採用しています。  
現時点の知識があれば理想的ですが、完全にゼロでもチャレンジする機会を設けています。  
知識がゼロの方は、この機会にご自分がどこまで知識をつけられそうかを確かめましょう。  

- Git
- Github
- (GithubFlow)
- Markdown
- Linuxコマンド基礎
- エディタの操作
- アルゴリズムの基礎
- DBMS・SQLの基礎知識
- Web技術の基礎（URL/HTTP/リクエスト/サーバーなど）
- HTML/CSSの基礎
- Rubyの知識
- Railsの基礎

現時点で知識が身についていない方を対象に、推薦学習教材をお伝えします。

[推薦学習教材](https://github.com/DiveintoCode-corp/worksample/blob/master/learning_material_web_application.md)

## 取り組み方の基本原則

ワークサンプルへの取り組む方の基本原則をお伝えします。  

- 優しく丁寧に対応すること
- ただ答えを教えるのではなく、その人のためになるようにサポートすること
- オンラインでのコミュニケーションは語弊が生じやすいので、表現などに気をつけること
- 事前に説明していない言葉やユーザーのレベルを考えて、サポートや教材開発を行うこと

## 取り組みへの質問について

ご質問がある場合は、ワークサンプル担当者にお気軽にご質問ください。  
ワークサンプルに取り組むためであれば、DIVE INTO CODEの自習室や教室の利用が可能です。積極的にご利用ください。  

## ワークサンプル1 テキスト開発

それでは最初のワークサンプルである、テキスト開発に入っていきます。  
あなたは、テキスト開発のミッションを行うことになり、カリキュラム内のある部分の執筆を行うことになりました。  
テキスト開発を行う際には、事前にどのようなテキストを開発するのか、どのようなことを学んだ状態で開発するテキストを学習するのか、そして何を目的にそのテキストを学んでいただくのかを知る必要があります。  

あなたは、Rails入門のテキスト作成を担当することになりました。  
HTML/CSS/JSの基礎とRuby,RubyアルゴリズムとGit/Githubを学んだ初心者を対象に、Railsを学ぶ前の`事前`テキストを作成をします。  
この事前テキストが終わった後に受講生は、Railsを本格的に学んでいくことになります。  
ここで重要なことは、Railsをきちんと理解するために必要な事前知識を調べて、見出しレベルで良いので落とし込むことです。  
初心者の人でも分かるようなテキストにすることを心がけて作成してください。  

### 見出しを作成しよう

さてどのようなテキストを作成するか、どのようなテキストを作成するか、テキストのゴールについて知ることができました。  
それでは、実際に見出しを作成しましょう。  
見出しは、Markdown形式で作成し、見出し3まで完成させてください。テキスト一つあたりの学習時間の目安は、15分で終わることです。  
また、必ず著作権について気をつけるようにしてください。  

`見出し例　(Linuxコマンド基礎の場合)`


```
# Linuxコマンド基礎

## このテキストのゴール

## Linuxとは

## Linuxコマンドとは

## なぜLinuxコマンドを覚える必要があるか

## 実際にLinuxコマンドを使ってみよう！
### ls
### mkdir
### cd

....etc
```

### 作成した見出しをGithubに提出する

見出しを作成することができたら、`worksample`というGithubリポジトリを作成し、作成した見出しを`1_create_heading.md`というファイル名で作成し、`Github`上で見れるようにしましょう。  

### 見出しを肉付けしよう

見出しを作成することができたら、その次は DIVE INTO CODE のワークサンプル担当者からのレビューがあり、そして見出しに肉付けを行います。  
また、詳しく説明するために、さらに見出しを付け加えても構いません。  

`見出しの例`

```
### リスト
```

`肉付け後の例`

```
### リスト
Pythonにはリストという概念があります。
リストを使用することで複数の要素を扱うことができるようになります。

※要素
リストは複数の値を格納することができますが、その格納するそれぞれの値のことを要素と言います。

実際にリストを使用して、その概念について学びましょう。

リストを定義するためには`[ ]`(角括弧)を使用します。
`sample_list`という変数に、何も要素が入っていない空のリストを代入します。

>>> sample_list = [ ]
>>> sample_list
[]


※Python対話型インタプリタが起動していない場合、ターミナルで`python`と入力し実行しましょう。

リストには、複数の要素を定義することができます。
複数の要素を定義する場合、それぞれの要素をカンマで区切ります。

>>> sample_list = ['晴れ', '雨', '曇り']
>>> sample_list
['晴れ', '雨', '曇り']
```


### 作成した内容をGithubにPushする

作成した内容は、`worksample`リポジトリに、`2_fleshed_out_headline.md`を作成し、送信しましょう。  


## ワークサンプル2 テキスト修正

テキスト開発、お疲れ様でした。続いては、既存のテキストの修正です。  
もっとも重要な仕事として、日々受講生やメンターから報告されるテキストの改善点を実装していく、`テキスト修正`があります。  
テキスト修正するべき点については、実際は以下の図のようにGitHubのIssueで管理されています。  

[![https://diveintocode.gyazo.com/adfb7547a8fe9ee5a4b171d4e6829eb6](https://t.gyazo.com/teams/diveintocode/adfb7547a8fe9ee5a4b171d4e6829eb6.png)](https://diveintocode.gyazo.com/adfb7547a8fe9ee5a4b171d4e6829eb6)

テキスト修正のミッションを、このIssueを元に改善を行うことになります。  
今回のワークサンプルでは、実際のテキスト修正と同じように取り組んでいただきます。  

### ファイルを作成する

**今回使用する`3_improve_sentences.md`を作成し、事前にGithubにPushしておきましょう。**

### 修正するものについて
以下のIssueを担当しましょう。  

【担当するIssue】  
「selfについて」説明文が難しかったです。  

`該当文`

```
selfはインスタンスオブジェクト自身を指しています。クラスの中でインスタンスオブジェクトを呼び出す際やそのインスタンスオブジェクトを呼び出す際は、selfを使用します。
```

### 修正例

【担当するIssue】  
「バッククォート」なのですが、キーボードのどれか、一瞬分からなかったです。素人的ですが、ひょっとすると、迷う方がいるかもしれないです。  

`該当文`

```
コードを挿入する際は、
\`(バッククォート)を使用して、以下のように記述すると、ハイライトが適用されます。
```

`修正後`

```
コードを挿入する際は、
\`(バッククォート)を使用して、以下のように記述すると、ハイライトが適用されます。

バッククォートは、Shiftキーと＠キーを同時押しすると入力できます。
```

### 方法

**これまでの方法と異なるので注意してください**  

事前にGitHubに送信した、`3_improve_sentences.md`にプルリクエストを送る形で修正文を送信してください。  
なお、提出前に下記の内容を守ることができているかどうかご自分でチェックしてください。  

- [ ] 冒頭で全体像を明示する（できれば図解など）
- [ ] 各節に図解や数式など文章を補完するコンテンツを必ず含める
- [ ] 各節内の文章は出来るだけ読みやすいように改行を使うなどして工夫する
- [ ] コードを記述する場合はマークダウンの記号「`」を活用する

## ワークサンプル 3 オンライン質問回答

最後は、オンライン質問回答のワークサンプルです。  
実務では、オンライン学習サービス「DIVER」上での質問回答を行うことがよくあります。  
大切な業務のひとつです。  

### オンライン質問回答例

`質問例`

```
f.text_fieldとf.hidden_fieldの違いについて、念のための確認です。
以下の認識であってますでしょうか？

f.text_field　→　テキストを編集可能な状態で表示させる
f.hidden_field　→　テキストを編集不可の状態で表示させる
```

`回答例`

```
ほぼ合っていますが、多少補足します！

f.text_field　→　テキストを編集可能な状態で表示させる（テキストを打ち込むためのボックス部分を表示させる。そのボックスに最初からテキストが入っているかどうかは、form_for文に渡した引数によって異なる）

f.hidden_field　→　コントローラなどの命令で運んできたテキストなどのデータを、現在のページに含める。(見えないし編集もできない）
```

### 実際に回答してみよう

`質問`

```
Railsにおける、「単数」と「複数」の使い分けについての説明です。

例えばコントローラー作成時は"blogs"と、モデル作成時は"blog”とそれぞれパラメーター指定させています。それに基づいて様々な変数等が自動的に作成されているようなので、"blogs"と"blog"を使い分けることに意味があるのだと思うのですが、何処にも記載が無いので未だに混乱しています。

rake routes"を行ってみても、Prefixに"blog"　”new_blog"もあれば、"blogs" "confirm_blogs"もあります。何故こうなっているのか全く理解できていません。
```

### Push方法

`4_question_answer.md`に回答を記述して、GithubにPushしてください。  
なお、提出前に下記の内容を守ることができているかどうかご自分でチェックしてください。  

- [ ] マークダウンの引用記号「>」を使い引用する

## 提出方法

上記の内容に取り組んだものを反映した、あなたのGithubリポジトリのURLをご提出ください。  
なお、ご提出前に以下の項目をすべて満たしているかを確認しましょう。  

**`3_improve_sentences.md`のみプルリクエストを作成するということを忘れないでください**  

- [ ] `1_create_heading.md`に見出しを記述した
- [ ] `2_fleshed_out_headline.md`に見出しに肉付けを行った文章を記述した
- [ ] `3_improve_sentences.md`に修正文を記述して、プルリクエストを送信した
- [ ] `4_question_answer.md`に回答を記述した

### 提出期限

提出期限は、採用面接時にお話ができていればその期限までに。そうではない場合は、ご自分で決めてください。  
DIVE INTO CODEは、言われたからやるのではなく、自ら業務にコミットして達成していく姿勢を重視しています。  

以上でワークサンプルは終了です。  
お疲れ様でした。
