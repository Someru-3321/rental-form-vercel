# mi-mi+ レンタル空き確認フォーム (Vercel)

LINE LIFF 経由でアクセスするレンタル空き確認&仮予約フォーム。Vercelにホスティングして LIFF SDK を正常動作させ、User ID自動取得 → Apps Script API 経由で Notion 登録 + LINE Push 通知。

## アーキテクチャ

- **フロントエンド** (Vercel, 静的): `index.html` + LIFF SDK
- **API サーバー** (Google Apps Script): Notion 登録 + LINE Messaging API
- **DB**: Notion (出入管理表【mi-mi +】)

## 関連プロジェクト

- 旧 Apps Script Web App版: `../rental-availability-form/`
  - LIFF + Apps Script の iframe 競合で User ID 取得不可だったため移行

## デプロイ

GitHub push → Vercel 自動デプロイ
