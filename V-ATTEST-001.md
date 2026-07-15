# V-ATTEST-001 — CH1〜CH22 章別verdict・確定日 一覧（証跡転記文書）

## 0. 本文書の位置づけと宣言文

**本文書の外部登録時刻を `provable_prospective_from`（実証可能な事前主張時点）の起点とする。**

本文書は、研究プロジェクト本体（`keiba-research/keiba-research`）の一次記録である
`decisions.md`・`decisions_history.md`・`STATE.md`・`STATE_HISTORY.md`（および各章の
`ROADMAP_CH{n}.md`・`results/ch{n}_chapter_text.md`・`results/final_synthesis_report.md`等）
から、既に確定済みの内容を**転記**したものであり、本文書自体が新たな判定・数値計算・
解釈を行うものではない。

一次記録それぞれの作成日時（下表「確定日」欄）は、あくまで**研究側の自己申告
（append-only台帳・ファイルmtimeによる内部記録）**であり、それ自体に対する外部証跡
（第三者が検証可能なタイムスタンプ）は本文書の作成時点では存在しない。すなわち
「各章が実際にその日付に確定していたこと」を本文書は証明しない。

本文書が証明できるのは、**本文書というファイルの内容が、外部タイムスタンプサービス
（例: OpenTimestamps等、`keiba-research-hashes` リポジトリの運用方式に準ずる）に
登録された時刻の時点で、この内容として存在していたこと**のみである。したがって、
下表に記載された章別の verdict・確定日という「主張」について、第三者が
「後出しではない」ことを検証できる起点（`provable_prospective_from`）は、
一次記録の日付ではなく、**本文書が外部登録された時刻**である。

- 本文書の作成日: 2026-07-16
- 転記元ファイル（プロジェクトルート `keiba-research/keiba-research/` 直下、
  `orchestrator/snapshots/` 配下や `*_backup*.md` 等の過去スナップショットは転記対象外）:
  - `decisions.md`
  - `decisions_history.md`
  - `STATE.md`
  - `STATE_HISTORY.md`
  - 補助的に章タイトルの特定のため `ROADMAP_CH{n}.md`（第5〜22章）、
    `results/ch{n}_chapter_text.md`、`results/final_synthesis_report.md`、
    `results/ch3_conclusions_final.md`、`results/ch4_skeleton_final.md` を参照した
    （これらも一次記録の一部であり、上記4ファイルの内容と矛盾しない）。
- 本文書は「本物」「賭けてよい」等の断定表現を含まない。verdict はすべて一次記録からの
  逐語またはそれに準ずる要約転記であり、格上げ・解釈の追加は行っていない。

---

## 1. CH1〜CH22 一覧表

