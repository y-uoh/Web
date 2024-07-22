# HTMLタグメモ
## 共通（一般）
| タグ | 内　容 | MDNリファレンス | 備　考 |  
| --- | --- | --- | --- |
| `<b>`タグ | 太字 | [`<b>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/b) |  |  
| `<i>`タグ | イタリック文字 | [`<i>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/i) |  |  
| `<p>`タグ | 段落要素。テキストのひと固まりを表すときに使う | [`<p>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/p) |  |  
| `<h1>`タグ | 見出し要素 | [`<h1>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |  |  
| `<ol>`タグ | 順序付きリスト | [`<ou>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ol) |  |  
| `<ul>`タグ | 順序無しリスト | [`<ul>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ul) |  |  
| `<li>`タグ | リスト項目 | [`<li>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/li) |  |
| `<a>`タグ | アンカー要素：ハイパーリンクの作成 | [`<a>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/a) |  |  
| `<img>`タグ | 画像埋め込み要素：文書に画像を埋め込む | [`<img>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/img) | 空要素 |  
| `<hr>`タグ | 水平線要素 | [`<hr>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/hr) |  |  
| `<br>`タグ | 改行要素 | [`<br>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/br) |  |  
| `<sup>`タグ | 上付き文字要素。指数や添え字を表現 | [`<sup>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/sup) |  |  
| `<sub>`タグ | 下付き文字要素 | [`<sub>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/sub) |  |  
| `<>`タグ |  | [`<>`タグ詳細 -MDN]() |  |  
| `<>`タグ |  | [`<>`タグ詳細 -MDN]() |  |  
| `<>`タグ |  | [`<>`タグ詳細 -MDN]() |  |  
  
<br>  
  
## テーブル要素
| タグ | 内　容 | MDNリファレンス | 備　考 |  
| --- | --- | --- | --- |  
| `<table>`タグ | テーブル要素の宣言 | [`<table>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/table) |  |  
| `<tr>`タグ | 行要素。DBでいうレコード。この囲みで一行分を表現 | [`<tr>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/tr) |  |  
| `<td>`タグ | セル要素。DBでいうフィールド。表の個別のデータを表現 | [`<td>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/td) |  |  
| `<th>`タグ | 見出し要素。テーブルの項目部分（ヘッダー）を表現 | [`<th>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/th) |  |  
| `<thead>`タグ | テーブルヘッダー要素。テーブルのヘッダ部分を定義する | [`<thead>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/thead) |  |  
| `<tbody>`タグ | テーブル本体要素。テーブルの本体部分であることを定義する | [`<hbody>`タグ詳細 -MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/tbody) |  |  
| `<rowspan>`属性 | `th`や`td`の行数を属性値として指定できる | [`<>`タグ詳細 -MDN]() |  |  
| `<colspan>`属性 | `th`や`td`の列数を属性値として指定できる | [`<>`タグ詳細 -MDN]() |  |  
| `<>`タグ |  | [`<>`タグ詳細 -MDN]() |  |  
  
### Sample
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>人口順位</title>
</head>

<body>
    <h1>人口順位</h1>
    <table> <!--- table要素の宣言 ここから --->
        <thead>     <!--- ヘッダー要素を定義　ここから --->
            <tr>    <!--- 行要素を定義　ここから --->
                <th rowspan="2">順　位</th> <!--- 見出し要素。属性値rowspan="2"で設定されているので、2行分のセルを使っている --->
                <th colspan="2">地　域</th> <!--- 見出し要素。属性値colspan="2"で設定されているので、2列分のセルを使っている --->
                <th rowspan="2">法定人口（人）</th> <!--- 見出し要素。属性値rowspan="2"で設定されているので、2行分のセルを使っている --->
            </tr>   <!--- 行要素を定義　ここまでで一行 --->

            <tr>
                <th>都道府県</th>   <!--- 見出し要素。地域ヘッダーのサブヘッダーとなっている --->
                <th>市（区）</th>   <!--- 見出し要素。地域ヘッダーのサブヘッダーとなっている --->
            </tr>
        </thead>    <!--- ヘッダー要素を定義　ここまで --->

        <tbody> <!--- 本体要素を定義　ここから --->
            <tr>    <!--- 行要素を定義　ここから --->
                <td>0</td>  <!--- セル要素。レコードの一データ --->
                <td>東京都</td>  <!--- セル要素。レコードの一データ --->
                <td>特別区</td>  <!--- セル要素。レコードの一データ --->
                <td>9,733,276</td>  <!--- セル要素。レコードの一データ --->
            </tr>   <!--- 行要素を定義　ここまでで一行 --->

            <tr>    <!--- 行要素を定義　ここから --->
                <td>1</td>  <!--- セル要素。レコードの一データ --->
                <td>神奈川県</td>  <!--- セル要素。レコードの一データ --->
                <td>横浜市</td>  <!--- セル要素。レコードの一データ --->
                <td>3,777,491</td>  <!--- セル要素。レコードの一データ --->
            </tr>   <!--- 行要素を定義　ここまでで一行 --->

            <tr>    <!--- 行要素を定義　ここから --->
                <td>2</td>  <!--- セル要素。レコードの一データ --->
                <td>大阪府</td>  <!--- セル要素。レコードの一データ --->
                <td>大阪市</td>  <!--- セル要素。レコードの一データ --->
                <td>2,752,412</td>  <!--- セル要素。レコードの一データ --->
            </tr>   <!--- 行要素を定義　ここまでで一行 --->

        </tbody> <!--- 本体要素を定義　ここまで --->

    </table> <!--- table要素の宣言 ここまで --->
</body>

</html>
```  
  
[サンプルページ](C:\Users\udb19\OneDrive\デスクトップ\00_knowledge Book\10_web技術\Web\01_HTML\Talble_Sample.html)

