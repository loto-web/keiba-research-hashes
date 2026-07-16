# TRACKV-EXTRACT-FULL-002 registration evidence

本ファイルは signal_full_v2 全量抽出（consumed / virgin / lockbox の3ファイル）と
`FULL_EXTRACT_MANIFEST_v2.md` の SHA256 を `HASHES.md` へ登録した際のサーバ側
（GitHub）証跡を記録する。本ファイル自体もこのリポジトリの一部としてadd/commit/pushされる。

## 登録コミット

- commit hash (full, HEAD at registration): `bade2ea70b8d78b14f9e62a05be4ee94632ded6b`
- commit message: `Seal signal_full_v2 extract (population-def-001, 3-way scheme-A split)`
- commit author/committer date (GitHub API, UTC): `2026-07-16T13:42:43Z`
- files changed: `HASHES.md`（追記4行）
- html_url (commit): https://github.com/loto-web/keiba-research-hashes/commit/bade2ea70b8d78b14f9e62a05be4ee94632ded6b
- push range: `54d341a..bade2ea`（本コミット1件のみが本push操作でorigin/mainへ反映）

## GitHubリポジトリAPI応答（`GET /repos/loto-web/keiba-research-hashes`）

- `pushed_at`: `2026-07-16T13:42:53Z`
- `html_url` (repo): https://github.com/loto-web/keiba-research-hashes
- `default_branch`: `main`
- `created_at` (repo): `2026-07-13T09:27:57Z`

`pushed_at`（13:42:53Z）はコミットのauthor/committer date（13:42:43Z）の10秒後であり、
登録push操作と時間的に整合する。

## sha256（本文書が証明対象とするファイル、HASHES.md記載と同一値）

- `sha256(vnext/extract_full/signal_full_v2_consumed.parquet)` = `745c6d643176eba09219d4e3450d8caf3ce9d0524450a5e29d63ad43a6c67e82`
- `sha256(vnext/extract_full/signal_full_v2_virgin.parquet)` = `11d288ec8d93d5d145515f368d76815e1fbfc0de2319a6505783c16e47489bac`（封印・中身未開封）
- `sha256(vnext/extract_full/signal_full_v2_lockbox.parquet)` = `ee5a4a408ec5310f78297aa28e2fa902e89cbe82ae95d8eea30b94281955bf95`（封印・中身未開封）
- `sha256(vnext/extract_full/FULL_EXTRACT_MANIFEST_v2.md)` = `695b6d0ba3c069b475313fdc8b4e04c7374d50f0918bb9420214d142090b7ca4`

## 備考

- タイムゾーン: 上記GitHub API日時はすべてUTC。ローカル記録（`HASHES.md`の
  `recorded=2026-07-16 22:42:20`、環境のJST想定）とは約9時間のオフセットがあり、
  UTC 13:42台 = JST同日22:42台として整合する。
- `signal_full_v2.parquet`（3分割前の全量ファイル）自体は本登録の対象外（TRACKV-EXTRACT-FULL-002
  Task 5の指示どおり「3ファイル＋マニフェスト」の4件のみを登録）。行数・レース数・SHA256等の
  管理値は `FULL_EXTRACT_MANIFEST_v2.md` 内に別途記載済み。
- 本ファイルの内容は `decisions.md` へ転記するための一次証跡である。本ファイル自体は
  `keiba-research-hashes` 配下（本体プロジェクト外）にのみ存在し、本体プロジェクトの
  ファイルへの書き込みは行っていない。
