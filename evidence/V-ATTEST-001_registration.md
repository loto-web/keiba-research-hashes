# V-ATTEST-001 registration evidence

本ファイルは `V-ATTEST-001.md`（CH1〜CH22 verdict preregistration attestation）を
`keiba-research-hashes` リポジトリへ登録した際のサーバ側（GitHub）証跡を記録する。
本ファイル自体もこのリポジトリの一部としてadd/commit/pushされる。

## 登録コミット

- commit hash (full, HEAD at registration): `4e65683211a045239ade8d6270a64b2823e20bfd`
- commit message: `Register V-ATTEST-001: preregistration of CH1-CH22 verdicts (prospective clock start)`
- commit author/committer date (GitHub API, UTC): `2026-07-15T23:28:18Z`
- files changed: `HASHES.md`（追記1行）, `V-ATTEST-001.md`（新規107行）
- html_url (commit): https://github.com/loto-web/keiba-research-hashes/commit/4e65683211a045239ade8d6270a64b2823e20bfd
- push range: `d960b1c..4e65683`（本コミット含め計3コミットが同一push操作でorigin/mainへ反映。
  うち先行2コミット `865cb38`（hash registry +2 new）・`4c065c8`（ots stamp, pending Bitcoin
  confirmation）は本セッション以前に既にローカルへコミット済みだった未push分であり、
  V-ATTEST-001登録作業自体の一部ではない）。

## GitHubリポジトリAPI応答（`GET /repos/loto-web/keiba-research-hashes`）

- `pushed_at`: `2026-07-15T23:28:31Z`
- `html_url` (repo): https://github.com/loto-web/keiba-research-hashes
- `default_branch`: `main`
- `created_at` (repo): `2026-07-13T09:27:57Z`

`pushed_at`（23:28:31Z）はコミットのauthor/committer date（23:28:18Z）の13秒後であり、
登録push操作と時間的に整合する。

## sha256（本文書が証明対象とするファイル）

- `sha256(V-ATTEST-001.md)` = `611b17b1e4cf21ca0444ff227e66407e76446d7f57c36a26e3dacabe7146ac83`
  （`HASHES.md` 末尾行として同一値を記録済み）

## 備考

- タイムゾーン: 上記GitHub API日時はすべてUTC。ローカル記録（`HASHES.md`の
  `recorded=2026-07-16 08:27:42`、環境のJST想定）とは約9時間のオフセットがあり、
  UTC 23:28台 = JST翌日08:28台として整合する。
- 本ファイルの内容はオオシマさんが `decisions.md` へ転記するための一次証跡である。
  本ファイル自体は `keiba-research-hashes` 配下（本体プロジェクト外）にのみ存在し、
  本体プロジェクトのファイルへの書き込みは行っていない。
