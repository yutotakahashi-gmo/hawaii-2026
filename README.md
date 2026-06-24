# Hawaii 2026 🌺 Travel App

Oahu / Waikiki への旅（2026/8/11 → 8/25・5名: Emi · Ikuo · Maki · Yuto · Reika）の旅程アプリ。
`index.html` 1ファイルで完結する静的サイト。ビルド不要・依存なし。スマホ最適化＋PWA対応。

## 内容
- 🗓 旅程（日ごとテーブル・Googleマップ直リンク）
- ✈️ 移動（往復フライト）
- 🏨 宿（前半 Vrbo / 後半 Park Shore Waikiki）
- 🍴 食事メモ
- 🛂 ESTA チェック（5名分・端末保存）
- 💳 費用メモ
- ✅ 持ち物チェックリスト（端末保存）
- 出発カウントダウン

## ローカルで開く
`index.html` をブラウザで開くだけ。

## デプロイ（GitHub Pages・git不要のWeb UI手順）
1. https://github.com/new でリポジトリ作成（例 `hawaii-2026`、**Public**、READMEは付けない）。
2. 空リポジトリには直接アップロードできないので、まず「creating a new file」で `.gitignore` を1つ作成・コミット → `main` ブランチが作られる。
3. `https://github.com/<ユーザー名>/hawaii-2026/upload/main` を開き、次のファイルをまとめてアップロード → コミット:
   - `index.html`
   - `site.webmanifest`
   - `apple-touch-icon.png` / `favicon-32.png` / `icon-192.png` / `icon-512.png`
   - `README.md`
4. **Settings → Pages** → Source `Deploy from a branch` → Branch `main` / `/(root)` → **Save**。
5. 数十秒後に `https://<ユーザー名>.github.io/hawaii-2026/` で公開。

> GitHubへのログインはご本人で。OneDrive同期フォルダ上では `git init` が不安定になることがあるため、Web UI手順が確実です。

## iPhoneホーム画面に追加
Safariで公開URLを開く → 共有 → 「ホーム画面に追加」。専用アイコンで全画面起動します。

## ⚠️ プライバシー
公開版にはパスポート番号・予約番号・航空券番号・ESTA申請番号・カード情報は**含めていません**。
機微情報も手元で見たい場合はリポジトリを **Private** にするか、非公開メモで管理してください。
