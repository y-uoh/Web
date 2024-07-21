# セマンティックHTMLとは
- 文の構造によってHTML要素に意味・役割をもたせること
- レイアウトや見た目を重視してタグを使うのではなく、**意味に注目してタグを利用しよう**という考え方がセマンティックHTMLの考え方
- セマンティックとは、意味を持たせるという意味

## メリット
### サイトの検索順位が上がる
セマンティックタグを正しく使用することで、サイトを巡回しているクローラーがサイトを構造的に理解し、結果サイトの検索順位が上がることにつながる
  
### 保守性が向上する（コードの可動性が上がる）
セマンティックタグを使用することでコードが読みやすくなるので、HTML全体の構造がわかりやすくなる
  
## セマンティックタグのとは
- セマンティックタグは100種類以上あるが、よく使用するタグは以下の通り
```html
- <main>
- <article>
- <aside>
- <section>
- <header>
- <footer>
- <nav>
- <figure>
- <figcaption>
```  
  
- 上記のタグを組み合わせた作成したHTMLのファーマットの一例
```html
<body>

  <header>
    <nav>
      <!-- header部分 -->
    </nav>
  </header>
  
  <main> 
    <article>
      <section>
	    <figure>
  　        <img src="sauna.png" alt="サウナの画像">
  　　　    <figcaption>サウナの画像</figcaption>
         </figure>
      </section>

      <section>
        <!-- コンテンツ部分 -->
      </section>

      <section>
        <!-- コンテンツ部分 -->
      </section>

    </article>
  </main>

  <aside>
    <!-- サイドバー部分 -->
  </aside>

  <footer>
    <!-- footer部分 -->
  </footer>

</body>
```  
  
## 参考サイト
- [【HTML】セマンティックとは？ -Zenn ](https://zenn.dev/simizunomoto/articles/792b0988039496) 
- [セマンティックHTMLとは？初心者向け3分で分かりやすく解説 -Biz.Online ](https://it-biz.online/web-design/semantic-html/)  
  