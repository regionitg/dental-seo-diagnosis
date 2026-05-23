# 🦷 歯科医院 AI診断ツール

Gemini 2.5 Flash を使った歯科医院向けSEO・MEO診断ツールです。
医院名とエリアを入力するだけで、検索順位・クチコミ・専門性の3軸で診断します。

---

## 機能

- **AI診断**：Gemini 2.5 Flash による SEO・MEO総合診断
- **スコア表示**：総合スコア＋3項目（検索順位・クチコミ・専門性）をドーナツグラフで表示
- **QRコード生成**：診断結果ページのURLをQR化して共有・印刷に活用
- **2部印刷**：A4用紙1枚に診断結果を2部出力（院長・スタッフ用など）
- **共有URL**：診断結果をURLパラメータで保持し、リンク共有に対応

---

## 使い方

### ローカルで使う（ファイルをダブルクリック）

1. `index.html` をブラウザで開く
2. API設定からGemini APIキーを入力
3. 医院名・エリアを入力して「AI診断を実行」

> **APIキーの取得**：[Google AI Studio](https://aistudio.google.com/apikey) で無料取得できます

### GitHub Pages でデプロイする（推奨）

QRコードに診断結果URLを埋め込む機能はデプロイ環境でのみ動作します。

```bash
# 1. リポジトリをクローン（またはこのフォルダをpush）
git clone https://github.com/YOUR_USERNAME/dental-seo-diagnosis.git
cd dental-seo-diagnosis

# 2. GitHubにpush
git add .
git commit -m "initial commit"
git push origin main
```

その後、GitHub → Settings → Pages → Source を `main` ブランチ `/root` に設定すると
`https://YOUR_USERNAME.github.io/dental-seo-diagnosis/` で公開されます。

---

## ファイル構成

```
dental-seo-diagnosis/
├── index.html   # メインアプリ（これ1ファイルで完結）
├── .gitignore
└── README.md
```

---

## セキュリティについて

- **APIキーはHTMLにハードコードしないでください**
- このツールはAPIキーをブラウザ内の入力フィールドで受け取り、Gemini APIに直接送信します
- GitHubにpushするコードにAPIキーが含まれていないことを必ず確認してください

---

## 開発・運用元

**株式会社レジオン**  
〒812-0016 福岡県福岡市博多区博多駅南5-6-26-101  
TEL: 092-433-4066  
https://region-co.com
