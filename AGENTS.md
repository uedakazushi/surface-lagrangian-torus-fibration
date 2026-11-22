# surface-lagrangian-torus-fibration — 研究・保存指示
2026-11-23 / v2.11

## 公表計画の実行

- 最上位の目的は数学的価値の最大化。現在の公表計画と担当作業は `00_research_plan.md` 冒頭に置く。中心結果の正確性・新規性・読者の検証可能性を優先し、既存の論文順や未解決atlasの完成を他の成果の公表条件にしない。
- 計画をmainへ保存した後、証明・先行研究比較・原稿整理を実行し、実際の点検範囲と残る課題を現行資料へ反映する。計画を書いただけで研究完了とはしない。

## 入口と正本
- 研究全体の入口は https://github.com/uedakazushi/research-hub 。再開時はhubの該当項目を確認し、最初にこのrepoの `00_research_plan.md`、次に本書、`research/notes.md` と必要な原稿を読む。
- 本研究の現行資料の正本はGitHub `main`。主たる公表用原稿は `papers/surface-lagrangian-torus-fibration.tex`（本文のある主原稿）であり、節分割可。独立論文は記述的な別名を付け、READMEと研究方針に役割を明記する。
- 一般原則と研究固有の目標を区別する。研究で使う文献、証明、再現入力の正本は当該repoに置く。

## 三研究の共同編集と証明の正本

- `multiscale-kaehler-einstein`（固定SNC・配置補空間のPart I–III）、`kaehler-einstein-degeneration`（退化族の局所一様解析Part IV・条件付き大域枠組Part V）、本repo（actual KE–Lagrangian構成と同じ写像の大域GH実現）を一つの研究計画として監査・編集する。リポジトリと本文の正本はこの分担で維持し、独立な論文を自動的に統合・複製しない。
- 同じ射影のatlas/GH同時実現を進めるときは `ke:moment-relative-replacement` の保持corner全葉・source近傍・canonical moment・anchor cuts・marked閉商の条件を先に照合する。この条件下のGH安定性、成分別の相対面積実現とstrict cut判定、sourceを保持する微小変更、actual coreの有限anchor-period条件は本文に証明がある。五次では `ke:k4-actual-neck-periods`、`ng8:quintic-full-moment`、`ke:quintic-simultaneous-realization` により、初期source葉を選んだ所定targets・全moment・両側neckの切片/framing・全open overlapsと同じ射影のatlas/GHを構成した。六次では `ke:petersen-full-moment` と `ke:sextic-simultaneous-realization` により、等重み・初期source葉選択の同時atlas/GH/測度を構成した。次は未点検の最小解析入力と一次比較に公表前監査を絞り、先指定追加保持集合への拡張を独立課題として扱う。Source固定点を横切る全intervalへfree-bandの面積affine性を流用せず、`ng8:source-dh-wall` と固定fiber版の適用条件を読む。
- 各作業は利用側の主定理から逆向きに、入力の定理ラベル・仮定・対象領域・計量の尺度・定数とcutの選択順序を確認する。共通の詳しい接続表は本repoの `research/ke-dependencies.md`、シリーズの見通しはmultiscale側の `papers/series-overview.tex`、短い進捗と再開先はresearch-hubが正本。各repoの証明・詳細todoをhubへ転載しない。
- 固定補空間の空間的blow-down、固定compactでの退化族の収束、選択した遅いexhaustionでの一様評価を区別する。成分は $\mathbb P^2$ から $d-1$ 本の直線を除いたもの。固定成分の漸近錐とcubical targetの局所幾何の一致から、任意のmoving領域の解析評価を推論しない。
- Surfaceの直接scalar/portal証明を、外部のCP/PBE/TCやPart IIIのH_loc/H_ancの検証へ読み替えない。Part IIの標識付き複素・双曲periodと本稿の第二作用periodも同一視しない。五次の同じ射影によるatlas/GH同時実現は初期source葉を選ぶ存在定理として本文に証明があり、六次でも標準等重みPetersen targetsについて同じ射影のatlas/GH/測度を証明した。
- 入力を訂正した場合は、その正本を先に直し、利用側の依存表・本文・要約へ波及を反映する。三repoを保存して確認した状態に基づきhubを更新する。異なるrepoの並行変更を保持し、固定した確認commitと最新mainとの差を確認してから引用を更新する。

## この研究の最優先目標と自走指示

