##HTML 基本まとめ

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
