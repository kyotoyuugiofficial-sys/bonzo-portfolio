# bonzo portfolio / WORK_PROGRESS

更新：2026-11-20（日本時間）

## 現在の公開先
- https://bonzo-portfolio.pages.dev/
- GitHub: kyotoyuugiofficial-sys/bonzo-portfolio / main
- Cloudflare PagesはGitHub連携で更新。WorkによるCloudflareログイン・パスワード再設定は中止を継続。

## 今回の変更
- main最新版 0540d8e890c424497257484da9ef9d6e13a0ab8f を新規cloneして編集。過去のZIPは使用していない。
- 日本語・英語の抽象的な標語と説明文を直接的な情報へ変更。
- 通常の見出し、コンパクトな余白、単純な画像とリンクの構成へ変更。巨大文字、波形、画像上の重ね文字を撤去。
- ナビゲーションに関連リンクを追加。このサイトのGitHubソースへのリンクを追加。
- OP動画を開閉式にし、クリック後にYouTubeをロードする仕様を維持。
- 公開済みの本番URLをsiteUrlへ設定。
- 既存の作品公式サイト、人物配置、ゲーム本編には変更しない。

## 検証
- ローカルで日英4ページをビルド。静的チェック131項目が通過。
- PC見出し32px、横はみ出しなし。
- 390pxと768pxのiframe viewportで横はみ出しなし。
- モバイルメニューの開閉とリンク選択後の閉じ動作を確認。
- OPの開閉パネルとYouTube埋め込みの読込、英語音楽ページを確認。
- GitHubのCloudflare Pagesチェックでデプロイ成功を確認。公開HTMLの見出し変更を確認。
- 初回の公開確認で古いCSSキャッシュの混在を検出し、CSS/JSに内容ハッシュ付きURLを追加。
- 8b51d56c3d3ad564dedcb42d83057e1c952fd5a9 のCloudflare Pagesチェックがsuccess。公開画面でもハッシュ付きCSSの読込と32px見出し・16px本文を確認。
- 本番の日英トップ・音楽ページを確認。本番390px/768px幅で横はみ出しなし。モバイルメニューの開閉・リンク選択後の閉じ動作を確認。
- 実機iOS/Android/Safari、音付き動画の全編再生は未検証。

## 未確認・保留
- 今回の依頼本文は末尾「見」で途切れており、新規SNS URLなどの追加指定は含まれていない。新しいURLは推測していない。
- note本人URL、X本人URL、問い合わせ先の公開承認、正式な試聴音源は未確認。サイトは準備中表示を維持。
- note記事・X投稿・GitHubプロフィール原稿は以前に作成済み。未承認の記事公開や本人認証は行わない。

## 次回の手順
1. main最新版とこの記録を読む。古いZIPで上書きしない。
2. 公開ページの反映結果を確認する。
3. 所有者から追加リンクURLや承認済み問い合わせ先を受けたらcontent/settings.jsonへ設定。
4. npm run build && npm run check を通してGitHub連携で更新し、公開ページも検証する。