最優先は `00_research_plan.md` のP0、すなわち**本研究のactual Lagrangian fibrationが負KE計量のGH極限を幾何学的に実現すること**である。精密な主張は主稿の `ke:global-realization`、統合証明は `ke:global-metric-realization`。任意の固定次数d≥5について、実際のKE形式に関する大域fibrationと、合成写像p_Tπ_tの全曲面ambient距離に対する一様distortionの消失を証明する。現行主稿では全固定d≥5に対する証明を統合し、新証明と接続に必要な箇所を内部点検している。共通anchorでの保持neckのmoment範囲と、同一momentのcorner参照点による全域値比較を明示し、固定残余基底の有限cutに一様なMoser被覆・接続を用いる。Closed-cornerは有限cutの明示条件で一様に比較し、全target端点のportalと全fiber合併をambient距離で扱う。Sourceの全moment退出は三境界Schwarzから得るarm tensor比較によりO(1)であり、中央点の直接退出もGaussian可積分性に依存せず証明した。Componentのcore・collarとneck尾部の費用をC(1+log(N_j+1))で評価し、残余基底の先行選択から全fiber合併・portalにも同じ予算を得た。Compact-relative Morse–Smale化でcore skeletonの閉isotropic filtrationを明示し、primitive・nontrapping・相対補間・全fiber trimも重点監査した。Core経路の構成の同一性・支持・量化に限定した独立内部監査を完了し、全K2交わりの恒等collarと補間後partitionの全fiber trimを明示した。相対flux空間と小さい非延長germ、contact rescalingの固定葉非保存例は任意指定germの延長とfibration構成を区別するために使う。固定coupling chartsでのbasic＋exact-cutoff経路は各成分のg_a個の正則葉periodの消滅と同値であり、障害次元・最小holonomy調整rankはいずれもΣg_aと本文に証明した。正則bandの第二作用判定とcanonical frameの残余period差、同じ形式・normal action・端とsaddle点のgermsでもcritical actionが曲がる反例を本文に保持する。Sourceのtransversality判定、一重focus近傍の一つの残余periodによるexactness、通常のTaylor不変量とprimitiveの定数項、全飽和近傍の移送を本文に統合した。例外面積を規格化したradial Kähler blow-upと、CG比較の飽和patch外恒等・全compact nodal neighborhoodsの保持も明示した。有限閉whole-fiber quotient、同じ合成写像の全fiber連結性、Euler関数の有限支持とcoarse fiber公式を本文に整理した。一般存在の任意marked trees、P0の固定族から選ぶ一つのT、作用atlasの一般存在と五次・六次の同じ射影の追加構成を区別する。五次では、finite endpoint条件と全moment面積実現を組み合わせ、同じπでatlasとGHを同時実現する証明を統合した。六次では等重み・標準Petersen targetsと初期source葉の選択により、全moment・全open接着を経て同じ射影のatlas/GH/測度を証明した。七次以上では同じP0基底の各coreの局所matroidal chartが位相的に不可能だが、metric結論は保たれる。次は五次・六次の同時実現を中心に、未点検の最小解析入力・使用域と一次比較に公表前監査を絞る。六次標準targetsの有限条件・内部二端cuts・全moment・両端全葉の整合は本文の証明を正本とし、追加保持集合・任意weightsへの拡張は未解決条件として扱う。任意focus不変量の先指定へ広げず、既存P0を優先し、形式証明・外部査読や新規性確認と混同しない。

