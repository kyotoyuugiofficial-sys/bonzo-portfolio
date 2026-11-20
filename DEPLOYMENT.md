# Cloudflare Pages / GitHub連携の設定

通常のChromeで、Cloudflareの Workers & Pages から「Pages」のGitインポートを選択してください。Workersのデプロイ設定ではありません。

| 項目 | 値 |
|---|---|
| GitHub所有者 | kyotoyuugiofficial-sys |
| リポジトリ | bonzo-portfolio |
| 本番ブランチ | main |
| Framework preset | None |
| Root directory | 空欄（リポジトリ直下） |
| Build command | npm run build && npm run check |
| Build output directory | dist |
| 環境変数 | NODE_VERSION = 22 |

GitHub連携でリポジトリを選ぶ際は bonzo-portfolio を追加してください。既存の作品公式プロジェクトやそのGitHub連携は変更しないでください。

初回ビルドではCloudflareが設定する CF_PAGES_URL を読み取り、OGP等の絶対URLを生成します。公開後の安定した本番URLが確認できたら、WorkへそのURLを知らせてください。Work側で SITE_URL を確定してGitHubへ保存します。仮のドメインを予想して設定する必要はありません。main以外のブランチのビルドはnoindexになります。

未承認の問い合わせ先と未確認のnoteリンクは掲載しません。それらが未設定でもビルドできます。今後、確認した値をWorkがcontent/settings.jsonへ設定します。音源は公開許諾とファイルの確認後に登録します。

公開後は日本語 /、英語 /en/、音楽 /music/ と /en/music/、画像、YouTube、モバイルメニュー、404、OGP、sitemapを確認します。本番の動作確認はまだ行っていません。

技術資料：https://developers.cloudflare.com/pages/configuration/build-configuration/
