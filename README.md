# Lagrangian torus fibrations on general-type surfaces
2026-11-22 / v3.15 — [研究方針](00_research_plan.md) · [研究ノート](research/notes.md) · [Cloud Codexの再開手順](research/cloud-codex.md) · [research-hub](https://github.com/uedakazushi/research-hub)

**各固定次数 \(d\ge5\) の一般位置全平面退化について、actual負Kähler–Einstein形式の大域Lagrangian torus fibrationが、径の尺度のGH極限を実現する定理の証明を主稿に置いている。** 同じ写像 \(f_t=p_T\pi_t\) の全曲面ambient距離に関する一様distortionと、特異fiberを含む全fiber合併の収縮を扱う。今回の新証明と接続を複数担当で内部点検した。形式証明、全主稿・全外部入力の包括的再監査、外部査読、新規性の網羅的確認は未実施である。**このリポジトリは複素次元2専用**。三次元の研究は [threefold-lagrangian-torus-fibration](https://github.com/uedakazushi/threefold-lagrangian-torus-fibration) を正本とする。

## 三つの研究を通した編集

[multiscale-kaehler-einstein](https://github.com/uedakazushi/multiscale-kaehler-einstein) の固定補空間幾何（Part I–III）、[kaehler-einstein-degeneration](https://github.com/uedakazushi/kaehler-einstein-degeneration) の退化族解析（Part IV–V）、本repoのactual KE–Lagrangian実現を共同で監査・編集する。証明は担当repoを正本とし、原稿を複製・一括統合しない。詳しい定理・仮定・尺度の接続は [依存表](research/ke-dependencies.md)、シリーズ総説はmultiscale側、短い到達点と再開先は [research-hub](https://github.com/uedakazushi/research-hub) に置く。固定補空間の空間的極限と退化族の一様性、直接scalar/portal経路と未検証のCP/PBE/TC、複素periodと第二作用を区別する。

固定成分側のPart I v1.4では、全射な錐写像・一様閉球評価・LDPを保持し、ordinary volume-IRFAからの任意の深部平行移動とstripの全変動収束、metric-IRFAを加えたballの全変動収束とpointed measured GH収束、直接StokesによるChern–Weil・面質量の規格化を整理した。全faceの体積漸近から一様subcritical momentsを導くことで、Abel–Mellin recursionのweighted error条件と、exact tail/joint/Laplaceのexponential volume条件を追加仮定せずに済む。適用範囲と確認版は[依存表](research/ke-dependencies.md)に集約する。曲面側担当の直接点検は今回のChern–Weil・規格化の鎖であり、translation・強化したtail・Mellinは共同点検結果の同期である。これらの固定空間の結果をP0や中間尺度の新しい解析入力へ加えず、本repoの主稿は改訂33を維持する。

## 全域実現定理の内容

\(\operatorname{Ric}(\omega_t)=-\omega_t\)、\(R_t=\log(-\log|t|^2)\) とし、actual \(\omega_t\)-Lagrangianな大域fibration \(\pi_t:X_t\to B_d(T)\) を、標識付き基底収縮 \(p_T:B_d(T)\to\mathcal C_d\) と合成して
\[
\sup_{x,y\in X_t}\left|R_t^{-1}d_{g_t}(x,y)-d_\square(p_T\pi_t(x),p_T\pi_t(y))\right|\longrightarrow0
\]
を証明した。対象族は平面が一般位置、\(F_d\) が全三重点で非零かつ各二重線で相異なる単純零点を持ち、小さい非零parameterで滑らかという既存の一般性条件を満たす。全曲面のambient距離を用い、source・branch・coreの全特異fibersを含む。\(d\ge6\) では \(p_T\) が潰す内部木上の複数のfibersの合併全体も収縮する。主張は `ke:global-realization`、統合証明は [ke_global_metric_realization.tex](papers/sections/paper/ke_global_metric_realization.tex) の `ke:global-metric-realization`、定数と選択の範囲は [研究方針](00_research_plan.md) を参照。

証明は十分遅い対角選択と一つの許容された標識付き木系を用いる。最適収束速度、任意に先指定した木系への適合、次数一様性、全次数のmatroidal atlas、special Lagrangian性は結論に含めない。関連KE研究のCP/PBE/TCを証明したとはせず、本稿ではscalar Schwarz障壁による下界とportal接続による上界で代替する。必要な外部入力の所在と仮定は [依存関係表](research/ke-dependencies.md) にまとめる。従来の大域構成・作用適合atlas・整数接着の有効な成果も保持する。

### 固定成分と中間尺度の接続

主稿 `topo:component-cone-germ` は、固定成分の漸近錐 $C_{2,d-1}$ と $\mathcal C_d$ の成分頂点のmetric tangent coneを、半径 $r<1/2$ の閉球の厳密等長で同定する。`ke:intermediate-component-cone` は、同じ大域全射の歪みを $\epsilon_t$ として $1\ll a_t\ll R_t$、$R_t\epsilon_t=o(a_t)$ なら、actual曲面の距離 $a_t^{-1}d_{g_t}$ も成分頂点上の基点からこの錐へpointed GH収束することを示す。尺度は $a_t=R_t\sqrt{\epsilon_t+R_t^{-1}}$ と選べる。基点のtarget値のずれ $\eta_t$ も含めて $R_t(\epsilon_t+\eta_t)=o(a_t)$ とすれば、同じP0の一成分のcore・変更collarの全領域内の任意基点へ拡張できる。新証明は独立内部点検済みで、任意の尺度や極限交換、tensor収束は主張しない。K2の全交わりとK3の相対core接着の指定証明鎖も独立点検し、対象範囲で訂正を要するギャップは見つからなかった。

### 三つの存在主張の量化

| 主張 | 選択と結論 |
| --- | --- |
| 一般のsymplectic存在 `main:global` | 固定した $[\omega]=aH$ のKähler形式と、任意に選んだmarked pants treesに対して全域Lagrangian fibrationを構成する。計量崩壊を結論しない。 |
| P0 `ke:global-metric-realization` | 固定した次数・退化族ごとに一つの木系 $T$ を選び、全ての十分小さい $t\ne0$ に対してactual負KE形式の $\pi_t$ と同じ $p_T\pi_t$ のdistortion消失を得る。$t$ に関する滑らかなfibration族や任意指定 $T$ への適合は結論しない。 |
| 作用atlas `main:action-atlas` | $d=5,6$ では、critical areas・第二作用等を合わせた別の選択で大域作用適合matroidal atlasを持たせる。P0の同じ $\pi_t$ がこのatlasも持つとは証明していない。 |

五次・六次の同時atlas＋GH実現を進めるには、P0で保持するcorner・source近傍に相対的なcritical-area調整と、調整前後のGH比較写像の一様な変化の制御が必要であり、現状は未解決である。個別の存在定理や定性的なMoser移送を同時実現の証明に代用しない。

## Cloud Codexから再開する

最新mainで [研究方針](00_research_plan.md) → [AGENTS.md](AGENTS.md) → [依存関係](research/ke-dependencies.md) → [研究ノート](research/notes.md) を読む。主定理 `ke:global-metric-realization` から依存証明をたどる。Coreの正則化から指定actual collar、全域fibrationへ至る経路は、構成の同一性・支持・選択順序に範囲を限定して独立内部監査した。全K2交わりを恒等collarに含め、補間後の葉族を全fiber単位で切り詰めることを明示した。Sourceのfocus判定・全飽和近傍の移送と、nodal blow-upの面積・支持・選択順序を本文に明示し、必要箇所を内部点検した。有限閉whole-fiber quotient、同じ合成写像の連結fibers、fiber Euler関数の有限支持とcoarse fiberのEuler公式を本文に整理した。一般存在・P0・作用atlasの量化を分けて点検した。次は公表前監査を続け、Introduction・主定理のscopeを全域構成から逆向きに照合する。五次・六次の同じπによるatlas＋GHの同時実現には、相対critical-area調整とGH比較写像の変化の制御が未解決条件として残る。無限個のbranch fibersと有限個のbranch strata、πのLagrangian fibersと合成写像のfiber合併を区別する。既存P0の範囲と優先順位を保ち、任意のfocus不変量への先指定を追加しない。有限cut・portal・全fiber合併の成果と一次文献比較は現行本文に保持する。全依存証明の包括的再監査・新規性確認は未完。組版・表示確認の状態は末尾を参照。

```sh
python3 scripts/research_check.py setup --require-tex
python3 scripts/research_check.py static
python3 scripts/research_check.py tex
```

環境要件・そのまま渡せる開始指示・必要な範囲の検証方法は [Cloud Codexの再開手順](research/cloud-codex.md)。通常の研究継続・コミット・mainへの保存は承諾を求めず行い、**切りのよいところで、長くても前回成功pushから約15分を目安に有効な現行成果を保存**しながら、方針の達成条件に沿って研究を進める。保存が必要でも未完成の証明を完成と記さず、他者変更を保持する。これらのファイルは再開・実行のための指示であり、Cloudサービス側の環境設定や新規タスク起動を自動的に行うものではない。

## 論文と役割

| 原稿 | 役割 | 組版の確認範囲 |
| --- | --- | ---: |
| [主原稿](papers/surface-lagrangian-torus-fibration.tex) | 相対SNC構成・次数分割・分岐底・作用適合atlas、actual KE全域GH実現と選択した中間尺度の成分錐とcore内の任意基点（改訂33） | LuaLaTeX組版済み、273頁、指定7頁表示確認 |
| [五次整数接着](papers/quintic-integer-gluing.tex) | 指定K5データの整数条件・高分母支持・未解決の大域接着 | 201頁 |
| [Meridian surgery](papers/meridian-surgery.tex) | 閉corner circuitsの局所置換の障害 | 18頁 |
| [TeX研究ノート](papers/research-notes.tex) | 証明素材・残る条件の整理 | 現行65頁、第1・4頁を表示確認 |

## 主な到達点と残る課題
指定hyperplane Kähler classでの正則Lagrangian \(T^2\) と、分岐辺上の \(S^1\times(S^1\vee S^1)\)、面内のpinched torus、core上のlogarithmic Weinstein skeletonを扱う。五次は(cores, branch edges, nodes)=(5,10,50)、六次は(6,30,90)で、分岐辺数は無限個のfiberの個数ではない。通常のalmost toric fibrationを超える特異模型を用いるため、Leung–Symingtonの分類と矛盾しない。全大域接着の公表前監査はなお必要。

五次整数アフィン接着では、四rayの完全matching条件等を証明し、高分母の必要支持候補を \(G_{5,14},G_{5,16},G_{5,17}\) の3型・26標識まで絞った。ただし26は実現数ではなく、一般分母の剛性・三高係数の同時非負性や全支持型の大域接着は未解決。

KE退化との関連では、全閉triple cornerのactual局所GH収束、定量的二段階平均、固定残余基底のactual neckとsourceのpinched torusを得ている。`ke:source-reduction-pinched-fiber` は固定点でのsmooth exact transportとprimitive消滅cycle、`ke:fixed-marked-tree-exhaustion` は全stage・全ての小さい複素parameterで一つの木を保つ選択を明示する。零momentの特異商を滑らかなsymplectic曲面とみなさず、parameter全体のtorus cycleのmonodromyを自明化しない。現行主稿の主要結果は次の通り。

- **同じnormal moment上の接続：** 固定source-free基底の残余点全体をactual長さ $O(1)$ で結ぶ。Moser像と、同じlevel上の複数fiberの合併も、正規化ambient径 $O(R_t^{-1})$ を持つ（`ke:fixed-base-moment-connectors`）。
- **三つの端の座標と作用：** 固定深度比で分離したarmで、射影neck座標との比の対数を全固定階で指数的に評価。積を保つsmooth補間で三端のnormal circlesを同時に合わせ、canonical normal periodの厳密な一致を示す。非正則な補間帯ではtame symplectic性を使う（`ke_neck_corner_transition.tex`）。
- **一つのcorner bundleへの統合：** 平均順序を比較するHamiltonianを $O(m^{-2})$ で評価してcutoffし、各端のnormal-first構成を相対統合する。単一moving armでは共通moment intervalを両端の漸近から構成し、actual reduced葉が小さいgraphとなることを示す。Collar外を固定して延長できる（`ke_relative_corner_patch.tex`）。第二periodの一致は自動でない。
- **有限cutの一様なcorner距離評価：** $m\ge m_*,\ R\ge R_*,\ \log(m+1)+4\log R\le R/8$ なら、内在・protected距離のdistortionは $C[m^{-1}+(\log(m+1)+\log R)/R]$。固定 $m$ の後に $t$ を小さくして使え、$m_t\to\infty,\ \log m_t=o(R_t)$ によりGH収束を得る。Fiberの非正規化内在径は $C/m$ 以下（`ke:slow-cut-closed-corner-gh`）。

- **全交わりで葉が一致する部分fibration：** 残余compact、normal cutoff、moment区間、parameter閾値の順に選び、全flowの共通開領域を構成する。Corner cut $m_t=6b_j$ とneckの葉でのtrim $B=7b_j$ を離して選び、first-exitと逆normal flowの自然性により、全intersectionが双方の全fibersで飽和することを証明した。Source・saddleの局所型を保って貼り合わせられる（`ke:neck-corner-saturated-union`）。
- **Central sourceのactual経路評価：** 固定rescalingでdensityは $L_t^{-2}$、canonical potentialは有界、normal momentは $O(L_t^{-1})$。Traceと平均二乗距離は $O(1)$、全中央点からgateへの退出は $O(L_t^{-1/2})$、oriented arm断面へは $O(1)$ で接続できる（`ke_source_connectors.tex`）。Source-freeな $|\mu|\le A/M_t$ のcentral band全体もactual径 $O(1)$。Source側では正のpotentialの対数勾配でactual球を深部に閉じ込め、complex SobolevのGaussian積分とBishop–Gromov比較から、固定点を含む中央coreの全点径 $O(1)$ を証明した。固定基底のsource-inclusive中央帯と閉pinched torus全体も正規化ambient径で収縮する。Potentialの一様square-root-Dini modulusを仮定する十分条件も示し、そのmodulus自体は未検証と区別する。
- **全momentのsource退出：** `ke:source-arm-uniform-tensor` は、三種類の境界でnormal covectorを制御し、source軸を含むoriented armの二側tensor比較を与える。固定normal座標での水平経路と動径補正により、`ke:source-all-moment-exit` の費用は全共通intervalで $O(1)$。中央固定点も短いgate退出と同じarm比較で扱えるため、この接続定理はGaussian可積分性に依存しない。同一momentの全fiber合併は固定基底で非正規化径が有界となる。

固定source chartのEuler場による明示的なresidual接続も保持する。成分coreではcanonical primitiveの差から固定領域のactual移送を構成し、境界を固定する相対flux条件とexactな平均化germを明示した（`ke_component_core_transfer.tex`）。`ke_component_core_geometry.tex` は任意固定compactと全collar上でKE形式・primitiveを保つsmooth正則化、正residueの有限型KE core、その小さい飽和近傍のmarked Lagrangian fillingを与える。全域への相対接着は下記四節で証明した。

**Actual KE形式上の全域接着：** `ke_component_link_cover.tex` で正residue periodを既存momentsと厳密に合わせ、閉linkと全特異層近傍の固定段階被覆を構成する。`ke_core_invariant_primitive.tex` はgeneratorのC1評価、exact scalar平均と全cutoff支持の被覆から、core外にtrappingを作らないadapted primitiveを得る。`ke_relative_reduced_foliations.tex` はsaddleを動かしてfull critical leavesを保つ。`ke_actual_core_gluing.tex` の `ke:actual-global-fibration` はLiouville cone fillingと全fiber単位のtrimにより、全 $X_t$ を覆うactual fibrationへ接着する。追加証明は別担当と内部点検済み。内側のprimitiveをcompact-relative Morse–Smaleに選び、index順の閉isotropic filtrationを得た。Skeletonの連結性は負時間像のnested intersectionから直接示す。各componentのcoreと変更collarは $C(1+\log(N_j+1))$ のactual ambient接続費用を持ち、十分遅い対角選択で正規化径が消える。

**指定collarの相対条件：** `ke:component-flux-space` は既知のCohen–Suciuの境界cohomologyを一般位置直線配置へ適用し、各componentの障害空間 $H^1(S;\mathbb R)/\operatorname{im}H^1(K;\mathbb R)$ の次元を $\binom{d-2}{2}$ とする。`ke:nonextendible-small-core-germ` は、同じactual形式を固定しても、恒等写像に任意に近いsymplectic collar germがcore全体へ延長できない例を与える。これは全域fibrationの不存在ではない。本構成は指定contact formを保つcone extensionと葉族の相対補間を用い、任意に先指定したcollar embeddingの延長を仮定しない（`ke:contact-rescaling-collar-scope`）。

**Core cutのtarget像：** 固定成分のstrictly plurisubharmonic potentialへ最大原理を使い、切り取った各coreの二つの独立深度を $CN_j$ 以下に抑えた。各capの旧softmax像は成分頂点の $\sqrt2\log(CN_j)/R_t$ 近傍に入る（`ke:removed-corner-target-cap`）。保持cornerには旧protected距離の評価が残り、旧corner内の経路は全曲面距離の上界に使える。旧softmax値と $p_T\pi_t$ の整合は次の構成で与える。

**全域基底の整合：** `ke:global-base-parameterization` により、全保持cornerで旧softmax値との誤差は $O((1+\log N_j)/R_t)$。正則torusを持つ旧辺をtriangleの少し内側へ送り、core panelsとneck stripsを明示的に貼り合わせる。潰される内部木には全枝共通のcanonical momentを使う。

**全域quotientとEuler予算：** `glue:closed-whole-fiber-quotient` は、有限閉piecesの全overlapが共通の全fibersで飽和することから閉同値関係とcompact Hausdorff quotientを与える。`topo:connected-preimages` と `topo:cubical-composite-connected` により、同じ $f_t=p_T\pi_t$ の全fibersも連結である。内部木上の合併は三次元部分を含み得るので、Lagrangian fibrationの主張は $\pi_t$ に属する。`inv:euler-pushforward` はfiber Euler関数の支持を有限個のnodesとcoresへ局在させ、`inv:cubical-fiber-euler` はcoarse fiberに入るnodeの重複度とcore寄与からそのEuler数を求める。Nodeの総数は $d\binom d2$ であり、各triangle/bigonへの配分は選んだ具体的recipeに依存する。

**全曲面の距離下界：** `ke:sharp-global-one-active` はsourceを含む正則normal frameに対する係数 $1+o(1)$ のscalar評価を与える。二active方向は既存full-triple比較で扱い、`ke:global-depth-lipschitz` で全曲線の長さを先に評価する。`ke:anchor-trimmed-neck-domain` で保持neckのmoment範囲を閉じ、`ke:same-moment-corner-reference` の同じmomentのcorner境界torusへ比較を移す。これにより `ke:global-depth-base-comparison` で同じ $f_t$ と一様に比較し、`ke:global-ambient-lower` を得る。経路の領域間往復回数を仮定しない。

**全曲面の距離上界とfiber合併：** `ke:global-ambient-upper` は、旧cornerの経路、全moment source退出、同じmomentのneck全体、各componentの対数費用と有限portal galleryを組み合わせる。Anchor interval外のneck尾部にも深度 $CN_j$ を証明し、残余基底の接続定数を先に選んで $1+\log(N_j+1)$ に吸収する。全接続予算は $H_{j,t}=C(1+\log(N_j+1))$、上界誤差は $C_d\{b_j^{-1}+(1+\log R_t+\log(N_j+1))/R_t\}$。このcut選択から最適収束速度は結論しない。`ke:collapsed-tree-full-fiber-collapse` は六次以上の内部木上の全fiber合併も評価する。各componentのcore径評価を、異なるcore全部の合併径やfiber内在径と取り違えない。これらを `ke:global-metric-realization` で同じ全射 $f_t=p_T\pi_t$ のdistortion消失へ統合した。`ke:eq:global-realization-explicit-cut-budget` は下界も合わせて、固定族の $C_d$ による $C_d\{\varepsilon_j+b_j^{-1}+K_j^{-2}+(1+\log R_t+\log\mathfrak m_j+\log K_j+\log(N_j+1))/R_t\}$ の一様評価を与える。Stageの定数はcutの下限とparameter閾値へ入り、これらの有効な成長率は未評価である。

公表前には、依存する既存証明と一次文献の包括的再点検、新規性確認、主稿の全体点検が必要である。確認済みの範囲は [検証状態](research/validation.json) に分けて記録する。

**SNCの固定collarとperiod障害：** `snc:reeb-leaf-kernel`、`snc:fixed-holonomy`、`snc:minimal-holonomy-controls` は、固定normal connection・coupling chartsの下でbasic formとexact cutoffによる相対接着が可能であることを、各成分の $g_a$ 個の独立な正則葉periodの消滅と同値にする。障害空間と必要なholonomy調整のrankはともに $\sum_a g_a$。全 $2g_a$ component periodsの消去は十分だが過剰である。Basic補正は全critical collarsの外に支持できるが、非零障害を消すconnection変更では一般に元のfull saddle collarsを動かす必要がある。Unitary holonomyの位相値だけの固定とconnection・normal gaugeの固定は異なる。既知のIKMの成分上の原理と、本稿の整数格子・SNC統合・couplingへの適用を区別する。詳細と一次資料は [研究ノート](research/notes.md#sncの固定coupling-chartsと葉のperiod障害) を参照。

**Normal actionと作用atlasの追加条件：** `neck:regular-period-matching` は、可縮な正則torus bandでの既定base同定に対し、独立第二作用が整数shear・符号・定数を除いて一致することをsymplectic matchingの必要十分条件とする。固定primitiveに関するexact matchingではその定数も零でなければならない。これは既知のaction-angle theoremの適用である。`ke:transition-residual-period` はcanonical frameのwindingによる残余period差を記録し、normal periodの一致から第二作用の原点まで一致とはしない。

**固定形式でもcritical actionは曲がる：** `atl:fixed-form-bent-branch` は、同じactual $\Omega$、normal action、両端・toric collars・saddle点のgerms、marked treeを保つLagrangian葉族でも、critical actionを非直線にできることを示す。`atl:critical-action-obstruction` により、二階微分が非零のbranch点には任意のdenominatorを許しても局所作用適合matroidal chartがない。既存の五次・六次atlas構成は、共通embedded marked classでcritical-region areasと切片を指定してこの障害を避ける。一般のLagrangian存在、P0のactual計量実現、選んだfibrationの作用atlasは別の主張である。

**七次以上のP0基底のcore障害：** `ke:global-core-nonmatroidal` は、$d\ge7$ の同じP0基底の各coreに、本稿の意味での局所作用適合matroidal chartが存在しないことを示す。Core linkの $b_1=\binom{d-2}{2}\ge10$ と三価matroidal linkの上限8による位相障害であり、同じcore・木系を保つ範囲の結論である。P0のactual Lagrangian性、同じ $p_T\pi_t$ によるGH実現と全fiber合併の収縮は維持される。別の基底や特異fiber型を許す全fibrationの不存在ではない。

**既存GH定理との比較：** Fernández de Bobadilla–Pełkaの [Theorem 6.14](https://arxiv.org/pdf/2312.13248v4) は、(b)で近傍fiberの余次元零部分のLagrangian fibrationを与え、(c)ではproperな族なら全nearby fiberについて補助Kähler計量のGH収束を与える。本稿との違いはGHが局所か全域かという一点ではなく、指定されたactual負KE形式での全域 $\pi_t$ と、同じ合成写像の全曲面ambient距離比較にある。形式のcohomology classの一致だけでは必要な計量制御は従わない。

**Focus近傍全体と作用の保存：** `ke:source-focus-transversality` は指定した写像 $(\mu,A(\mu,p))$ の非退化focus型を $d_pA(0,q)\ne0$ と判定する。`ke:focus-neighborhood-period` は一重pinched torusの小さい飽和近傍でnormal cycleが消え、残余cycle一つのperiodがclosed primitive差のexactnessを判定することを示す。Node primitiveを固定しても残余作用の原点は変えられるが、外側regular torusでも固定すれば差はexactとなる。`ke:focus-whole-neighborhood-transport` は構成したfibrationを全近傍で運び、通常のTaylor不変量 $S$ を保存し、exact transportなら追加定数 $S_0$ も保存する。これは既知の半大域不変量の本稿への適用であり、独立に指定したfocus模型の同値や、異なる $t$・stage間での不変量一定は主張しない。

**Nodal surgeryの面積と支持：** `glue:area-normalized-blowup` は例外曲線の実面積 $e$ を用いて指定複素blow-up上のradial Kähler形式を直接構成する。Chakravarthy–Gromanの比較写像は選んだ飽和affine-convex patchの外で恒等とし、球の外まで恒等とはしない。固定patch、容量を決める $\epsilon$、compact nodal neighborhoods全体、collarsとcuts、最後に $t$ の順に選ぶ。既知の相対surgeryをactual成分へ適用する証明であり、任意の独立primitiveの一致を付け加えない。

## 極限候補の有限距離幾何

座標部分複体への明示的な非伸長retractionにより、全targetの最短路を六つ以下のlabelへ還元できる。Closed-cornerの三枚のsquareは全targetに等長に埋め込まれ、portal比較のgallery数は五次30、六次以上60で足りる。

六次以上では **$\operatorname{diam}(\mathcal C_d,d_\square)=2\sqrt5$**。最大対は互いに素な三元supportのall-ones頂点対に限る。四つのsquare galleryによる上界と120三角形のPL calibrationによる下界を証明し、有限部分を有理数演算で独立検算した。この直径定理は既存の五次の値 $\sqrt{13}$ に依存しない。全域実現定理と合わせ、六次以上ではactual KE曲面の $R_t^{-1}\operatorname{diam}(X_t,g_t)\to2\sqrt5$ を得る。

## ビルドと再現

repo直下で `latexmk papers/surface-lagrangian-torus-fibration.tex`、`latexmk papers/quintic-integer-gluing.tex`、`latexmk papers/meridian-surgery.tex`。LuaLaTeX、LuaTeX-ja、日本語フォント、TikZを使用し、PDF/SyncTeXは `build/`。計算の入口は `python3 verification/run_current_checks.py`。ソースと証明書は `papers/sections/` と `verification/`。PDFはGitで追跡しない。

**曲面主稿改訂33の既存確認（2026-11-22）。** 今回の管理資料同期では曲面TeXを変更・再組版していない。中間尺度の成分錐の系を、target値が成分頂点へ一様に近づく領域の任意基点へ強め、同じP0のcore・変更collarへ適用した。新しい基点移動の証明と適用領域を独立に点検した。K2の全交わり・共通葉と、K3のlink・primitive・相対葉族・補間後trim・全域被覆の指定証明鎖を別担当が点検し、対象範囲で訂正すべきギャップは見つからなかった。P0に新しい解析仮定は加えていない。**改訂33をLuaLaTeXで組版し（273頁）、変更箇所を含む指定7頁を画像で表示確認した。未解決参照・引用、重複ラベル、欠落字形、overfullはない。** 実行範囲は [検証状態](research/validation.json) に記す。数学的点検・組版・保存は別々に扱う。整数検算suite・他論文・TeX研究ノートの再組版、形式証明、全主稿・全外部入力の包括的再監査、外部査読、網羅的新規性確認は今回未実施。