- 本目標の解決へ向けた証明、反例の探索、必要な計算、一次文献確認、現行文書と再現手順の更新は継続して実行する。通常の研究上の選択ごとに「続けてよいか」と確認せず、計画だけを作って終了しない。独立した五次整数接着分類・三次元研究へ、P0との依存理由なく優先対象を移さない。
- 再開時は最新mainと作業ツリー・並行変更を確認し、研究方針 → 本書 → `research/ke-dependencies.md` → `research/notes.md` → 必要な原稿の順に読む。環境の具体的な入口は `research/cloud-codex.md`。会話履歴、旧bundle、前回の一時ディレクトリを前提にしない。
- 方針の最優先課題から着手する。現行ではK0/K5の指定証明鎖と五次・六次同時実現の独立内部点検を終えたので、依存表から未点検の最小解析入力・使用域と一次比較を特定して公表準備を進める。既点検鎖の一律な反復はしない。各作業単位で仮定・領域・定数の依存・証明する補題を特定し、証明または明確な障害を得るまで検討する。独立な解析、接着、証明点検は可能なら分担する。
- 一つの方法が詰まったら、その失敗が計算上の問題か、未証明入力か、反例によるものかを区別し、ノートに本質的障害だけを残す。より弱い十分条件、直接の距離比較、別の局所構成、独立な次の課題へ進む。同じ未検証仮定を言い換えて証明済みにしない。
- K1–K4の成果は適切な主稿の節と現行ノートへ統合し、証明済み・条件付き・未完成の状態と次の具体的補題を研究方針で更新する。文書整備・検算成功・部分結果をP0の完了と報告しない。
- P0を完了とする前に、全特異領域を含む全射性・連結fiber、actual Lagrangian性、全域distortion、全固定dの範囲、依存証明・一次資料を点検する。重要な新証明は可能なら別agentが独立に点検する。数学的点検と形式証明を混同しない。
- 反例が得られたら元の主張と依存主張を訂正し、どの条件を変えれば正しいかを証明とともに整理する。反例を隠すための無言の目標縮小や、仮定の追加だけによる完了宣言はしない。
- 実行時間やサービスの制約で作業が区切られる場合も、その時点の有効な結果・未解決の補題・再開先をmainへ保存する。アクセス不足なら利用可能な課題を続け、未保存分は下記の緊急保存方針に従う。リポジトリへの指示の保存と、Cloud環境の設定・タスク開始・継続実行は別の状態として報告する。

## P0で維持する数学的な区別

- 六次の標準同時実現は `ke:petersen-actual-neck-periods` → `ke:petersen-two-end-cuts` → `ke:petersen-balanced-separator` → `ke:petersen-thin-source-block` → `ke:petersen-full-moment` → `ke:sextic-simultaneous-realization` を正本とする。等重みの一意性はzero-external targetsの指定framingに限る。内部source blockの幅と累積位置を区別し、正margin後に中央helperをfreezeしてからfull source annuliを固定する。Core domain・primitiveは先、anchor葉とfillingは全moment構成の後に選ぶ。Source-free anchor bandsの全open接着と、A/B別starの平行移動付き三面transitionを保持する。指定鎖の独立内部点検済みという状態を、全主稿・全K2入力の再監査や形式証明へ読み替えない。現行版の組版・実表示の範囲は検証資料の実施記録で確認し、旧版の結果で代用しない。

- 公表比較ではFBPの明示GH近似・properな全fiberの補助Kähler GHを既存結果として扱い、actual KE形式・同じ全域射影・ambient距離の同時達成を区別する。双対複体との同相/細分を計量の一致へ読み替えず、異なるparameterや尺度の量化を明記する。
- `ke:projected-source-normal-form` の定義域は固定残余基底を先に選ぶ。正逆の共通tube・全orbit・全小複素parameterの量化を保つ。`ke:fixed-cutoff-volume-transport` のcutoff Aと退化尺度R_tを区別し、Part IのCe^{-A}だけからtの有効収束速度を推論しない。Part IVの縮むbufferに対する円周評価はactual bufferの存在を仮定し、その供給やMoser生存を自動的に含めない。

- 五次同時実現の公表原稿では、`ke:eq:quintic-affine-full-transition` の平行移動を含む三面の整数アフィン接続、全open germs、解析選択後のthin代表 $H_{r,t}$ の役割を保持する。旧 `ng8:relative-dh`・`ng8:straight-neck` はnodal neighborhoodsを避けたfree neckの結果であり、source-inclusive全momentへ流用しない。各tで同じ射影にatlasとGHを持たせることと、atlasのparameter極限又は極限計量のHessian性は区別する。

