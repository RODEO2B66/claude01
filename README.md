# ⚡ VOID RUNNER

シンプルな2D回避ゲームです。迫りくる敵をかわして、どこまで生き残れるか？

![Game Screenshot](https://img.shields.io/badge/HTML%2FCSS%2FJS-only-00ffcc?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-ready-brightgreen?style=flat-square)

---

## 🎮 遊び方

| キー | 操作 |
|------|------|
| `W`  | 上に移動 |
| `A`  | 左に移動 |
| `S`  | 下に移動 |
| `D`  | 右に移動 |

- 赤い敵に当たると **ゲームオーバー**
- 生き残った時間がそのまま **スコア** になります
- スコアが上がるにつれて敵が速くなります

---

## 🚀 プレイ方法

### ローカルで起動
`index.html` をブラウザで開くだけ。サーバー不要！

```bash
open index.html   # Mac
start index.html  # Windows
```

### GitHub Pages で公開する手順

1. このリポジトリを GitHub にプッシュ済みであることを確認
2. リポジトリの **Settings** タブを開く
3. 左メニューから **Pages** を選択
4. **Branch** を `main` / `/ (root)` に設定して **Save**
5. 数秒後、以下の URL でアクセスできます：

```
https://<あなたのユーザー名>.github.io/<リポジトリ名>/
```

例: `https://RODEO2B66.github.io/claude01/`

---

## 📁 ファイル構成

```
claude01/
└── index.html   # ゲーム本体（これだけで動きます）
└── README.md    # このファイル
```

---

## 🛠️ 技術仕様

- **言語**: HTML / CSS / JavaScript（外部ライブラリなし）
- **描画**: Canvas 2D API
- **対応ブラウザ**: Chrome / Firefox / Safari / Edge（最新版）
- **ゲームループ**: `requestAnimationFrame` 使用

---

## 📝 コードについて

`index.html` のJavaScript部分はセクションごとにコメントで説明しています。初心者の方でも読めるよう、処理の流れを逐一記載しています。

主な構造：
- **定数・変数** — ゲームの設定値
- **キーボードイベント** — WASD入力の受け取り
- **startGame()** — ゲーム初期化
- **spawnEnemy()** — 敵の生成ロジック
- **updatePlayer() / updateEnemies()** — 毎フレームの移動処理
- **checkCollision()** — 当たり判定（AABB）
- **draw()** — Canvas への描画
- **gameLoop()** — メインループ（requestAnimationFrame）

---

## ライセンス

MIT License — 自由に使用・改変してください。