| 章 | タイトル | verdict | 確定日 | 出典 |
|---|---|---|---|---|
| CH1 | **未特定** — `decisions.md`/`decisions_history.md`/`STATE.md`/`STATE_HISTORY.md` のいずれにも「第1章」「CH1」という独立した章バッチ・タイトル・verdictの記載を確認できなかった。プロジェクトの最初期記録は2026-06-15のSTEP-AUDIT（シグナル来歴監査）で、章番号付けは後述CH3から開始されている。 | 未特定 | 未特定 | 該当なし（不在を確認） |
| CH2 | **未特定（部分推定）** — 独立した「CH2」バッチは確認できないが、`results/final_synthesis_report.md`（batch_id: CH3PLUS-FINAL-SYNTHESIS-001）内に「第2章で確立された5軸定義・v6確定方針」という遡及的言及がある。5軸（axis_form/axis_human/axis_class/axis_context/axis_train）定義とv6スコアエンジン確定方針を指すと推定されるが、専用の章バッチID・単一の確定日は一次記録中に見当たらない。 | 未特定（遡及言及のみ、独立verdict行なし） | 未特定 | `results/final_synthesis_report.md` §結論、§1.2-1.3（参照のみ、日付記載なし） |
| CH3 | 経路依存性研究プログラム — 水準シグナルの市場吸収（`CH3_FINE_MARKET_CONTROL_COMPLETE_COARSE_ARTIFACT_CONFIRMED`）と経路効果（LATE_STEAM等）の学術的頑健性・執行可能性の検証 | `CH3_FINE_MARKET_CONTROL_COMPLETE_COARSE_ARTIFACT_CONFIRMED`（水準シグナル全滅）／`CH3_TIMESERIES_ABSORPTION_COMPLETE_MARKET_ABSORBS_EARLY`／経路効果は`PATH_EFFECT_ROBUST_FINE`だが執行可能性は`EXEC_SIGNAL_DIES_LOOKAHEAD_ONLY`で研究的事実・執行不能としてclose | 2026-07-02（第3章結論の最終集約: CH3PLUS-FINAL-SYNTHESIS-001） | `results/ch3_conclusions_final.md`、`STATE_HISTORY.md`（CH3-FINE-MARKET-CONTROL-ARTIFACT-AUDIT-001等） |
| CH4 | 予測上限の情報理論的形式化 — Plackett–Luceモデルによる市場÷oracle-ceilingの推定（luck floor） | `CH4_LUCK_FLOOR_ESTIMATED`（市場÷oracle-ceiling=119.3%/119.1%等、Track Qで頑健性確認済み） | 2026-07-02（CH4-LUCK-FLOOR-FORMAL-001） | `STATE_HISTORY.md:3581-3582`、`results/final_synthesis_report.md` §2 |
| CH5 | 情報到着の期間構造と執行境界の定量化 | `RESEARCH_FIX_v2`確定（司令塔サインオフ済み）。第2〜5章は本サインオフをもって凍結。ROADMAP_CH5.mdは本行をもってclose | 2026-07-03（CH5-CHAPTER-TEXT-001 / R10） | `STATE_HISTORY.md:5651-5665`（見出し「CH5-CHAPTER-TEXT-001 / R10 ＋ ARCHIVE-MAINT-002（2026-07-03）」）、`ROADMAP_CH5.md`（見出し行） |
| CH6 | ラストマイルの解剖学 — 分布・形状・フロー | `RESEARCH_FIX_v3`確定。第6章の確定verdict: R11=`LASTMILE_TAIL_BODY_STRUCTURE_CONFIRMED`／R12→R12b=`EXEC_REOPEN_ARTIFACT_CONSISTENT`／R13→R13b→R13c=着地1（アーティファクト再分類、クローズ）／R9'=`PARIMUTUEL_IMPACT_DATA_INSUFFICIENT`／R14=`LASTMILE_FLOW_UNDETERMINED`。第2〜6章は本記録をもって凍結 | 2026-07-04（CH6-LANDING1-SIGNOFF-BUNDLE-001） | `STATE_HISTORY.md:4929-4991`（見出し「CH6-LANDING1-SIGNOFF-BUNDLE-001（2026-07-04）」）、`ROADMAP_CH6.md`（見出し行） |
| CH7 | 市場の解読と準効率市場下の意思決定（Track R / Track B 二部構成） | `RESEARCH_FIX_v4`確定（Track R）／`BETTING_FIX_v1`確定（Track B）。Track R確定verdict: D3=`DECOMP_ASSETS_READY`／R16=`SURROGATE_DECOMPOSITION_REPRODUCED`／R17=複合（`PRIVATE_RESIDUAL_INFO_CONFIRMED`＋`EXEC_REOPEN_CANDIDATE_FLAGGED`）→R17b/R17cを経てクローズ。第2〜7章は本記録をもって凍結 | 2026-07-05（CH7-PAPERIZATION-AUTORUN-003 / R19'・E9'） | `STATE_HISTORY.md:6310-6330`（見出し「CH7-PAPERIZATION-AUTORUN-003 — R19'（2026-07-05、Track R本文最小差分＋RESEARCH_FIX_v4確定）」）、`STATE.md:251`、`ROADMAP_CH7.md`（見出し行） |
| CH8 | 市場情報集約の科学 — FLBの情報論的分解・残差の実体持続性・構造不変性（Track S）＋Daily翻訳レーン | `CH8_TEXT_COMPLETE` + `PAPER5_PREPRINT_DRAFT_READY` | 2026-07-06 | `decisions_history.md:619`（CH8-TEXT-001 (C1)）、`ROADMAP_CH8.md`（見出し行） |
| CH9 | レジーム異質性の機構測定 — 情報集約構造の条件依存性と残差実体分析の再挑戦（Track S続章）＋Daily翻訳レーン | `CH9_TEXT_COMPLETE` + `PAPER6_PREPRINT_DRAFT_READY` | 2026-07-07 | `STATE_HISTORY.md:7048`（見出し「CH9-TEXT-001 (C1) — 完了（2026-07-07）」）、`ROADMAP_CH9.md`（見出し行） |
| CH10 | 頭数閾値の局在化と情報帰属構成の再配分構造 — レジーム機構測定の深化（Track S続章）＋Daily翻訳レーン | `CH10_TEXT_COMPLETE` + `PAPER7_PREPRINT_DRAFT_READY` | 2026-07-08 | `STATE_HISTORY.md:7538`（見出し「CH10-TEXT-001 (C1) — 完了（2026-07-08）」）、`ROADMAP_CH10.md`（見出し行） |
| CH11 | 帰属閾値の来歴監査 — 観測カバレッジ構造と市場情報構造の分離、およびsplit分岐の統計的機構（Track S続章）＋Daily翻訳レーン | `CH11_TEXT_COMPLETE` + `PAPER8_PREPRINT_DRAFT_READY` | 2026-07-09 | `decisions_history.md:985`（CH11-TEXT-001 (C1) VERIFY-AND-RECORD）、`ROADMAP_CH11.md`（見出し行） |
| CH12 | ゲートの外側を測る — ゲート非適用調教特徴量による市場帰属の全観測域再測定、ゲート情報損失の定量、実欠測の情報性（Track S続章）＋Daily翻訳レーン＋v-next提案レーン | `CH12_TEXT_COMPLETE` + `PAPER9_PREPRINT_DRAFT_READY` | 2026-07-10 | `STATE_HISTORY.md:8668`（見出し「CH12-TEXT-001 (C1) — 2026-07-10」）、`ROADMAP_CH12.md`（見出し行） |
| CH13 | 開催日の中の市場 — 日内セッション位置（レース番号帯）による価格形成・市場帰属・較正構造の変化の実測（Track T新設）＋Daily翻訳レーン | `CH13_TEXT_COMPLETE` + `PAPER10_PREPRINT_DRAFT_READY` | 2026-07-11 | `decisions_history.md:1119`（CH13-TEXT-001 (C1)）、`ROADMAP_CH13.md`（見出し行） |
| CH14 | ゲート位置の市場 — 枠番・馬番（発走位置）情報の価格反映・較正・帰属構造・吸収タイミングの実測（Track U新設）＋Daily翻訳レーン | `CH14_TEXT_COMPLETE` + `PAPER11_PREPRINT_DRAFT_READY` | 2026-07-11 | `decisions_history.md:1481`（CH14-TEXT-001 (C1)）、`ROADMAP_CH14.md`（見出し行） |
| CH15 | 並行プールの市場 — 単勝・複勝・枠連の券種間価格整合・較正・情報集約構造の実測（Track V新設）＋Daily翻訳レーン | `CH15_TEXT_COMPLETE` + `PAPER12_PREPRINT_DRAFT_READY` | 2026-07-11 | `decisions_history.md:1534`（CH15-TEXT-001 (C1)）、`ROADMAP_CH15.md`（見出し行） |
| CH16 | クラス階層の市場 — レースクラス別の価格集中・較正・クラス遷移の価格付け・情報吸収構造の実測（Track W新設）＋Daily翻訳レーン | `CH16_TEXT_COMPLETE` + `PAPER13_PREPRINT_DRAFT_READY` | 2026-07-12 | `decisions_history.md:1563`（CH16-TEXT-001 (C1)）、`ROADMAP_CH16.md`（見出し行） |
| CH17 | 馬場状態の市場 — 馬場（トラックコンディション）別の価格集中・較正・道悪適性の価格付け・馬場変化情報の吸収構造の実測（Track X新設）＋Daily翻訳レーン | `CH17_TEXT_COMPLETE` + `PAPER14_PREPRINT_DRAFT_READY` | 2026-07-13 | `STATE_HISTORY.md:11059`（見出し「CH17-TEXT-001 (C1) 総括（2026-07-13・完走）」）、`ROADMAP_CH17.md`（見出し行） |
| CH18 | 価格の時間構造の市場 — オッズ時系列断面別の較正精度・FLBの断面間変化・断面間乖離の解消方向・移動規模と最終較正の実測（Track Y新設）＋Daily翻訳レーン | `CH18_TEXT_COMPLETE` + `PAPER15_PREPRINT_DRAFT_READY` | 2026-07-13 | `STATE_HISTORY.md:11580`（見出し「CH18-TEXT-001 (C1) 総括（2026-07-13）」）、`ROADMAP_CH18.md`（見出し行） |
| CH19 | 騎手情報の市場 — 乗り替わりという公開情報の価格構造・較正・構成統制・吸収タイミング・階層移動方向の非対称の実測（Track Z新設）＋Daily翻訳レーン | `CH19_TEXT_COMPLETE` + `PAPER16_PREPRINT_DRAFT_READY`（crosscheck100%, fig6/6, forbidden_word=0） | 2026-07-14 | `decisions.md:720`（CH19-TEXT-001 (C1)）、`ROADMAP_CH19.md`（見出し行） |
| CH20 | 馬体重という公開情報の市場 — 馬体重増減の価格構造・較正・構成統制・吸収タイミング・増減方向の非対称の実測（Track AA新設）＋Daily翻訳レーン | `CH20_TEXT_COMPLETE` + `PAPER17_PREPRINT_DRAFT_READY`（figs=6/6, citation_todo=11, qualifiers=43） | 2026-07-14 | `decisions.md:747`（CH20-TEXT-001 (C1)）、`ROADMAP_CH20.md`（見出し行） |
| CH21 | 市場の相補情報 — de-vig市場価格は公開ハンディキャップ要約に直交して較正情報を載せているか（市場情報集約の相補分解・セグメント集中・逆較正局在）（Track AB新設）＋Daily翻訳レーン | `CH21_TEXT_COMPLETE` + `PAPER18_PREPRINT_DRAFT_READY`（crosscheck=100%, banned=0, mtime=match） | 2026-07-14 | `decisions.md:764`（CH21-TEXT-001 (C1)）、`ROADMAP_CH21.md`（見出し行） |
| CH22 | 距離変更の市場織り込み — 前走からの距離延長・短縮という顕著な公開条件変化を、群衆はどこまで正しく価格化しているか（価格構造・帯別較正・方向非対称・初距離の不確実性プレミアム・吸収タイミング）（Track AC新設）＋Daily翻訳レーン | `CH22_TEXT_COMPLETE` + `PAPER19_PREPRINT_DRAFT_READY`（citegrep=100%, bannedwords=0） | 2026-07-15 | `decisions.md:809`（CH22-TEXT-001）、`ROADMAP_CH22.md`（見出し行） |

