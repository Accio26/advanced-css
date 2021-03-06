## HTML 基本まとめ

基本構造
```html
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

1. DOCTYPE htmlとは
> ドキュメント宣言とは、その文書のバージョンを宣言するメタ情報です。上記のようにHTML5であれば、`<!DOCTYPE html>`と記述します。その他のバージョンでは違う書き方をしますが、基本はHTML5を使用しますのでその他の書き方を覚える必要はありません。
2. HTML要素とは
> html要素は、この文書がHTMLの文書であることを表します。ちなみに、「lang=”ja”」の”ja”は日本語で書かれた文書であることを表します。
3. head要素とは
> head要素にはその文書のメタデータを記述します。例えば、`<title></title>`でその文書のタイトルを、`<description></description>`でその文書の要約を定義することができます。
4. body要素とは
> body要素は、その文書の本文を表す。このbody要素で囲まれた領域がWebページとして表示される。
> body要素内にhtml文書を記述していく。

## 頻出タグ
`<html></html>`:HTMLを示す  
`<head></head>`: ヘッダ部分を示す  
`<title></title>`: ヘッダ内に記述する、タイトルを示す  
`<body></body>`: ボディ（本体）部分を示す、ブラウザに表示するタグはここに記述する  

`<h1></h1>~<h6></h6>`: 見出しのタグ、1が最も大きく、6が最も小さい文字サイズで表示される  
`<p></p>`:一つの段落であることを表す、文字に限らず画像などもこの中に表示できる  
`<a></a>`:ハイパーリンクを指定する `<a href="url"></a>`なども指定できる  
`<br>`:改行する  
`<div></div>`:ひとかたまりの範囲として定義する  
`<figcaption></figcaption>`:図表のキャプションを示す  
`<figure></figure>`:図表であることを示す  
`<footer></footer>`フッタであることを示す  
`<form></form>`:入力・送信フォームを作る  
`<img>`: 画像を表示する  
`<input>`:フォームを構成する様々な入力部品を作成する（種類が多い）  
`<li></li>`:リストの項目を記述する  
`<nav></nav>`:ナビゲーションであることを示す  
`<script></script>`:文書にJavaScriptなどのスクリプトを組み込む  
`<span></span>`:一つの範囲として定義する  
`<ul></ul>`:順序のないリストを表示する  

## そもそもHTML5とは？
> HTML5とは、HTMLのバージョン5、改訂第5版です。 ウェブページを作成する際、以前にはHTML 4.01やXHTML1が標準的に利用されていましたが、 現在は次世代のウェブ環境に合わせて仕様策定されたHTML5が標準となっています。HTML 4やXHTML1の目的は、HTMLタグで構造付けされたHTML文書を作成することでした。 これらのバージョンのHTMLでは、作成された情報をただ公開している分には良いのですが、 ユーザーの操作に反応してなんらかの情報処理をする、いわゆるウェブアプリケーションを作成するには機能不足な面がありました。HTML5では、これまでのHTML 4と同じようなHTML文書を作成する機能が改良されているのに加えて、ウェブアプリケーションを開発するための様々な仕様が新たに盛り込まれています。 今までプラグインなどのHTML以外の技術を併用しないと実現できなかった機能のいくつかが、標準のHTMLやJavaScriptで比較的シンプルに実現できるようになっています。


HTML5のhead部分とは？

> HTMLのhead部分は、ページが読み込まれてもWebブラウザーには表示されない部分のことです。
> この部分には`<title>`といった情報やCSSへのリンク、独自のファビコンへのリンク、そしてそのほかのメタデータ（HTMLを誰が書いたのとかそのHTMLを表現する重要なキーワードなど）の情報を含んでいます。

メタデータ：`<meta>`要素
> メタデータはデータを説明するデータで、HTMLには文書にメタデータを追加する「公式」な方法があります。
> `<meta>`要素です。

#### 作成者と説明を追加する
多くの`<meta>`要素は`name`と`content`属性が含まれます。
・`name`はmeta要素の種類を指定します。含まれる情報の種類です。
・`content`は実際のメタコンテンツを指定します。

ページに入れるのが便利な2つのメタ要素は、ページの著書を定義するものと、ページの説明(description)を与えるものです。例を見てみます。
```html
<meta name="author" content="Chris Mills">
<meta name="description" content="The MDN Web Docs Learning Area aims to provide complete beginners to the Web with all they need to know to ge started with developing web sites and applications.">
```
