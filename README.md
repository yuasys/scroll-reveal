# scroll-reveal

【目的】ASWサービスのサンプルサイト仕様の実験／検証をすること

## スクロールアニメーション効果の導入

ユーザーにとって楽しいサイトを追求すると、デザインそのものの美しさはもちろんですが、さり気なく動きのあるサイトも気が利いていて嬉しくなる機能だと思います。  

ライブラリ「scrollrevealjs」を使ってスクロールアニメーションを実装すると、スクロール操作によって画像やテキストがふわっと動きます。実装は簡単です。

[この動画](https://youtu.be/Wt19KoskUAM)に触発されて最初のリポジトリを作成しました。基本はお手本通りですが初期のソースは[ここ](https://github.com/Shin-sibainu/Reveal-Scroll-Animation)にあります。  

1. スクロール効果ライブラリで有名な [ScrollRevealの公式サイト](https://scrollrevealjs.org/)です。
1. 実際の動きは[このリンク](https://yuasys.github.io/scroll-reveal/)（※右クリック➜「新しいタブで開く」の使用をおすすめします）から確認できます。
1. コンテンツの一部で、[Fontoawesome](https://fontawesome.com/)のお世話になっています。また、実際にFontAwesom実装作業をするときに参考になる[動画解説](https://youtu.be/Un9LujMC1qQ)も紹介します。
1. コンテンツ内のテキストボックスには曇りガラス効果（backdrop-filter)が用いられていますが、[モバイルでは無効](https://caniuse.com/css-backdrop-filter)な場合があるので、注意が必要です。  
例えば、iPhone標準のSfariの場合「backdrop-filter: blur(20px);」などとしても無効なので、直後の行に  
CSSのプロパティ名に接頭辞「-webkit-」を付けて、「-webkit-backdrop-filter: blur(20px);」などとした行を追加してあげるとOKになります。

### おまけ CSS基礎学習におすすめの動画再生リスト

[この動画学習（再生リスト）](https://youtube.com/playlist?list=PLil1beHgVxREji2evsQYLieygYIiZ5jfc)はとても簡潔丁寧な解説があり分かりやすいので、おすすめします。
