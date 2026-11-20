# WORK_PROGRESS — bonzo portfolio

更新：2026-11-20（日本時間）

## 完了
- 日本語・英語トップと音楽ページ、レスポンシブ表示、クリック同意後のYouTube読込、SEO・OGP、404を実装。
- 独立した新規リポジトリ kyotoyuugiofficial-sys/bonzo-portfolio を作成。Webソースのみをmainへ保存する構成。
- Git連携向けの設定をDEPLOYMENT.mdに記録。外部依存パッケージなし。
- 問い合わせ先とnoteが未確定でもビルド可能。未承認の連絡先や架空URLは出力しない。
- Cloudflareの実デプロイURLを自動読込。プレビューbranchはnoindex。
- X用アイコン・ヘッダー、プロフィール、固定ポスト・初期投稿5件、noteプロフィール・記事3本、GitHubプロフィールREADME、パブリッシャー向け日英プロフィールを別途作成済み。未承認原稿はこの公開リポジトリに含めない。

## 方針・保護対象
- CloudflareのWorkブラウザによるログイン、ログイン再試行、パスワード再設定は中止。通常のChromeで所有者がGitHubとPagesを連携する。
- 既存のキョウトユウギ公式サイト・リポジトリには、この段階で変更を加えない。
- ゲーム本編コード、未公開シナリオ、秘密情報、購入した音源は含めない。

## 未完了
- 所有者によるCloudflare PagesのGit連携・初回公開。設定はDEPLOYMENT.mdを参照。
- 問い合わせ先の公開承認、note本人URLの確定。
- X・note新規アカウントの登録承認と本人認証。投稿・記事の公開承認。
- GitHubプロフィール原稿の確認と反映。
- 正式音源のファイル・権利・公開範囲の確認。

## 検証
- 元サイトのPC、390px・768px幅、メニュー、日英切替、音楽ページ、YouTube読込をブラウザで確認済み。
- 静的チェック126項目通過。今回のGit連携用変更について、ローカル・Pages本番・Pagesプレビューを模した3通りのビルドで各126項目が通過。robotsの索引制御とOGP絶対URLも確認済み。
- 本番URL、Cloudflare内の実ビルド、実機iOS/Android/Safari、音付き動画全編・音源試聴は未検証。

## ファイル
- build.mjs / check.mjs / package.json：ビルドと検証
- content/settings.json：確認済みリンク、連絡先、音源登録
- static/：Webデザインと公開済みの作品紹介画像
- DEPLOYMENT.md：通常のChromeから行うPages設定
- WORK_PROGRESS.md：この再開記録

## 次回Workの手順
1. このリポジトリのmainと本ファイルを読む。以前の保存先や古いZIPで上書きしない。
2. Pagesの公開URLが提供されていれば、その実URLを検証してSITE_URLを確定する。
3. npm run build && npm run check を実行し、公開された日英4ページと画像・動画・OGPを検証する。
4. 承認済みの連絡先と確認済みnote URLを設定し、GitHub更新で自動デプロイを確認する。
5. X/note/GitHubプロフィールの未公開原稿を所有者と確認し、認証と承認のある範囲で設定を続ける。

本番URL：未発行。Cloudflare接続は所有者の操作待ち。GitHub保存とWeb公開は区別する。