---

## 2. 特記事項（未特定・不確実な項目の正直な注記）

1. **CH1**: 一次記録4ファイルのいずれにも「第1章」「CH1」という独立した章バッチの
   存在を確認できなかった。プロジェクト最初期の記録（2026-06-15、STEP-AUDIT）は
   シグナル来歴の監査であり、章番号体系の外にある。CH1という章が実在するか自体、
   本転記の範囲では確認不能。
2. **CH2**: 同様に独立バッチは未確認。`results/final_synthesis_report.md` に
   「第2章で確立された5軸定義・v6確定方針」という遡及的な言及が1箇所あるのみで、
   単一の確定日・単一のverdict文字列としては特定できなかった。5軸定義および
   v6確定方針に関連する個別の記帳は2026-06-15〜2026-07-02の間に多数散在しており、
   どの記帳をもって「第2章の確定」とするかは一次記録上一意に定まらない。
3. **CH5〜CH7**（登録直前grepで補完、2026-07-16）: 当初探索では`CH{n}-TEXT-001`形式の
   単一verdict行を発見できていなかったが、追加grep（`CH5-`/`CH6-`/`CH7-`×
   `TEXT-001|FINAL|CLOSED|SYNTHESIS|VERDICT|verdict`）により、CH5〜CH7では
   `CH8-TEXT-001`以降とは異なる命名規則（`RESEARCH_FIX_v{N}`タグ確定という形式）で
   章クローズが記録されていることが判明した。CH5=`RESEARCH_FIX_v2`
   （`STATE_HISTORY.md:5651`）、CH6=`RESEARCH_FIX_v3`（`STATE_HISTORY.md:4929`）、
   CH7=`RESEARCH_FIX_v4`+`BETTING_FIX_v1`（`STATE_HISTORY.md:6310`）として上表を
   更新済み。第4章の`RESEARCH_FIX_v1`が同系列の最初の例であり（CH4行参照）、
   `CH{n}-TEXT-001`命名は実質的にCH8章以降で採用された規則であると判断できる。
