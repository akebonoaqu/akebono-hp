# デプロイ手順（再アップロード）

## 現在の公開URL
https://akebono-hp.izxzw300.workers.dev

## HPを更新したら、この手順で反映します

### 1. Cloudflareダッシュボードへ
https://dash.cloudflare.com/ にログイン
→ Workers & Pages → **akebono-hp** をクリック

### 2. 新しいデプロイを作成
右上の **「New deployment」**（雲アイコン）をクリック

### 3. ファイルをアップロード
「Upload assets」エリアに、`index.html` をドラッグ&ドロップ
（フォルダごとドロップでもOK）

### 4. Deployボタンをクリック
数十秒で反映されます

---

## Claude Codeでの編集フロー

1. Claude Codeに「〇〇を変更して」と依頼
2. 私（Claude）が `index.html` を編集 → GitHubにpush
3. 上記の手順でCloudflareに再アップロード

※ GitHub ↔ Cloudflare の自動連携ができると一番便利ですが、
   現状は手動アップロード方式です。

---

## ローカルで確認する方法

```bash
open ~/Documents/あけぼの鍼灸マッサージ院HP/index.html
```
