# Safari 業務指示書ポータル — はじめての方へ

> Safari買取店 業務指示書のWebポータル  
> シンプルな静的HTMLサイト

---

## セットアップ確認（1分）

Cursorで開いたら、チャットに入力：

```
このサイトの概要を教えて
```

---

## 新しいPCでのセットアップ

```bash
# GitHubにログイン（オーナーのみ・初回）
gh auth login

# リポジトリを取得
git clone https://github.com/komatsu-matsuko/safari-manuals.git
cursor safari-manuals/
```

---

## ローカルで確認する方法

サーバー不要。ファイルをブラウザで直接開くだけ：

```bash
open index.html
```

---

## 編集・更新の依頼方法

Cursorのチャットで直接依頼：

```
「業務手順のセクションを追加して」
「デザインをもっとわかりやすくして」
「新しいページを作って」
```

---

## 公開（デプロイ）

```bash
git add .
git commit -m "update: [変更内容]"
git push origin main
```

**mainへの直接pushはオーナーのみ。**

---

## ファイル構成

```
safari-manuals/
├── SETUP.md     ← このファイル
├── README.md    ← プロジェクト説明
├── index.html   ← 業務指示書ポータル（メインページ）
└── .cursor/rules/  ← AIの知識定義
```