4. **CH3の確定日**: CH3は複数のサブバッチ（CH3-FINE-MARKET-CONTROL-ARTIFACT-AUDIT-001、
   CH3-MARKET-TIMESERIES-INFORMATION-ABSORPTION-001、CH3-PARIMUTUEL-OS-EQUILIBRIUM-001、
   CH3-PENDING-TRIAD-001等、2026-07-01〜07-02）から構成される。表中の確定日は
   最終集約バッチ（CH3PLUS-FINAL-SYNTHESIS-001、2026-07-02）の日付であり、
   個々のサブ結論の確定日はそれぞれ異なる。
5. 本表の「出典」欄に記載した行番号は転記時点（2026-07-16作成の本文書作成過程）の
   ものであり、`decisions_history.md`・`STATE_HISTORY.md` は append-only での
   追記が続くため、将来的に行番号がずれる可能性がある。ファイル内容そのものの
   sha256ハッシュによる照合は `keiba-research-hashes/HASHES.md` を参照。
6. 本文書はCH1〜CH22のみを対象とする（ユーザー指定範囲）。CH23以降は本表に含まない。

---

## 3. 免責

本文書は研究記録の証跡整理であり、馬券購入の推奨・投資助言ではない。verdict欄の
文言はいずれも一次記録からの転記であり、本文書独自の「本物」「賭けてよい」といった
格上げ的評価は一切含まない。