- Ric(ω_t)=−ω_t、R_t=log(−log|t|²)、計量R_t^−2g_t、距離R_t^−1d_gを使う。正規化前の成分内部の四次元極限と混同しない。
- Mainの定性的存在結果から無制御にMoser移送しただけでは計量適合性を得ない。局所closed-cornerの内在/protected距離を全曲面のambient距離に読み替えない。
- KE側の(G)_d・(CP)_d・(PBE)_d、五次coarse packageの(TC)_5は実際の仮定を確認する。未解決入力は証明するか、同等に十分な別の全域評価で置き換える。Bounded volume densityはtensor二側比較を含意しない。
- d≥6ではp_Tが潰す木の上の全fiberの合併を制御する。Normal circleの一致とreduced葉・第二periodの一致、位相的同型と計量的一様性も区別する。P0に大域matroidal atlasや最適収束速度を追加要求しない。
- 全域quotientでは全overlapのwhole-fiber飽和と閉同値関係を確認し、基底同相の存在をHausdorff性の根拠に循環使用しない。π_tとp_Tのconnected fibersから合成の連結性は閉写像の逆像連結性で示す。合成fiberは三次元部分を含み得るのでLagrangian性と混同しない。Euler関数はnodes・coresの有限支持を用い、面ごとのnode配分を具体的recipeから一般P0へ拡張しない。
- 一般存在の「任意marked T」とP0の「固定族→選んだ一つのT→全小t」を区別する。P0にt-smooth familyを追加しない。d=5では新定理の初期source葉選択・全momentと全葉接着の条件下でatlas/GHを同時実現する。d=6は等重みPetersen targetsについて、別に証明した内部二端cuts・balanced separator・中央freeze・全moment構成から同時実現する。五次の定理だけをPetersenへ流用しない。任意先指定の大きいsource近傍を保つ相対変更も主張しない。d≥7の局所matroidal core障害は同じcore・木系を保つP0基底についての結論であり、異なる基底を許す全fibrationへの不存在へ拡張しない。FBP Theorem 6.14(b)の部分fibrationと(c)の全fiber補助計量GHを区別し、先行結果を局所GHだけに縮小して比較しない。
- SNCではconnection/gauge固定とunitary holonomy phasesのみ固定を区別する。Basic補正を全critical collars外へ置けることから、非零葉periodを消すholonomy補正まで元のfull saddle collarsを固定できるとは結論しない。既知のIKMの成分原理とSNC統合、TMZのexact deformationとBSVのadapted primitive存在の適用範囲を分ける。
- 正則bandの第二作用の一致、primitiveに関するexact matching、critical actionの有理直線性を区別する。Normal actionと局所saddle germの一致から作用atlasを結論しない。Sourceのfocus局所型とcompact singular fiber近傍全体の同時移送も区別する。通常のTaylor不変量はsymplecticな全葉移送で保存され、primitiveの残余定数項にはexactnessが必要である。Node primitiveの固定だけでexactnessを推論せず、outer regular torusのperiodも確認する。Surgeryの比較写像は固定した飽和affine-convex patch外で恒等とし、球の外全体の恒等と取り違えない。任意の半大域focus不変量を指定できるとは主張しない。
- 解析入力の正本は `uedakazushi/kaehler-einstein-degeneration`、多重スケールの背景は `uedakazushi/multiscale-kaehler-einstein`。必要な定理のpath・label・確認commit・仮定を依存表で確認し、sourceを読んで使う。外部repoで作業するときはそちらの最新方針・AGENTSを先に読み、証明を二重管理しない。

## 研究の方針と確実性
1. 数学的重要性・新規性・理解の深化・応用可能性・正確性・実現可能性を総合し、目的と方針を柔軟に修正する。履歴を積み増す代わりに現行資料を整理する。
2. 証明済み・追加仮定付き・証明未完成・予想・計算観察を区別し、仮定・証明の所在・依存関係・未解決箇所を記録する。原稿に証明が存在することは、その証明を今回独立に監査したことと異なる。
3. 先行研究の一次資料を確認し、適用範囲と本研究の貢献をIntroductionに明示する。文献と新規性の未確認事項は憶測で埋めない。他repoの結果を使うときは具体的な定理と仮定を記す。
4. 論文は原則日本語のLuaLaTeX。https://github.com/uedakazushi/research-hub の `papers/paper-template.tex`, `papers/README.md`, `.latexmkrc`, `.vscode/` を参考にする。主原稿を改名するときはinput、分割原稿のTeX root、文献、README、設定も更新する。
5. 研究ノートは現行の着想・例・補題・計算・障害・文献比較を保持する。論文中の十分な証明は複製せず参照する。過去の会話や更新日誌・旧版ZIPを蓄積しない。
6. 誤りの判明時は依存する主張を含めて修正し、ノート・方針・公表原稿・hubの記述を一致させる。

