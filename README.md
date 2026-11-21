# bodyquest

自分用の筋力増強アプリ。**娘の questboard とは別のリポジトリ**（混同しないため）。

- 公開先：`https://kohshi529-glitch.github.io/bodyquest/`
- 本体：`index.html` の1枚だけ。外部ライブラリなし、オフラインでも動く
- 記録は**この端末のこのブラウザの localStorage** にだけ残る。
  サーバにも Firebase にも送らない。**ホーム画面のアイコンからだけ開くこと**
  （別のブラウザで開くと別の保存領域になり、記録が見えない）
- バックアップ：設定タブ →「書き出す」で出た文字列をメモに保存。復元は同じ枠に貼って「読み込む」

## 中身

| タブ | |
|---|---|
| 今日 | 5種目のレベル制クエスト。全セットで上限に届くと次回レベルが1つ上がる |
| 計測 | 周径（上腕・大腿・胸囲・腹囲）／TANITA／InBody |
| 予測 | プログラムから立てた予測と実測の差。系列の傾きの判定 |
| 記録 | カレンダー、スコアの推移、12週の目標 |
| 設定 | セット数、レベルの手動調整、予測モデルの前提、バックアップ |

## 設置のしかた

1. GitHub で新しいリポジトリ `bodyquest` を作る（Public）
2. `index.html` と `README.md` をアップロード
3. Settings → Pages → Source を「Deploy from a branch」、ブランチ `main` / `(root)` にして Save
4. 数分後に `https://kohshi529-glitch.github.io/bodyquest/` が開く
5. iPhone の Safari で開き、共有 →「ホーム画面に追加」

## 更新のしかた

`index.html` を同じ名前で上げ直すだけ。**localStorage の記録は消えません**（同じオリジンのため）。
