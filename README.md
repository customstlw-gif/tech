# Tech Command Reference（運用コマンド集）

Snowflake・PostgreSQL・Red Hat Enterprise Linux・HULFT・CLUSTERPRO・JP1/AJS3・GitLab などの運用コマンドを、技術ごと・ケースごとに整理したリファレンスサイトです。GitHub Pages で公開しています。

## 構成

```
.
├── index.html          トップページ（技術一覧）
├── snowflake/
│   └── index.html      Snowflake 運用コマンド
├── aurora-postgresql/
│   └── index.html      Aurora PostgreSQL 運用コマンド
├── rhel/
│   └── index.html      Red Hat Enterprise Linux 9.8 運用コマンド
├── hulft/
│   └── index.html      HULFT10 for Linux 運用コマンド
├── clusterpro/
│   └── index.html      CLUSTERPRO X 6.0 for Linux 運用コマンド
├── jp1-ajs3/
│   └── index.html      JP1/AJS3 Version 13 運用コマンド
├── gitlab/
│   └── index.html      GitLab(Linuxパッケージ版)運用コマンド
├── .nojekyll           Jekyll 変換を無効化（ファイルをそのまま公開）
└── README.md
```

## 新しい技術を追加する手順

1. 既存ページ（例: `snowflake/index.html`）をコピーし、`<技術名>/index.html` として作成する
   - フォルダ名は英小文字とハイフンのみ（例: `postgresql`, `rhel`）。URL になるため公開後は変更しない
2. タイトル・目次・各章のコマンドを書き換える（章立ては下記の共通構成に合わせる）
3. トップの `index.html` で該当カードを「公開中」に変更し、`<a class="card" href="<技術名>/">` にする
4. Commit して main に反映する（1〜2 分で公開される）

## 共通の章立て

| No | ケース |
|----|--------|
| 01 | 構築 |
| 02 | 構成情報の取得 |
| 03 | 性能情報の取得 |
| 04 | 障害時の調査 |
| 05 | 権限・セキュリティ監査 |
| 06 | コスト・容量管理 |
| 07 | バックアップ・復旧 |

## 公開前チェック

- 実在のホスト名・IP アドレス・アカウント名・パスワード・社名が含まれていないか
- 仮の名前の付け方（`SAMPLE_`、`<...>`）が技術間で揃っているか
- 対象バージョンと最終更新日を記載しているか
- トップページからリンクされているか