## 保存と検証
- 現行資料だけで再開できるよう、ソース、必要な文献情報、再現コード、入力、証明書を保持する。軽量化を理由に価値ある証明を削らない。古い資料の有効部分を統合するまでは消去しない。
- **Cloud Codexの継続作業では、証明・検算・原稿の切りのよい区切りでこまめに保存し、前回の成功したpushから長くても約15分を目安に、現行の有効な成果を通常コミットしてGitHubの `main` へpushする。** 15分ちょうどを待たず、完了した補題・有用な反例・障害・中間の証明候補が生じた時点で保存する。長い計算・組版・文献調査に入る前にも可能な範囲で保存し、時間制限や中断に先回りする。時間計測・pushの機会がない実行環境では絶対的な時間保証はできないが、次の機会を待たず優先して保存する。
- **未完成でも再開可能な状態で保存する。** 証明候補・未検証の計算は完成結果と誤認させず、仮定、確実性、残るギャップ、次に試す具体的手順を現行研究ノート・方針へ統合する。独立に意味のある作業単位を小さく切り、15分の区切りで数学的な完成を無理に装わない。変更がなければ空コミットや日時だけの形式的pushはしない。
- **保存手順：** `git status` と `git fetch origin` で作業ツリーとリモート `main` を確認し、変更したファイルの範囲を点検する。時間のかからない範囲で `git diff --check` と関連する検査を行い、自分の変更だけを通常コミットする。リモートに並行変更があれば内容を確認して安全に取り込む（必要ならrebase等）、非fast-forwardを強制しないで `main` にpushし、`origin/main` の反映を確認する。重い全検証の完了を15分保存の条件にはせず、未実施の検証を明記して後続で実行する。
- push失敗時はネットワーク・認証・競合を区別して、安全に再試行する。研究は可能な範囲で続け、push不能ならローカルコミットと現行資料を保持し、緊急時のみLibraryへ保存する。前回成功pushから15分超の未保存作業を漫然と積み増さない。force push、他者変更の上書き、GitHub Actionsの追加・起動は禁止。hub更新は研究の実質的区切りに対象repo保存後に行い、15分ごとに内容が変わらないhubを機械的に更新しない。
- `latexmk` と VS Code LaTeX Workshopで組版し、SyncTeXとPDFを `build/` に整合させる。PDF・中間生成物は通常Git追跡しない。実行した数学的点検、計算、組版、pushは別々に報告する。
- `python3 scripts/research_check.py preflight` で依存環境、`python3 scripts/research_check.py static` で構成を確認する。TeXを変更したら `python3 scripts/research_check.py tex` で主稿を組版する。既存整数接着の有限検算は関連箇所を変更・使用した場合に `python3 scripts/research_check.py arithmetic` で行う。静的検査は数学の証明ではなく、整数検算はKEの解析的主張を検証しない。必要な検証ができなかったときは対象と理由を明記する。
- GitHub管理後はLibraryへの定常的二重保存/ZIP作成をしない。push不能時は緊急保存する。既存Libraryファイルは明示指示なしに削除しない。

## research-hub 更新義務
1. まず本repoの方針・原稿・ノート・READMEを最新の内容へ整理し、`main`へ保存する。
2. hubの最新READMEとAGENTS.mdを読んで、主要到達点・主張の状態・未解決の核心・次の一手・依存関係・正本・再開先・資料を実際に確認した日を更新する。
3. 詳細todo/証明/履歴はhubに転載しない。実質変更がないときは無用に更新しない。他項目と並行変更を保つ。
4. hubも通常コミットで`main`へ反映し、研究repo保存とhub更新の成否を独立に確認する。失敗した場合は対象と理由を報告する。公開範囲を勝手に変更しない。

## 回収した原資料の扱い
`research/source-manifest.json`と`research/migration.md`で全文・要約・未回収を区別する。移行完了の判定に短い要約を使わない。取得した最新版の訂正・追加仮定を旧稿の強い記述より優先する。保存済みの証明書と今回の再実行を混同しない。

## 複素次元3の正本との区別
三次元のfocus block・補集合の位相・全域存在問題は `https://github.com/uedakazushi/threefold-lagrangian-torus-fibration` を正本とする。曲面の主原稿、五次整数接着、KE適合は本repoで管理する。相互の結果は定理番号・適用仮定を明示して引用し、正本を二重化しない。

## 参照パスの現行運用
TeXの分割節と検証用proofは `papers/sections/{paper,paper_arithmetic,paper_surgery,notes}/` に置き、ルートsymlinkに依存しない。検算コードの参照を変えるときは `verification/run_current_checks.py` と `verification/verify_repository_layout.py` を照合する。旧検証JSON中の相対パス・SHA-256は歴史的な出典記録であり書換えない。ハッシュ確認は元コードとのパスだけの差を検証して数学的変更を許さない。現行のGitHub正本・hub更新義務は従前どおり。
