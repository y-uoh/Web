# VScodeテクニック
`VScode`で`HTML`を記述するにあたってのテクニック一覧  
  
## HTMLスケルトンのひな型の補完
- `!`を置いて`Tab`補完を行うと、HTMLスケルトンが補完される  
  
## 文書の体裁を整えるFormat Document
- `Shift + Alt + f`で`Fortmat Document`が実行され、文書の体裁が自動で整う  
  
## lorem
- `HTML`文書中に`lorem`と入力し`Tab`補完を行うと**適当な仮のテキスト**を自動で挿入してくれる
- `lorem * 5`などと記述すると、5行分仮テキストを挿入するなどの記述の仕方もある  
  
## コメントアウト
- コメントアウトは`<!-- コメント -->`と記述する
- VScodeのショートカットは`Ctrl + /`で、コメントアウトの切り替えができる  
  
## Emmet
- HTMLを作成する際の便利ツール
- HTMLスケルトンを補完してくれる`!`もEmmetの機能のひとつ
- 例えば子要素一発で作る際に、`main>section>h1`と記述し`Tab`を押下すると下記のように自動的に子要素を補完してくれる
```html
<main>
    <section>
        <h1></h1>
    </section>
</main>
```  
- Emmet構文を数が多くあるので、便利に使うにはリファレンスを確認しながらやるとよい
[Emmetチートシート](https://docs.emmet.io/cheat-sheet/)  
