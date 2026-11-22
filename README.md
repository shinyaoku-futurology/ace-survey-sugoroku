# エースを狙え！🎾 緊急アンケートすごろく

LINEグループ「エースを狙え！🎾」向けの、スマホ向け簡易アンケートすごろく。

公開予定URL（仮）: https://shinyaoku-futurology.github.io/ace-survey-sugoroku/

## 中身

- `index.html` … 本体（オフライン可。画像は `assets/` 相対パス）
- `assets/` … メリン画像
- `og.jpg` … OGP（1200×630）

## 遊び方（仕様）

ふりだし → 5マス（選択でやる気ポイント増減） → あがり

5マス：ヒゲ／今朝の気分／体調／化粧のノリは？／エースを狙うか？

- 各マス最高20点 × 5マス ＝ **100点満点**（途中もゴールも点数を大きく表示）
- **60点以上** → 今日は参加する！（60〜79点は赤い〇）
- **80点以上** → 今日は参加する！＋ **赤いぐるぐる花丸**（SVGで描画・アニメ）
- **60点未満** → 今日は参加しない（また今度）
- 回答はどこにも送信・保存しない（遊ぶだけ）

## GitHub Pages 公開手順

1. 新規リポジトリ例: `ace-survey-sugoroku`（public）
2. このフォルダの中身（`index.html` / `assets/` / `og.jpg`）をリポジトリ直下に置く
3. Settings → Pages → Deploy from branch → `main` / `/ (root)`
4. 反映後: `https://<user>.github.io/ace-survey-sugoroku/`
5. `index.html` の `og:url` / `og:image` / `twitter:image` を実際のURLに合わせる（必要なら）
6. Facebook 等でシェアする場合はシェアデバッガーで OGP を再取得

## 短縮URL

公開URLが決まったら is.gd などで短縮してグループに共有。

例（公開後に実行）:

```bash
curl -s "https://is.gd/create.php?format=simple&url=https%3A%2F%2Fshinyaoku-futurology.github.io%2Face-survey-sugoroku%2F"
```

## 注意

- グループへの投稿・送信はこのアプリ自体では行わない
- 仲間の顔写真は使っていない（メリン画像のみ）
- フォントは Noto Sans JP（Google Fonts）。中国語CJKフォントは使わない
