# Matcharcoal

炭入り抹茶のランディングページ（日英）。Cloudflare Pages で公開。

- 1枚の静的HTML（`index.html`）。ビルド不要
- メール登録フォームは Formspree のURLに差し替えて使用

## 販売を始めるとき
1. `tokushoho.html` の【要入力】をすべて埋める
2. Stripe で商品ごとに Payment Link を作る（数量の変更を許可、配送先住所の入力、送料、支払い後は `https://matcharcoal.pages.dev/thanks.html` に移動）
3. `index.html` の `SHOP` で `open:true` にし、`links` に Payment Link の URL を入れる
4. 価格を変えた場合は `SHOP.prices` も Stripe と同じ金額にする
