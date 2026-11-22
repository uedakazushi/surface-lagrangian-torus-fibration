# KE–fibration 大域実現の依存関係

2026-11-23 / v3.30。目標・優先順位は [研究方針](../00_research_plan.md)、大域実現の定式化と結論は主原稿の `ke:global-realization-section` 節・定理 `ke:global-metric-realization` を正本とする。本書は外部入力の所在・適用範囲、本稿の直接評価による依存の接続、および確認範囲を保持する。

**現行の到達点（改訂53・公表準備）。** 各固定次数d≥5のactual負KE–Lagrangian射影による全域GH実現と、同じ射影へ運ぶ確率KE体積の極限に証明がある。五次のcompatibleな有限データに加え、六次では等重みw_i,j=2/5とsource配分(1,1,1,1;2)を用い、初期source葉を選んだ同じπ_tに全域作用atlas・GH実現・確率体積極限を持たせる（`ke:sextic-simultaneous-realization`）。六つの標準Petersen系のいずれも選べる。f_tの押出しは成分頂点、π_tの押出しはcore頂点の等重み原子測度へ弱収束する。全cubical距離と有限な測度の台、確率体積と未正規化のrescaled体積を区別する。任意先指定の大きいsource近傍、任意の異なるweights・focus不変量、atlasのparameter極限や極限計量のHessian性は結論しない。指定証明の独立内部点検と、全主稿再監査・外部査読・形式証明・包括的新規性確認を区別する。

**六次の有限条件から同時実現へ（改訂44）。** `ke:petersen-actual-neck-periods` はactual finite-t primitiveとwindingから、標準zero-external targetsのsource配分(1,1,1,1;2)、external切片ρ_i,k=ρ_j,k、内部切片ρ_i,j=ρ_j,iを導く。Row sum 4πからρ_i,j=4π/5、w_i,j=2/5が一意に定まる。`ke:petersen-two-end-cuts` の内部累積位置条件を、`ke:petersen-balanced-separator` と `ke:petersen-thin-source-block` の中間面積指定・Diniによる薄いblock・中央parameter-freezeで満たす。Full source annuliをその後で固定し、`ke:petersen-full-moment` が全moment targetsと両anchorの全open germsを実現する。`ke:sextic-simultaneous-realization` は同じdomain・primitive・moment・cutsと固定marked Tを使い、三面共通の平行移動付き整数アフィン接続からatlasを、相対値比較から同じπ_tのGHと確率体積極限を得る。各証明と接続は作成担当以外の読み手も対象を区切って点検した。任意に先固定した大きい内部source blockの位置障害は残り、その場合に同じ存在を主張しない。

## K0・K5の現在の点検範囲

改訂43の下記の証明本文を独立担当が実読し、統合担当がcompact core・cone filling・統合定理と主要一次箇所を照合した。対象内では追加仮定、量化の循環、修正を要する欠落を認めなかった。これは指定範囲の内部点検であり、形式証明・全主稿再監査・外部査読ではない。

| 証明鎖 | 確認した条件と要点 |
| --- | --- |
| `ke:compact-relative-morse-smale` → `ke:actual-limit-weinstein-core` → `ke:actual-link-cone-filling` | 小contact isotopyの明示liftで両端primitiveを厳密に固定し、compact exact Moserで同じ二形式へ戻す。閉trapping集合内のbroken trajectoriesから閉isotropic filtrationを得る。元のcontact form・全境界葉を保ち、有限退出・cone点連続性・skeleton連結性を直接示す。Whitney条件やfinite-volume endの正時間完備性は入力にしない。 |
| Meridian normalization → adapted primitive → relative reduced foliation → whole-fiber trim → `ke:actual-global-fibration` | Actual cycles上のresidue/winding、cutoff支持全体の共通作用とnontrapping、全critical葉の補間を確認。補間後のpartitionでtrimし、全開collarの同じ全fibersと有限閉quotientから全域被覆・連結性を得る。Saddle位置・第二action・critical値は固定しない。 |
| `ke:collapsed-tree-common-moment` → `ke:collapsed-tree-full-fiber-collapse` → `ke:coherent-corner-portals` | 内部木全体で厳密に同じmomentを用い、単独のπ-fiberではなく全f-fiber合併を評価。Support 1/2/3、端の小区間、閉anchor端点、μ=0を含む。固定residual domainsと接続定数をNより前に選ぶ。 |
| `topo:six-label-gallery` → `ke:global-ambient-upper` → `ke:global-metric-realization` | Square上の非伸長retractionと最短路の再訪排除からM_d≤60。旧full corner内のactual ambient接続とportal誤差を加算し、target線分へのexact liftを仮定しない。全固定stageの条件を最後のt閾値へ含める対角選択を確認。 |

一次比較では、CE §4A Lemma 4.1（刊行p.21）の正端は一定倍率までの固定であること、EM Definition 2.1/2.5とLemma 2.16/Remark 2.18（刊行pp.540–544）がcompletionとcontact rescalingを許すこと、Abbondandolo–Majer Introduction/Theorem 1がclosed manifoldを仮定することを照合した。本稿の両端厳密固定・compact domain・弱い閉filtrationは、それぞれの本文で直接証明する。BSV Prop.2.10の正のreal weightsと選択されたadapted primitive、TMZ Theorem 2.13のexact deformation・空間/parameter相対条件も、任意指定connection・core germ・full葉の保存と区別する。正確な一次URLと頁は後掲の各入力節が正本である。

K2全体とPart IVの全小摂動解析を一律に再監査したわけではない。六次のend-periodへの適用に必要な全phase・orbit/trajectory bufferは、次項の範囲で独立に点検した。既存の対象限定点検を保持し、残る公表作業では最小解析入力と実際の使用域、先行結果との同時達成範囲を照合する。K0のcone extension自体を主要新規性とせず、actual KE形式・既存の全葉・同じ全域射影・ambient距離の接続を貢献の中心とする。

## 六次同時実現の追加依存

| 接続 | 本文の正本と入力 |
| --- | --- |
| Actual有限periodと等重み | `ke:petersen-actual-neck-periods`、`ke:petersen-equal-weight-periods`。Canonical primitiveの閉差、row sum 4π、actual winding、A/B別framingから(1,1,1,1;2)とρ=4π/5を得る。旧central surgeryの正blow-up areaを代入した結論ではない。 |
| 全moment targetsと有限cuts | `ke:petersen-target-areas`、`ke:petersen-two-end-cuts`。`ng8:uniform-k2-end-periods`、actual source wall、Stokesから正targetsと内部累積面積の二端条件を得る。 |
| Source葉の初期選択 | `ke:petersen-balanced-separator`、`ke:petersen-thin-source-block`。三sourceずつの二領域Moser、薄いgraph近傍のDini、正margin後の中央freezeにより、full source annuliを凍結する前に全cutsを満たす。 |
| 全open接着と同時実現 | `ke:petersen-full-moment`、`ke:sextic-simultaneous-realization`。五領域relative Moser、anchor後選択、非零bandの端germ相対補正、A/B別starの同じaffine transition、`ke:relative-replacement-gh` と `ke:global-volume-measure` を用いる。 |

上の新証明は作成担当・統合担当・独立担当が対象を分担して実読した。正負のsource shear、closed primitive差へのclutching、separatorのwall、全momentのDini、中央freeze、marked product、全open germsと同じP0 cutsを確認した。既存K2全解析・全主稿の独立再認証、形式証明、外部査読ではない。次は既存の指定点検と重複しない最小解析入力・使用域および一次比較を照合する。

## 六次への K2 end-period 入力の点検範囲

`ng8:uniform-k2-end-periods` → `ke:petersen-target-areas` の適用を、Part IV v1.12 の `coarse:eq:simplex-log-gradient`・全深部tensor定理と、曲面の `ke:relative-corner-section`・`ke:neck-corner-saturated-union` の本文から独立に照合した。固定d≥5の全位相・全深度比の評価であり、六次は有限個のchartと整数基底の定数を変えるだけである。B=θb（5.4<θ<5.5）と7bは広いnormal-first plateau [5b,9b] 内にあり、retained cornerの6b cut内と取り違えない。全orbit・trajectoryのbuffer、同じprimitiveのcentered exact transport、source-free endのμ=0での滑らかさとStokesの2C/b面積評価を確認した。Residual stage→normal cut/common interval→N→t閾値→thin葉の順に循環は認めなかった。

これはend-periodに使う出力と接続の点検である。`coarse:cor:degree-d-volume-lower` の全境界下界供給、`coarse:lem:nested-metric`・`coarse:lem:small-volume-tensor` の内部解析、外部Schwarz/Savin/Schauder定理、source-normal-formと三arm座標補間の全証明は今回再証明していない。正確な実読labelと未点検範囲は `research/validation.json` の `k2_end_period_review` を参照する。次の解析監査は未点検の入力に絞り、確認済みのend-period chainを一律に反復しない。

## 公表に用いる最小解析核と新しい固定空間の帰結

Part IV v1.12の `coarse:thm:boundary-to-triple` はexact triple領域の全phase quotient、各固定tのradial閉包近傍でのsmooth負KE計量、固定faceの一様density下界を入力とする。Translated complete simplexのvolume squeezeとSavin小摂動評価で全深部C^q誤差O(1/m)を得る。`coarse:thm:full-triple-tensor` は固定次数の全平面退化への適用。局所kernelとcapped-volume鎖の指定監査を保持し、今回全証明を反復したとはしない。

Part IV v1.15の `simplex:prop:boundary-floor-sharpness` は、この局所仮定クラスでdepth coordinatesと比較模型k_Lを固定した場合のO(1/m)の最適性を与える。Expanded simplex族は同じ固定face下界と全phase・smooth閉包の条件を満たし、balanced点で厳密な誤差、正規化単体の境界へ近づく点で非零の一次項を持つ。命題全文とpure-model dominant-productへの非循環な依存を独立に点検した。Actual compact射影的族の誤差下界、facet shift補正後の最適性や全域GHの最適速度は結論せず、曲面P0の新たな解析入力にも加えない。導入の `intro:local-stability-scope` がこの範囲を引用する。確認保存版は末尾の表に置き、既存の解析入力pinとは区別する。

固定endの最小解析入力は `pair:prop:fixed-end-transfer` に分離した。固定collarのlog-densityのC¹収束と極限成分のradial derivative 4/s+O(s^(−1−δ))から、period 1のcanonical momentに±4π/s_r+O(s_r^(−1−δ))+o_(t;r,K)(1)を得る。固定K→小さい固定r→全小複素tの順と全phase一様性を保つ。`pair:rem:normal-frame-winding` は全orbitを含むpatchでΩ↦bΩとするとμ′=μ−2π wind(b)となることを示す。Zero windingでもprimitiveの残余閉periodは別に保持する。追加式・符号・Hermitian normの半径差を作成担当と独立担当が点検し、SongとRochon–Zhangの指定一次箇所を照合した。Moving内部のtensor/bufferはこの命題の結論に含めない。

Part I v1.9の `prop:compact-product-logarithmic-germ` は、尖点付き有限面積双曲曲線Sと閉コンパクト連結Riemann因子Yの積の実距離Laplace変換を、Re s<3の切断半平面上でW/(1−s)−H(s)Log(1−s)+G(s)と表示する。Hはentire、GはRe s<3で正則であり、`cor:compact-radial-recovery` はWとmonodromyからYの正規化基点距離分布を復元する。正次元のコンパクト負KE因子ではH(1)>0で、有理型延長はできない。通常volume-IRFA一般からの解析接続や等長型の回収は主張しない。Part IV v1.12の固定end最小入力とnormal winding、曲面改訂43の同じ射影の確率体積極限と合わせて総説v1.13へ統合した。曲面P0の新しい退化族仮定にはしない。証明・確認範囲・保存版は依存表を参照する。 内在的裾係数・compact基点一様性・gauge・moving/link・測度論の既存指定監査も、その有効な範囲で保持する。

本稿の証明入口は `ke:proof-inputs`、`ke:proof-route`、`ke:cut-selection-order`。五次の `ke:k4-actual-neck-periods` から全moment実現 `ng8:quintic-full-moment`、同時実現 `ke:quintic-simultaneous-realization` をたどる。Uniform K2 end periodsにはPart IVの全深部tensor/gradient評価とsurfaceのexact transportを使う。初期source葉を選ぶことで全tailのstrict cutsを満たす。六次は `ke:petersen-two-end-cuts` → `ke:petersen-balanced-separator` → `ke:petersen-thin-source-block` → `ke:petersen-full-moment` → `ke:sextic-simultaneous-realization` をたどる。追加先指定annuliは別途のstrict cutsが残る。

## 同じ射影へ運ぶ体積測度

`ke:global-volume-measure` はPart I `lem:CW`・`thm:facemass` と本稿の固定成分収束、`ke:global-depth-base-comparison`、既存のslow diagonalを用いる。各W_iの体積2π²(d−4)²の和がX_tの体積と一致し、固定compactのgraph像でf_t→e_iとなることから、確率体積をd個の頂点の等重み原子測度へ運ぶ。Song [Theorem 1.2(4), p.4](https://arxiv.org/pdf/1706.01518)の体積保存も一次資料で照合した。全dのπ_t版はp_Tの成分頂点逆像が一点であることによる。測度論の新しい族一様入力や量的速度は課さず、全cubical距離と有限な測度の台を分ける。

Pille–Schneider, [Hybrid convergence of Kähler–Einstein measures](https://doi.org/10.5802/aif.3455), AIF72(2)(2022), Theorems A–B pp.589–590、Remark2.4 p.605、Proposition3.1 p.607との一次比較を加えた。原子化と交点数の成分重みは既知であり、本族の確率重み1/dも一致する。本稿は同じactual射影上のGH近似と測度収束を示す。原典のhybrid中央fiberとcubical計量基底を同一視せず、Aの半安定還元仮定とBのnormal/reduced模型・特異集合へ質量を置かない複素弱収束の条件を区別する。規格化と正確な一次箇所は研究ノートおよび `ke:global-volume-scope` に置く。

### 有限cutoffの測度予算と局所bufferの定量化

固定側の `cor:CW-fixed-cutoff-budget` は、固定SNC対の T=log(1+Σq_i) に対するKE体積脱落とStokes defectをCe^{-A}で抑える。曲面の `ke:fixed-cutoff-volume-transport` は、同じf_tの押出しと等重み原子測度のW1距離を η_K(t)+D_d(δ_K+e_K(t)) で抑える。固定cutoffを先に選ぶことでδを制御し、その後で固定compact上の位置・体積誤差を小さくする。追加moving tensor仮定もtの有効率も含まない。両証明を作成担当以外も独立に実読した。

Part IV v1.13 `coarse:lem:localized-chern-lu` は正則写像のrank落ちを許し、actual半径2σの球からtr_gF*h≤C_nκ^{-1}(1+σ^{-2})を得る。`neck:cor:shrinking-buffer-circle` は0<σ_t≤1のactual bufferを仮定し、normal circle長≤C(1+σ_t^{-1})/m_tを与える。m_tσ_t→∞なら収縮し、径尺度ではR_tm_tσ_t→∞が十分。Bufferの存在・flow生存・full tensor比較はこの系の結論外であり、P0の既存buffer証明を置き換えない。局所cutoff・rank-one・体積上界の接続を統合担当も実読した。

### 有限標本の距離行列

同じ確率KE体積から独立に選んだ有限標本の距離行列は，異なるラベル間距離が2のd点等重み空間の標本行列へ分布収束する（`ke:random-ke-distance-matrix`）。二点距離は(1/d)δ_0+(1−1/d)δ_2で，平均は2(d−1)/d。これは既存GH・測度収束からの系で，追加解析入力を要しない。全cubical空間のGH極限と標本距離が観測する測度台を区別する。
証明正本は `papers/sections/paper/ke_global_metric_realization.tex` の `ke:random-ke-distance-matrix`。この新しい系にPart IVやPart Iの追加入力はなく，標本分布の極限を全cubical GH極限の代用としては扱わない。今回確認したのは頂点間距離の長さ下界，k重積測度とdistortionの接続，および一・二次momentの有界性であり，既存の全域GH証明の再監査ではない。

### 距離行列のWasserstein誤差と全域下界の指定監査

既存のGH distortion \(\epsilon_t\) と同じ射影の確率体積輸送 \(W_1((f_t)_*\nu_t,\nu_0)\) だけから、独立なk点の正規化距離行列の分布について \(W_1^{(\infty)}(\mathcal L_{t,k},\mathcal L_{0,k})\le\epsilon_t+kW_1((f_t)_*\nu_t,\nu_0)\) を証明した（`ke:random-ke-distance-transport`）。固定compactの予算では右辺を \(\epsilon_t+k[\eta_K+D_d(\delta_K+e_K)]\) と評価でき、二点距離が{0,2}の\(\rho\)-近傍外に出る確率も同じ輸送費用を\(\rho\)で割って抑えられる。k重結合の費用は\(\ell^\infty\)行列normで測り、固定されたkと族を対象とする。Moving tensorの追加入力も有効t速度も与えない。

正本は `ke_global_metric_realization.tex`。今回の大域距離入力点検は `ke:global-clipped-depth-map`、`ke:global-clipped-cogram-lower`、`ke:global-lower-rank-one-reduction`、`ke:global-depth-base-comparison`、`ke:point-to-corner-portal`、`ke:global-ambient-upper` の接続に限定した。二方向co-Gramの全phase・全深度入力そのものはPart IVに依存し、source-inclusive normal Schwarzの三境界補題、K2内部解析、全coreは今回独立再検証していない。従って原稿にある全域GH結論の包括的証明監査を完了したという主張にはしない。

### Source 深部の一様体積予算と相対coreの指定監査

`ke:source-uniform-deep-volume-tail` により、固定source tubeの深部体積V_t(S)は全ての小さいtに一様にC/S以下。さらに固定0<θ<1/4のS0≤S≤θLではcθ/S≤V_t(S)≤Cθ/Sと最良次数であり、S≥L/2+A_bではc_b L^{-2}exp(−(2S−L))≤V_t(S)≤C_b L^{-2}exp(−(2S−L))と中央指数領域まで二側比較する。既存capped体積上下界のみを積分し、新しいmoving tensor仮定は不要。全neck・全曲面の体積裾、距離径や有効GH速度を導くものではない。

正本は `papers/sections/paper/ke_source_potential_buffer.tex`。密度上下界を中心sourceへ導く `ke:source-tube-potential` はPart IV `coarse:cor:degree-d-volume-lower` と `coarse:lem:complete-volume-upper` に依存する。追加したC/S尾部はこの密度の上界のみを積分するため、source-arm tensor、中央Gaussian、全moment退出、core貼合せ及びCP/PBE/TCを仮定しない。既存の全点source退出は `ke:positive-poisson-log-gradient` → `ke:source-arm-scale-buffer` → `ke:source-arm-uniform-tensor` → `ke:source-all-moment-exit` を必要とする。Coreのconical extensionはEvans--Mauri Lemma 2.16/Remark 2.18を踏まえつつ，元のactual link contact formの保持とwhole-fiber trimを本稿で別に証明する。今回はsource/coreの指定鎖を対象限定で読み，外部の全解析定理の仮定・K2全証明・全coreの包括的再認証は実施していない。

### Capped入力の最適性とactual source体積

**Capped前因子はactual KE体積についても鋭い。** Part IV v1.16 の `coarse:prop:capped-prefactor-sharp` が同じbarrierの指数2の最大性を証明し、曲面主稿 `ke:source-capped-actual-prefactor-sharp` はさらに `ke:source-central-density` を用いて、実際のω_t²≥cΩ_t,d^(β)がt一様に全X_tで成立する必要十分条件はβ≤2と証明する。β>2では固定単純sourceの中央点p_tでω_t²/Ω^(β)≈L_t^(2−β)→0。これは既定のα_iとcanonical densityを固定したときの結論であり、別の障壁構成やGH速度の普遍的限界ではない。

Part IV v1.16は `coarse:prop:capped-prefactor-sharp` のbarrierに関する証明の正本。本稿は `ke:source-central-density` を加え，actual `ω_t²` の同じ前因子最適性を証明した。利用するsource中央で `xy=tz`，`(x,y,z)=(τX,τY,XY)`，`α_x,α_y≈L_t`，`Ω_{0,t}≈|dX∧dY|²` を明記する。既存 `coarse:cor:degree-d-volume-lower` の入力仮定を変更しない。

**Source深度の臨界moment。** `ke:source-depth-critical-moments` は固定source tubeの二側質量裾から、m=min(s_x,s_y)≥S0の領域上の実際のKE体積moment ∫m^γ dV が、0<γ<1では定数次数、γ=1ではlog L_t、γ>1ではL_t^(γ−1)であることを証明する。層別積分 M_γ=S0^γ V(S0)+γ∫S^(γ−1)V(S)dS と、通常armのV≈1/S、中央側のV≈L_t^(−2)e^(−(2S−L_t))を組み合わせる。これはmoving sourceの重み付き体積の臨界指数1を与えるが、全曲面のmomentや有効なGH速度への外挿はしない。

**Savin H2に関する現行照合。** Part IV v1.17 の `coarse:lem:small-volume-tensor` において、実対称4×4の半正定値増分PをHermitian 2×2のℋ(P)へ写す際にtr_C ℋ(P)=tr_R P/4が成り立つ。固定モデルHの楕円性とdetの微分からSavin Theorem 1.3のH2を実operator normで確認した。H1とH4も同定理の仮定に一致する。これにはactual tensor comparisonを先に仮定せず、modelのnormalized cover上の一様boundsを先に確保する必要がある。Part IVで証明を所有し、曲面の `ke:global-realization` への入力は既存 `coarse:thm:full-triple-tensor` として変わらない。今回の確認は指定H1/H2/H4・線形化の適用範囲であり、全曲面の全K2/source/Weinstein証明を再監査した意味ではない。

## 三研究の責任範囲と依存の方向

三repoは一つの計画として編集・監査するが、証明の正本は分担する。固定SNC・配置補空間のPart I–IIIは `multiscale-kaehler-einstein`、退化族の局所一様解析Part IVとCP/PBE付き大域枠組Part Vは `kaehler-einstein-degeneration`、actual KE–Lagrangian構成と同じ写像の直接大域GH実現は本repoに置く。シリーズ総説はmultiscale側、詳しい利用関係は本書、研究全体の短い見通しはhubが正本である。外部結果の訂正は利用側へ反映し、証明を二重掲載しない。

| 対象・尺度 | 正本の結果 | 本稿への接続と限界 |
| --- | --- | --- |
| 固定 $U_i=H_i\setminus\bigcup_{k\ne i}(H_i\cap H_k)$、空間的blow-down | Part I `cor:arrangement-cone`、`thm:contract`、`cor:based-ball-approximation`、$(n,m)=(2,d-1)$ | $K_{H_i}+D_i=(d-4)H$、unit orthant錐 $C_{2,d-1}$。固定した全射 $\mathcal S_i$ と $K_i$ に対し、中心 $o$ のscaled閉球と中心 $R^{-1}\mathcal S_i(o)$ の錐の閉球のGH距離は $3K_i/(2R)$ 以下で、中心・半径に一様。本稿 `topo:component-cone-germ` は $\mathcal C_d$ の $e_i$ での接錐と等長同定する。固定空間の評価から $t$ 族のmoving領域一様性を推論しない。 |
| 固定compact base・固定endの後に $t\to0$ | IV `pair:prop:fixed-end-transfer`、`pair:thm:fixed-end-moment`、`pair:lem:diagonal-fixed-end` | 各stageの有限データ・誤差・予算を先に固定する遅い対角列。Moser buffer、moving neckのtensor比較、sourceの全moment退出、scalar下界は本稿で別に証明する。 |
| Actual $X_t$、距離 $R_t^{-1}d_{g_t}$ | 本稿 `ke:global-metric-realization` | IVのcapped density・full-triple・fixed compact入力から、scalar/portal経路で同じ $f_t$ の全域distortionを得る。外部CP/PBE/TCの検証ではない。 |
| 選択した $1\ll a_t\ll R_t$ | 本稿 `ke:intermediate-component-cone` | $R_t(\operatorname{dis}(f_t)+\eta_t)=o(a_t)$、$\eta_t=\sup_{A_t}d_\square(f_t(y),e_i)\to0$ の下で任意の基点 $y_t\in A_t$ から $C_{2,d-1}$ へ一様なpointed GH収束。同じP0の一成分core・変更collarへ適用できる。前行と局所錐同定の帰結であり、任意の中間尺度や極限交換は主張しない。 |
| 標識付き残余複素曲線とsource | Part IIのsecondary period、Part IIIのconifold模型 | 二重線の残余曲線は $\mathbb P^1$ minus $d-2$ triple points。$F_d$ のsource zerosは追加データ。複素・双曲periodを第二作用と同一視せず、Part IIIのH_loc/H_ancを本稿から無条件に解決済みとしない。 |

上表の中間尺度の帰結の証明は本稿のみを使い、Part Iの全域path liftingをP0の新しい解析入力として加えない。Part Iの漸近錐との比較は、固定空間側の原稿にある定理との同定である。

Part II `prop:partI-translation` は $n\ge2$ の非空faceからの移動極限を扱い、$n=1$ は別の恒等的な場合とする。`thm:intro-star`・`thm:star-chart` では、factor/cusp labelsを完全に保持したcurve factorsとKähler orientationから配置を復元する。`thm:intro-unoriented`・`thm:unoriented` は全curve factorsを用い、factor/cusp labelsを保って向きだけを忘れるgeneric結果であり、projective equivalenceと全体複素共役までの復元である。裸のmetric limitからlabelsが自動的に回復されるとはしない。本稿の第二作用periodとの同一視や、同じ $\pi_t$ による作用atlasとP0の同時実現へは使わない。ここで同期したのは定理文・data・量化の照合であり、Part IIの全証明の独立再監査ではない。

### Sourceを含む固定shellへの接続

`ke:source-inclusive-fixed-shell` は、sourceを含む固定残余compactで同一の正則体積frameを保ち、固定endのmoment $\pm4\pi/(-\log r^2)$ とshell横断費用を証明する。先にcompactと $r$、最後に全ての小さい複素 $t$ を選ぶ。Songの固定smooth locus収束とRochon–Zhangのcusp展開の一次資料を確認した。異なる正規形のprimitiveの一致やresidual period消滅は追加しない。`ke:global-clipped-cogram-lower` は固定parameterの有限評価へ定式化を改め、誤差消失は統合定理の最後の対角選択でのみ用いる。上下界・Part IV入力の指定証明鎖に循環やprotected距離のambient距離への無条件な置換は認めなかった。全主稿・全外部結果の包括的再監査ではない。

## 確認した正本と規格化

[multiscale-kaehler-einstein](https://github.com/uedakazushi/multiscale-kaehler-einstein) の確認済み数学本文はPart I v1.10・Part II v2.1、総説v1.14、研究資料v1.19である。固定cutoffの脱落体積・Stokes defectの新系を複数担当で実読した。保存版は `2926300c2425c7e68550ac08ee81a2afa639a0c6`。 Part Iの `def:clean`, `lem:fibres`, `prop:lifting`, `cor:upper`, `app:lifting` におけるambient endpoint接続と、`cor:arrangement-cone` の規格化を照合した。固定Hermitian depthsを保つ `lem:SNC-compatible-collars`、Rochon–Zhangの延長とcollar pullbackの全残余一様な比較 `lem:fc-collar-transfer`、背景形も含める `lem:RZ-collar-tensor` の三補題を独立内部点検した。一般log-smooth collarや残余normを保存しない射影の障害は `rem:log-collar-obstruction` に保持する。

計量側の対象限定点検は `prop:cogram`→`thm:contract`→`thm:rough` のrow estimate・全射性・距離比較と、`cor:based-ball-approximation` の中心・半径に一様な閉球評価を含む。これは `cor:GH` と `thm:moving` に適用できる。指定compactを零へ送る場合、加法定数はそのcompactに依存してよい。

`def:incidence-link` と `lem:positive-star-product` はcofaceのincidence copiesを保持し、正の面座標を持つ領域だけを積と同定する。`lem:star-ball-isometry` は $m_\alpha=\min_{i\in\alpha}\sqrt{c_i}a_i>2A$ の下で、半径 $A$ のambient閉球の厳密な積表示を与える。閉star全体のambient距離を積とする主張は使わない。`prop:cone-limits` と `cor:moving-limit-classification` は全てのmoving-basepoint limitsを有限位置の錐、または $(\mathbb R^{|\alpha|}_{\boldsymbol c}\times\mathcal L_\alpha,(0,z))$ に分類し、任意のscaling sequenceで各型を実現する。曲面側では定理文と構成を確認し、指定証明を担当・主担当が点検した結果を同期した。

`lem:cone-link-metric`・`prop:link`・`rem:link-metric-scope` は曲面側担当も独立に点検した。非連結linkでは成分間の長さ距離を $+\infty$ とし、$\pi$ で切り詰めた角距離によるcone公式と、そのpath metricによる長さ距離の回復を用いる。Coarse section誤差 $A_s$ に対する $(K+2A_s)/r$ は全方向に一様である。Pointed cone isometryが保つmetric linkの等長型の主張であり、named labels・cell decomposition・重み $c_i$・genuine geodesic-ray boundaryの回収は含まない。全rough raysのbounded-distance商をlinkと同定することもない。

測度側では `lem:deep-sector-partition`, `lem:cellwise-LDP`, `lem:exp-tight`, `thm:LDP` のambient open集合に対する下界・上界を点検した。Busemannからtailへの鎖は、一面のLipschitz potential、全faceのconditional moments、直接の指数積分を用い、LDP下界やcontracting mapの距離下界に依存しない。角度分布の分母は最小減衰率のcuspの重みの和であり、`thm:joint` と `cor:Laplace` への極限の順序も確認対象に含む。主稿Introductionの仮定依存表と照合した現行の主要条件・担当ごとの点検範囲は次のとおりである。純測度のsector/cutoff選択はclean collarsとvolume moduliだけを使い、co-Gramの定数を入力しない。

| 正本の結果 | 仮定・結論と確認範囲 |
| --- | --- |
| `thm:intro-measure`、`thm:LDP` | 非零有限測度と全faceで整合するordinary volume-IRFAを用い、各leading残余測度は非零finite/full-supportとする。収縮写像によるLDPにはmetric-IRFAを加え、測度は $\mu/\mu(X)$ に正規化する。KEのface translation・面質量は非正規化 $\mu=dV_g$ を用いる。確率測度のface massは表示した交点数係数を $\mu(X)$ で割った値である。各face massの総和が1になるという意味ではない。主定理と本文の対応を曲面側担当が直接点検した。 |
| `thm:translation`、`eq:translation-TV-strip`、`eq:translation-TV-ball` | 非空normal集合とconnected faceを固定し、$\mu_F=\chi_F\mu$ を $\Pi_T=(t_I-T,\pi_F)$ で押し出す。Ordinary volume-IRFAで任意の $\min_iT_i\to\infty$ に対するfixed strip×全residual spaceのTVを得る。Metric-IRFAと有限のcentered offsets・residual基点の収束を加えると、計量を追加rescaleせずambient閉球のTVとpmGHを得る。Normal phasesの収束やsmooth volume-IRFAは不要。定理文・依存仮定を直接照合し、既存の全証明点検は共同結果として保持する。 |
| `lem:CW`、`thm:facemass`、`app:CW` | 滑らかな基準曲率 $\Theta$ と有界primitive $\beta$ による $\omega-\Theta=d\beta$、有限Poincaré体積と勾配一様有界cutoffで直接Stokesを証明する。$[\Theta/(2\pi)]=c_1(L)$、$dV_g=\omega^m/m!$、Part Iのnormal角度座標の周期 $2\pi$、残余adjunctionを曲面側担当が直接点検した。一般good metricとのbounded potential、exact tail、Mumfordのsingular Chern–Weil theoremを主証明の入力にしない。 |
| `lem:Mellin-conditional-moments`、`lem:Mellin-weighted-TV`、`thm:Mellin-recursion` | 全faceのordinary volume-IRFAとcompatible full collarsからactual conditional residual measuresの一様subcritical momentsとweighted全変動収束を導く。一般Borel densityではnormal depthsに関するessential supremumで述べ、smooth densityでは通常のsupremumでよい。Recursionは固定compact subcritical parameter set上で一様であり、選んだ $b_F$ のweighted可積分性を追加仮定しない。共同点検結果の同期であり、曲面側担当による全証明の独立再監査ではない。 |
| `lem:vertex-tightness`、`thm:tail`、`thm:joint`、`cor:Laplace` | 非空境界と固定基点を仮定し、metric-IRFAと全faceのordinary volume-IRFAを用いる。Actual conditional momentsから残余shellを抑え、volume errorのexponential decayは追加しない。一般weightsでは最小entropyのcuspsだけを混合し、KEでは全entropyが1となる。Boundaryが空のcompact場合にはtailはeventually 0であり、この非自明な臨界公式は適用しない。強化した証明は共同点検結果、Introとの条件照合は曲面側の直接点検である。 |
| `prop:Mellin-incidence` | Component別cutoffを含むmixed transformの係数 $\operatorname{ARes}_J\mathscr M_{F\mid G}=\mathfrak m_G\mathbf1_{\{G\subset F\}}$ からcomponent incidenceを回収する。単独のface mass数値列からの回収ではない。Full polyhomogeneityやmeromorphic continuationもordinary volume-IRFAだけからは主張しない。 |
| `thm:Mellin`、`rem:Mellin-continuation`、`ex:Abel-not-meromorphic` | Ordinary volume-IRFAは一側Abel極限を与える。深さ1の抽象測度の $1/t$ 誤差は、Abel係数1と非有界な対数remainderを持つため、臨界点をmeromorphicに越えない。有理型延長には全角・残余変数での $L^1$ coefficient/remainder評価を伴うjoint polyhomogeneityを別途仮定する。追加例と主定理のscopeを曲面側担当も独立に確認した。 |

`lem:hyperbolic-curve-tail` は尖点を持つ有限面積双曲曲線の基点liftの最大高さを用い、角一様O(v^−2)距離誤差からA(p)e^−R+O(e^−3R)を得る。`ex:KE-product-distance-log` の実球二次項はC=A(p)∫_Y d_Y²dV_Y/2>0である。`prop:compact-product-logarithmic-germ` はこの裾誤差をStieltjes部分積分でRe s<3の正則項へ分離し、厳密な積距離のkernelからentireな対数係数Hを求める。誤差の微分評価を追加せず、級数の一様絶対収束を証明する。`cor:compact-radial-recovery` は全偶数momentsとコンパクト台の一意性から基点距離分布を復元する。研究ノートの非等長な球面変形は、一般Riemann因子では変換全体の一致も等長型を決めないことを示す。負KEクラスの剛性反例とはしない。作成担当・統合担当・独立担当が本文の式・正則領域・monodromy符号・復元係数を照合した。DLMFの指数積分/Bessel公式は古典的なものとして引用し、Golubev–Kamberの距離集中、CLTのheight sublevel、Grieserのpolyhomogeneous Mellinとのobservableと漸近領域の違いを一次資料で確認した。網羅的な新規性判定は未了。

Chern–Weil適用で直接確認した一次資料は [Rochon–Zhang, arXiv:1106.0873v2](https://arxiv.org/pdf/1106.0873v2) の (2.26)–(2.30), p.15（bounded-derivative空間）、Definition 2.10, p.22（法方向の規格化）、(5.1)–(5.9), pp.38–39（背景形・KE potential・adjunction・残余解）、Lemma 5.2の証明冒頭, p.40（背景Hermitian metric）である。(5.3)の符号はPDF画像でも確認した。$u\in C^\infty_{\rm fc}$ は (5.6)直後の存在入力であり、その有界微分にはTheorem 5.1を必要としない。Mumfordのgood-metric theoremは比較参照に留め、今回は著者PDFの検索indexで定義・Theorem 1.4のstatementを確認した範囲に限る。PDF本体の取得はtimeout/HTTPエラーで未完了であり、その証明全文を確認済みとはしない。

Part I v1.10は73頁にLuaLaTeX/latexmkで組版し、1・36–38・73頁の5頁を150dpiで実表示した。主要log六分類は全て0。これは固定補空間側の作成担当が行った現在の検証であり、曲面側の再組版や全頁検査ではない。内容不変の総説v1.14の既存22頁の組版・表示記録、Part II–IIIと研究素材の記録はその正本に保持し、今回は再実行していない。

先行研究の比較では、[Chambert-Loir–Tschinkel, Igusa integrals and volume asymptotics in analytic and adelic geometry](https://www.numdam.org/item/CML_2010__2_3_351_0/)（Confluentes Math. 2 (2010), 351–429）の §§2.1.12–13、§3.1.3、Propositions 4.2–4.3、Theorem 4.7、Corollary 4.8を文献担当が一次本文で確認した。Adjunctionによるresidue measures、componentを記録するClemens complex、Igusa主要係数とheight-ball測度漸近は既存の枠組みである。Part Iのordinary recursive L1漸近によるAbel係数、対数深さ、actual距離球のBusemann phaseとの接続と区別する。Height ballsをactual距離球と同一視せず、一般原理の新規性を主張しない。本担当は指定一次比較の報告を同期し、原著の全証明を再監査したとはしない。

上記の距離・測度証明はPart I、標識付きperiodの証明はPart IIのみを正本とする。対象限定監査を全Part I–III・全一次文献の包括的再監査や退化parameterに一様な評価と混同しない。本稿のP0と中間尺度の証明に、これらの大域錐・moving分類・link復元・LDP・tail・translation・面質量・Mellinを新しい解析入力として加えない。退化族の一様性や任意の中間尺度、同じ射影によるatlasとP0の同時実現も、この固定空間の結果からは得られない。

関連する [kaehler-einstein-degeneration](https://github.com/uedakazushi/kaehler-einstein-degeneration) の確認本文はPart IV v1.15・V v1.10、研究資料v1.28。新しい局所率の確認保存版は `1ee0acaf876b1334c964d60c409feb3b18b62373`。以下のIVは `papers/kaehler-einstein-degeneration.tex`、Vは `papers/cubical-gh-limit.tex`。`simplex:prop:boundary-floor-sharpness` の仮定適合、balanced点の厳密なscaling、境界へ近づく例の一次係数とpure-model入力への非循環な依存を独立に点検した。固定depth coordinates/reference k_Lの局所仮定クラスに限定し、compact射影的族やfacet shift補正後の最適性へは広げない。既存の `coarse:lem:simplex-model` の最小外部入力、一意性、tube/格子商の完備性、scalingとperiod、Ricci/volume係数、全深度の正規化についての指定点検は、確認版 `2bf17973cb2e2ecbb6b835ca7f77592cf6cf0664` の範囲を保持する。Zhang Theorem 2.1は直接実読し、CY1982原典Theorem 4.4の本文は未取得として区別する。既存capped density・full-triple/Savin・Schwarz半径・fixed-end/windingは一律に反復しない。正本の担当者がIVを126頁に組版し、1–2・7–9・60–62・125頁の9頁を150dpiで実表示した検証記録を照合した。主要log六分類0。V本文と既存37頁/指定5頁の記録は不変で再組版していない。IV/V本文の曲面科学入力pin改訂37も維持する。

外部入力について確認したのは、該当する定理文・証明の所在・依存仮定・規格化と、本稿の接続に必要な証明箇所である。下表の「証明あり」は原稿の状態を表し、全旧証明の独立再監査・形式証明・全一次文献の再精読を意味しない。今回の組版・指定頁の表示確認は上記のとおり別に行った。現行証明では上記mainを再取得し、full-triple比較、`simplex:lem:rank-one-schwarz`、`simplex:prop:dominant-product`、`simplex:cor:active-cogram`、`pair:thm:fixed-end-moment` と関連するvolume入力の定理文・必要な証明・規格化を照合した。本稿に必要な証明と大域接続の内部点検範囲は末尾に記す。

IV の `ass:Gd` は、一般位置の $d$ 平面、非零小parameterでの滑らかさ、各二重線上の $F_d$ の相異なる $d$ 個の単純零点、全三重点での $F_d\ne0$ を仮定する。各固定 $d\ge5$ と固定族を扱い、次数や族全体に一様な定数を要求しない。

\[
X_t=\{\textstyle\prod_{i=1}^{d}L_i+tF_d=0\},\quad
\operatorname{Ric}(\omega_t)=-\omega_t,\quad
[\omega_t]=2\pi(d-4)H,\quad
L_t=-\log|t|^2,\quad R_t=\log L_t.
\]

距離は $\bar d_t=R_t^{-1}d_{g_t}$、Riemannian metric は $R_t^{-2}g_t$。標的は

\[
\mathcal C_d=\{w\in[0,1]^d:\max_iw_i=1,\ |\operatorname{supp}w|\le3\}
\]

の各unit squareをEuclidean距離で貼った**複体全体の内在長さ距離** $d_\square$ である（IV `eq:degree-d-normalization`, `eq:Cd-definition`）。Primitive class $2\pi H$ に再規格化すると距離が $1/\sqrt{d-4}$ 倍になる。一般のhyperplane classでのfibrationをactual KE formへMoser移送する際、その移送の計量的制御は別の入力である。

## 現行の結論と外部仮定の扱い

定理 `ke:global-metric-realization` は、上の一般性条件を満たす任意の固定 $d\ge5$ について、actual $\omega_t$ に関する連結fiberの連続全射 $\pi_t:X_t\to B_d(T)$ と、同じ $f_t=p_T\pi_t$ に対する

\[
\sup_{x,y\in X_t}
\left|R_t^{-1}d_{g_t}(x,y)-d_\square(f_t(x),f_t(y))\right|\longrightarrow0
\]

を与える。正則fiberはLagrangian $T^2$、source・branch・coreの特異fiberは本稿の相対構成による。左辺は全曲面の任意の経路を許すambient距離である。$d\ge6$ で $p_T$ が潰す内部木上の全fiber合併も一様に収縮する。木系の組合せ型は固定するが、critical values・collar・基底parameter化と遅い段階選択は $t$ に依存してよい。

この結論は `ke:actual-global-fibration`、`ke:global-base-parameterization`、`ke:global-ambient-lower`、`ke:global-ambient-upper` を同じ写像で組み合わせたものである。**外部のCP/PBE/TCは未検証のままであり、本稿がそれらの全packageを証明したとは主張しない。** 本稿では、sourceを含むsharp scalar normal評価と全域clipped logarithmic mapによる下界、共通momentの接続と有限galleryによる上界で、P0に十分な距離評価を直接証明する。最適収束速度、次数一様性、任意に先指定されたcritical valuesの実現は含まない。

### 一般存在・P0・作用atlasの量化

`main:global` は任意のmarked pants treesを指定した固定形式上の存在定理である。P0は固定した次数・退化族から一つの許容木系 $T$ を選び、その後の全stageと全ての十分小さい複素parameterに共通に使う。定数は固定した次数・族・補助データに依存し、$t$ に関するfibration族の滑らかさ、任意指定 $T$、任意速度の対角化は結論しない。$R_t^{-2}g_t$ はtensorの規格化、$R_t^{-1}d_{g_t}$ は距離の規格化であり、径一の極限は $D_d^{-1}d_\square$ である。

`main:action-atlas` の $d=5,6$ の一般symplectic存在とP0は量化が異なる。五次の `ke:quintic-simultaneous-realization` は、compatibleな正weights・四角形系・source配分と初期source葉の選択により、同じactual $\pi_t$ の全域atlas/GHを構成する。等重みの対称六系から無条件な存在例を得る（対象退化族の既存一般性条件の下）。六次では `ke:petersen-full-moment` と `ke:sextic-simultaneous-realization` が等重みw_i,j=2/5・初期source葉選択の下で同じ射影のatlas/GH/測度を構成する。$d\ge7$ の `ke:global-core-nonmatroidal` は同じP0基底のcore linkの $b_1=\binom{d-2}{2}>8$ による位相障害で、異なる基底も許す全fibrationの不存在ではない。

## 既存GH結果との一次資料比較

| 一次資料・確認位置 | 既知の結論と本稿で別に証明する内容 |
| --- | --- |
| Fernández de Bobadilla–Pełka, [arXiv:2312.13248v4](https://arxiv.org/pdf/2312.13248v4), Proposition 5.6 p.24、Proposition 6.13 p.30、Theorem 6.14 p.31、Remark 7.4 p.34；CPAM (2026), e70060, [DOI](https://doi.org/10.1002/cpa.70060) | 6.14(b)は補助形式 $\omega_q^\varepsilon$ に対する余次元零部分のfibration。(c)はproperなら全nearby fiberと残余領域のpairのGH収束であり、部分領域だけのGHではない。補助計量を径で再規格化する。Actual負KE計量や全域Lagrangian core fillingをそのまま与える結果とは区別する。同じclassのMoser同定から距離制御は自動ではない。 |
| Fu–Hein–Jiang, GAFA 35 (2025), 542–632, [掲載版PDF](https://link.springer.com/content/pdf/10.1007/s00039-025-00708-y.pdf), §1.1 pp.543–544、Main Theorem p.544 | 孤立楕円特異点を持つ明示六次族のactual負KE計量を扱い、$\lvert\log\lvert\sigma\rvert\rvert^{3/2}$ のtensor再尺度でTian–Yau bubbleを得る。全平面SNC退化の $R_t^{-1}$ 距離によるcubical極限と、同じLagrangian射影への適合とは退化模型・尺度・結論が異なる。 |
| Y. Zhang, MRL 22 (2015), 1843–1869, [arXiv:1505.04728v2](https://arxiv.org/pdf/1505.04728v2), Theorem 1.1 p.3、Theorem 2.4 p.8、Theorem 2.6 p.10 | Q-factorial simple toroidal canonically polarized degenerationで、動く基点による元のKE尺度のpointed collapseと、最大退化点の局所semi-flat比較を与える。2.6は追加の非消失volume form条件下のgeneralized special Lagrangian torusの存在。本稿のsource全空間 $xy=tz$ とsmall resolution後のrelative ample性はそのまま仮定を満たさず、全曲面の径尺度・同じ射影の比較は別に証明する。 |
| J. Song, [arXiv:1706.01518v1](https://arxiv.org/pdf/1706.01518v1), Theorem 1.2 p.4 | Stable degenerationの元の負KE尺度で、成分内部に基点を取る非崩壊極限を与える。本全平面族では各 $\mathbb P^2$ から $d-1$ 本の直線を除いた完備KE成分であり、径尺度のcubical極限やLagrangian射影を与える定理とは区別する。 |

ここでの確認は指定定理・規格化・適用範囲の一次照合であり、各論文の全証明の再検証や網羅的新規性確認ではない。

## 外部解析入力の状態

| 入力 | 正本・ラベル | 適用範囲と残る条件 |
| --- | --- | --- |
| 全次数のcapped volume下界 | IV `coarse:cor:degree-d-volume-lower` | 固定 $d\ge5$、`ass:Gd` の下で証明あり。体積比からtensor二側比較を推論しない。 |
| Sourceのoriented volume比較 | IV `coarse:lem:pair-arm-density`, `coarse:lem:complete-volume-upper` | $xy=tz$ の正しいorientationのannulus–disc上で用いる。一般のcomplete域では対数体積比の上有界性を明示的に仮定する。本稿の有限annulus–discでは固定 $t$ のcompact closureへの延長とmodel densityの境界発散で確認できる。中央gateからvolume上界だけを中央へ延長し、中央のtensor比較は入力にしない。 |
| 全深部tripleのactual/model比較 | `full_triple_comparison.tex`, `coarse:thm:full-triple-tensor` | $m_1\le m<L_t/3$、$\min\ell_i\ge m$ で全phase・全深度比に $C^q$ 誤差 $O_d(m^{-1})$。追加のTC/PBE仮定を用いない。Source・pair全域の結論ではない。 |
| 係数1・境界の積漸近 | `simplex_boundary_geometry.tex`, `simplex:lem:rank-one-schwarz`, `simplex:prop:dominant-product`, `simplex:cor:active-cogram` | Complete simplex模型とそのactual tripleへの適用。三重点の外の全raw-active領域へ拡張した結果ではない。 |
| 閉cornerの距離評価 | `closed_triple_metric.tex`, `simplex:thm:closed-corner-model`, `simplex:cor:actual-closed-corner-metric` | 同一tripleの三枚のsquare自身の距離（本repo `topo:coordinate-retraction` により全target距離の制限と等しい）。Sourceの内在距離と保護領域内の経路について $O(\log R_t/R_t)$。この局所結果だけでは全 $X_t$ のambient下界を結論しない。 |
| Source-free束座標と一つのprimitive | `source_free_neck_coordinates.tex`, `pair:prop:bundle-conic`, `pair:cor:global-primitive` | Source・tripleを除いた二重線 $D^\circ$ の**固定**compact base上のexact $uv=t$ とnormal action。$\Omega=d\log v\wedge\tau$、$\lambda_t=d^c\log(\omega_t^2/\lvert\Omega\rvert^2)$ を固定。本稿のmoving exhaustionは固定段階の定数を先に取り、遅い対角選択で処理する。任意の指定速度に一様な外部定理とは読まない。 |
| 共通moment interval | 同上 `pair:thm:fixed-end-moment`, `pair:cor:actual-common-moment` | Period 1のnormal generator、$\iota_V\eta_t=-d\mu_t$。固定endで $\mu_t=\pm4\pi/s_r+O(s_r^{-1-\delta})+o_t(1)$、$s_r=-\log r^2$。**先に $r$ を固定し、その後 $t\to0$**。Average $\eta_t$ の結果で、actual formへのMoser flow生存を含まない。 |
| Normal circle上界の十分条件 | `source_free_neck_comparison.tex`, `neck:lem:rank-one-circle`, `neck:cor:buffer-circle` | $p^*h_D\le A\omega_t$、$\omega_t^2\le B(h_A+h_D)^2$ からvertical方向 $g_t\le ABg_A$。Actual ball bufferを別に仮定して円の長さ $O(1/\min(s,M_t-s))$。Mixed termsを許す。この外部補題自体はbufferを与えず、必要な固定段階のbufferは本稿のK1–K2で証明する。 |
| Exterior比較 | IV `coarse:hyp:TC5`, `coarse:cor:exterior-comparison` | **TC5は未検証仮定**。各点で正しいorientationのmodelに対し $h_t^{\rm mod}\le C\omega_t$。これに依存するsource直径・connector・粗い比較を無条件化しない。 |
| 全域のGH極限 | V `hyp:CPd`, `hyp:PBEd`, `thm:degree-d-limit`; IV `ass:PBEd`, `thm:degree-d-cogram` | **CP/PBE付き**。CPはraw density、source局在、粗い二側距離とfinite connectors。PBEはterminal product座標、protected rectangular inclusion、全radiusでの一様比較、actual/model両距離のescapeとcompatible exhaustion。局所chart存在だけでは不足。 |
| Rank-one Schwarz計算と局所最大値原理 | S.-T. Yau, *A general Schwarz lemma for Kähler manifolds*, Amer. J. Math. 100 (1978), 197–203, Theorem 2・式(16)とその証明、[doi:10.2307/2373880](https://doi.org/10.2307/2373880)、[掲載版PDF](https://archive.ymsc.tsinghua.edu.cn/pacm_download/59/11034-Shing-Tung_Yau_30.pdf) | 一次PDFのTheorem 2と証明を確認。主稿の参考文献は `YauSchwarz`。本稿 `ke_sharp_normal.tex` では $\Delta\log U\ge U-1$ の係数をBochner計算から直接導き、actual球上のcutoffと全境界を明示する。局所領域にcomplete-source版の結論を無条件で適用しない。 |
| Complex Sobolev関数のGaussian可積分性 | Dinh–Marinescu–Vu, *Ann. Sc. Norm. Super. Pisa* (5) 24 (2023), 927–954, Theorem 1.2・pp.928–929、[掲載版PDF](https://www.mi.uni-koeln.de/~gmarines/PREPRINTS/Dinh_Marinescu_Vu_ASNP_2023.pdf) | 一次資料で仮定を確認。固定Euclidean領域の距離函数に適用し、固定補助potentialの測度を使う。Actual potentialの一様Hölder性は仮定しない。正規化coverの周期数を除してactual体積のGaussian tailへ移す部分は本稿で証明する。 |
| 局所potentialの連続度による距離評価 | Guedj–Guenancia–Zeriahi, [arXiv:2310.20482v1](https://arxiv.org/abs/2310.20482v1), Proposition 1.4, p.5 | 一次PDFで仮定と証明を確認。固定Euclidean領域のpotentialに一様square-root-Dini modulusがあればcoreの径は $O(1)$。本source族でのそのmodulusは**未証明**。別の条件付き十分入力として保持し、P0の証明には使用しない。 |

`multiscale-kaehler-einstein` の固定配置補空間に関する結果はIVが引用する外部入力であり、固定空間の漸近から退化族上の一様性を自動的に導かない。本更新ではそのrepoと引用一次論文の全証明を再監査していない。具体的な結果を新たに使用するときは、IVの引用箇所から一次資料の定理・仮定を確認する。

## 本repoで接続する結果

| 入力・障害 | 原稿の所在 | 使用上の区別 |
| --- | --- | --- |
| 実際のLagrangian closed corner | [ke_closed_corner_gh.tex](../papers/sections/paper/ke_closed_corner_gh.tex), `ke:closed-corner-gh`, `ke:closed-corner-protected-gh` | 同じMoser像・同じfibrationに対する局所結果。Protected distanceを全曲面距離と同一視しない。 |
| 有限cutと遅いcutのclosed corner | 同上 `ke:slow-cut-closed-corner-gh` | $m\ge m_*,\ R\ge R_*,\ \log(m+1)+4\log R\le R/8$ でdistortionは $C[m^{-1}+(\log(m+1)+\log R)/R]$、非正規化fiber内在径は $C/m$。固定cut後のparameter選択が可能。$m\to\infty,\ \log m=o(R)$ でGH収束を得る。Full-triple比較は深度 $m/2$ の有限下限以上で一様、rank-one Schwarz・dominant-product・有限galleryも使用。 |
| 固定baseの同一moment上の接続 | [ke_staged_neck_averaging.tex](../papers/sections/paper/ke_staged_neck_averaging.tex), `ke:fixed-base-moment-connectors` | Source-freeな固定連結基底に限り、level全体とMoser像のactual ambient径 $O(1)$、正規化後 $O(R^{-1})$。異なる残余点を結ぶ。`ke:fixed-base-central-band` は固定 $A>0$ に対する $\lvert\mu\rvert\le A/M_t$ のband全体を、異なるmomentも含めactual径 $O(1)$ とする。Source・moving collar・全曲面の下界は含まない。 |
| 三armの座標・normal period | [ke_neck_corner_transition.tex](../papers/sections/paper/ke_neck_corner_transition.tex), `ke:arm-log-derivatives`, `ke:three-arm-coordinate-interpolation`, `ke:transition-normal-primitive` | 共通の許容射影を選び、固定深度比で分離したarmに限る。全固定階で指数的小摂動、積保存smooth補間、canonical normal periodの厳密一致。非正則補間帯はtame symplecticでありKähler性を仮定しない。第二periodの一致は含まない。 |
| 三端の平均順序の相対統合 | [ke_relative_corner_patch.tex](../papers/sections/paper/ke_relative_corner_patch.tex), `ke:quantitative-order-hamiltonian`, `ke:relative-corner-patch`, `ke:single-arm-reduced-graph`, `ke:arm-common-moment-strip` | 小さいprimitiveを固定し、centered平均の比較Hamiltonianを $O(m^{-2})$ で評価。Common source/imageとcutoff buffersの下で端ごとのstaged bundleを一つのactual corner bundleへ統合。単一moving armでは共通moment stripとactual reduced graphを証明。Source-inclusive neckとの共通flow領域と全交わりは、下のexhaustionの結果で別途確保する。 |
| Source中心の特異reductionとclosed fibre | `ke_staged_neck_averaging.tex`, `ke:source-reduction-pinched-fiber` | 固定parameterのsmooth primitive・両normal cutsのmoment符号・共通Moser存在域を仮定として分離する。固定点でchain primitiveと場が零、canonical momentも零。位相商 $I\times P$、閉pinched torus、primitive vanishing cycleを直接証明する。零reductionの通常の滑らかさやparameter一様正規形を仮定しない。 |
| 全stageと小さい複素parameterに共通な木 | `ke_neck_corner_exhaustion.tex`, `ke:fixed-marked-tree-exhaustion` | 一つのembedded pants foliation、単純sourceの一価bump isotopy、共通compact外のend graph補正を用いる。Core collar補間とwhole-fiber trimも同じ木を保つ。全 $H_1(T^2)$ markingの族全体の自明化は結論しない。 |
| Source-inclusive neckとcornerの全交わり | [ke_neck_corner_exhaustion.tex](../papers/sections/paper/ke_neck_corner_exhaustion.tex), `ke:fixed-stage-source-neck`, `ke:neck-corner-diagonal-matching`, `ke:neck-corner-saturated-union` | 残余compact→normal cutoff→moment区間→parameter閾値の順に選ぶ。Corner cut $6b_j$ とneckの葉でのtrim $7b_j$、first-exitと逆flow自然性により全交わりを同じ全fibersで飽和させる。Source・saddleを含む部分fibration。全曲面被覆・core・global GHは含まない。 |
| Central sourceの体積・moment・経路 | [ke_source_connectors.tex](../papers/sections/paper/ke_source_connectors.tex), `ke:source-central-density`, `ke:source-central-moment`, `ke:source-central-mean-distance`, `ke:source-central-short-escape`, `ke:source-central-arm-connectors` | 固定rescalingでdensity $L^{-2}$、有界potential、moment $O(L^{-1})$、平均二乗距離 $O(1)$、inradius $O(L^{-1/2})$、arm断面への接続 $O(1)$。Capped volume下界・oriented pair-arm density・complete volume上界を使用。全点径は結論しない。 |
| Source中央帯の全点径 | 同上 `ke:source-central-band-reduction`, `ke:source-potential-modulus` | $\lvert\mu\rvert\le A/L$ のsource中央帯を固定rescaled coreへ $O(1)$ で結ぶ。`ke:source-central-diameter` と `ke:fixed-base-source-central-band` により、固定点を含むcoreと固定基底中央帯・閉pinched torus全体のactual ambient径は $O(1)$。一様square-root-Dini modulusは**未証明**だが、Gaussian体積評価とBishop比較による証明に加え、`ke:source-direct-central-exit` のgate・arm・水平経路による直接証明がある。いずれもそのmodulusを用いない。全intervalには `ke:source-all-moment-exit` を用いる。 |
| Source-inclusive全moment退出とlevel合併 | `ke_source_all_moment_connectors.tex`, `ke:source-arm-uniform-tensor`, `ke:source-direct-central-exit`, `ke:source-all-moment-exit` | Source軸・固定点を含む全intervalで同じmomentの残余境界へ $O(1)$。三境界のrank-one Schwarz、射影下界、volume上界からarm tensor比較を導き、水平・動径経路で接続。中央点は短いgate退出を併用し、Gaussian可積分性を入力にしない。Target parameter化・全域下界は含まない。 |
| 固定残余compactの法線エネルギーと接続 | [ke_staged_neck_averaging.tex](../papers/sections/paper/ke_staged_neck_averaging.tex), `ke:neck-integrated-normal-energy`, `ke:neck-axial-upper`, `ke:neck-averaged-speed`, `ke:neck-shrinking-buffer` | KE側 `neck:prop:volume-envelope` から積分短円と同一残余点の係数1の接続上界。実計量の境界距離（上限1） $\delta_t$ が $m_t\delta_t^2\to\infty$ なら共通source・像。この十分条件と、K1–K2の固定段階で実証したbuffer・遅いexhaustionを区別する。 |
| Normal平均の双方向buffer | [ke_staged_neck_averaging.tex](../papers/sections/paper/ke_staged_neck_averaging.tex), `ke:short-circle-actual-buffer`, `ke:short-circle-image-buffer` | Actual短円とactual bufferを入力とする。像のambient直径を与えるが、$C^1$ 制御・intrinsic fiber径・base projection保存は与えない。 |
| Endsとneckの接着 | 同上 `ke:staged-neck-averaging`, `ke:staged-reduced-extension`, `ke:staged-neck-scope`; `ke_closed_corner_gh.tex`, `ke:relative-neck-matching` | 共通primitive・marked periodsを追跡できる。Reduced foliation germsの同時延長、開overlapの同じfiber partition、actual flowの生存は別に確認する。 |
| 距離の全域化 | [base_topology.tex](../papers/sections/paper/base_topology.tex), `topo:finite-portal-criterion`, `topo:finite-endpoint-comparison`, `topo:portal-counterexample`, `topo:ke-map-compatibility` | (N) no-shortcut、(S) square lifts、(F) fiber/portal connectorsは別入力。(F)は(N)+(S)から従わない。現行の上界は、再parameter化後のexact square liftを仮定せず、旧cornerのendpoint距離と共通momentの接続を有限galleryに直接適用する。下界は全域scalar mapで別途証明する。 |

## 中央sourceの全点径とcomponent移送の追加入力

主稿 `ke_source_potential_buffer.tex` はcapped/actual density比較を固定source tube全体へ統合し、射影下界と正のcanonical potentialのPoisson方程式からactual球の深部局在を証明する。`ke_source_global_distance.tex` はDinh–Marinescu–Vu, Ann. Sc. Norm. Super. Pisa (5) 24 (2023), Theorem 1.2（[掲載版PDF](https://www.mi.uni-koeln.de/~gmarines/PREPRINTS/Dinh_Marinescu_Vu_ASNP_2023.pdf)、pp.928–929で仮定確認）を距離函数に適用し、logarithmic coverの周期数を除してactual Gaussian tailを得る。`ke_source_diameter.tex` は同じactual球へのBishop–Gromov比較から全点径を導く。Actual potentialのHölder性、TC、局所tensor二側比較は追加仮定しない。このGaussian経路は独立な補助結果として保持し、現行の全moment退出と中央径には `ke:source-direct-central-exit` の直接経路を使える。

`ke_component_core_transfer.tex` はfixed-gauge smooth KE収束のcanonical primitive差から固定compactのactual移送を構成する。相対flux条件とexact collar germは証明した。`ke_component_core_geometry.tex` は任意固定compactで厳密一致するsmooth正則化、正residueの有限型KE coreとその小さい飽和近傍のfillingを与えるが、その存在だけから全collar葉の一致は従わない。現行の全域接着は下記四節によりactual linkから直接構成する。Smooth compactifying formの `comp:finite` をこの極限形式の定理と読み替えない。


Actual全域構成の追加証明は次を用いる。

| 入力・結論 | 主稿の節・ラベル | 検証範囲 |
| --- | --- | --- |
| 正residue period、閉link、固定段階の被覆とtrim | `ke_component_link_cover.tex`、`ke:component-meridian-normalization`、`ke:closed-component-link`、`ke:fixed-stage-stratum-coverage`、`ke:whole-fiber-core-trim`, `ke:anchor-trimmed-neck-domain` | 共通anchorで保持neckは正確に $[-\delta,\delta]$、外側尾部は各coreへ入る。Cornerのdominant-productは全深度比に一様。Source基底点を含むfixed-shell上界はRZの通常component cusp上で証明。整数windingとexact transportでmoment定数も同定。 |
| Actual invariant primitive | `ke_core_invariant_primitive.tex`、`ke:component-normal-generator-c1`、`ke:relative-corner-patch-c2`、`ke:component-shell-primitive-support` | RZの全cusp derivatives、triple全固定階比較、広いK2 construction domainsを使用。追加の全域tensor仮定なし。 |
| Saddle-moving relative family | `ke_relative_reduced_foliations.tex`、`ke:saddle-moving-relative-interpolation` | 各connected critical leafに一つのsimple saddle、boundaryのleaf partition固定。Global vector fieldの直接証明。非零moment bandのactual Lagrangian lift。 |
| 全域core接着 | `ke_actual_core_gluing.tex`、`ke:actual-global-fibration` | Evans–Mauri Lemma 2.16のcompact-domain版と上記入力。全曲面の連結fiberの全射とactual Lagrangian性、各componentごとの対数接続費用を与える。Uniform distortionは下の上下界と組み合わせて得る。 |
| Coreの弱い層別構造 | `ke_component_core_geometry.tex`、`ke:compact-relative-morse-smale` | Critical germs・境界primitiveを保つ小さいcontact holonomy修正、compact exact Moser、trapping compact内のbroken trajectories。次元順の閉isotropic filtration。Whitney条件は不要。 |
| Componentとneck尾部の対数費用 | `ke_actual_core_gluing.tex`、`ke:component-logarithmic-connectors`；`ke_global_ambient_upper.tex`、`ke:component-neck-tail-depth` | 固定cusp比較、$\int ds/s$、元のstrict psh potentialによる深度上界。尾部はmoment単調性と浅/深Moser分割で独立に深度 $CN_j$ に入れる。経路は拡大component compact内のambient経路であり、fiber内在距離ではない。 |
| Core cutのtarget cap | `ke_actual_core_gluing.tex`、`ke:core-depth-upper`、`ke:removed-corner-target-cap` | 固定成分のstrict psh potential・graph convergence・旧softmax逆式。各capは成分頂点へ一様収縮。保持cornerの旧protected距離と全曲面距離の上界を維持。全域parameterizationとambient下界は含まない。 |
| 全域基底parameter化と内部木の共通moment | `ke_global_base_compatibility.tex`, `ke:common-edge-moment-profile`, `ke:corner-cap-disk`, `ke:global-base-parameterization`, `ke:collapsed-tree-common-moment` | Weighted moment inverse、moment-cut capのproper arc、明示insetとstrip補間で全保持cornerの旧値へ $O((1+\log N_j)/R_t)$ 近接。内部木の中央部分では全枝共通momentを厳密に保つ。全曲面距離下界を含まない。 |
| Sourceを含む係数一の法線評価 | [ke_sharp_normal.tex](../papers/sections/paper/ke_sharp_normal.tex), `ke:normal-harmonic-depth-barrier`, `ke:sharp-scalar-normal-barrier`, `ke:sharp-global-one-active` | 正則global normal frameで $\Delta s=0$、$U=\lvert d\log s\rvert^2$ に $\Delta U\ge U(U-1)$。固定shell・moving shell・残余境界の全てを評価し、$1+\varepsilon_j+A_j\mathfrak n_j/s+C_js/(\kappa L)$ の障壁を使う。Source軸、physical-depth補正、triple外のactive全被覆を含む。SharpなRZ漸近や全neck tensor比較を追加仮定しない。 |
| 全域scalar mapとambient下界 | [ke_global_ambient_lower.tex](../papers/sections/paper/ke_global_ambient_lower.tex), `ke:global-depth-lipschitz`, `ke:same-moment-corner-reference`, `ke:global-depth-base-comparison`, `ke:global-ambient-lower` | 下側cut $\mathfrak m_j$ とplateau $L/K_j$ を用いる全域 $\Theta_t$。一方向はsharp normal、二方向はfull-tripleのco-Gramで評価し、任意の全曲面経路に沿って長さを抑える。同一momentのcorner参照点で全域値比較を証明。Corner移送の段階一様性と既存の許容cut条件で係数は固定族の $C$ とできる。経路の領域往復回数を有限と仮定しない。 |
| 内部木の全fiber合併とambient上界 | [ke_global_ambient_upper.tex](../papers/sections/paper/ke_global_ambient_upper.tex), `ke:collapsed-tree-full-fiber-collapse`, `ke:coherent-corner-portals`, `ke:global-ambient-upper` | 残余基底を先に選び、許容cut条件の下で全 $f_t$-fiberのambient径を $C(1+\log(N_j+1))$ で評価。全endsで同じmomentのportalsを選び、旧full-cornerのendpoint上界を高々60本のsquare galleryで接続する。除去capを通る曲線もambient上界には使用できる。 |
| 全域quotientと合成fiberの連結性 | `global_gluing.tex`、`glue:closed-whole-fiber-quotient`；`base_topology.tex`、`topo:connected-preimages`、`topo:cubical-composite-connected` | 有限閉piecesのwhole-fiber飽和から閉同値関係を作る。後段の基底同定に依存せずHausdorff性を得て、閉写像の連結逆像により同じ $f_t=p_T\pi_t$ の全fibersも連結。内部木上の合併には三次元部分があり得る。 |
| Fiber Euler関数とcoarse fiber | `invariants_examples.tex`、`inv:euler-pushforward`、`inv:cubical-fiber-euler` | 実際の有限層化・局所productと $\chi_c$ の加法性を用いる。非零寄与はnodesとcoresのみ。Cubical像でのnode衝突は重複度付きで数え、例示した面別node配分を一般存在の必然条件とせず、追加の作用atlas条件下での六次bigon剛性は保持する。数値一致をgluingの代用にしない。 |
| 同じactual写像による大域実現 | [ke_global_metric_realization.tex](../papers/sections/paper/ke_global_metric_realization.tex), `ke:global-metric-realization` | 上記の同じ $\pi_t$ と $f_t=p_T\pi_t$ に、全固定段階の条件を満たす一つの遅い対角選択を適用。全射性、uniform ambient distortion消失、GH収束、全fiber合併の一様収縮を得る。許容cut下の上下両側の明示budgetを固定族の一つの係数で与える。Cutの成長と閾値は未評価。外部CP/PBE/TCの結論を入力にしない。 |
| Focus写像の判定と全飽和近傍の作用 | `ke_staged_neck_averaging.tex`、`ke:source-focus-transversality`、`ke:focus-neighborhood-period`、`ke:focus-whole-neighborhood-transport` | 一つの残余periodでclosed primitive差のexactnessを判定。Symplectic push-forwardでTaylor不変量、exact transportで追加定数項も保存。任意先指定模型とのmatchingやparameter間の不変量一定は含まない。 |

## Sourceとmarked葉層の一次資料

Zung, *A note on focus-focus singularities*, Differential Geometry and its Applications 7 (1997), 123–130, DOI [10.1016/S0926-2245(96)00042-3](https://doi.org/10.1016/S0926-2245(96)00042-3)、[一次原稿 math/0110147](https://arxiv.org/pdf/math/0110147) の§2、§3 Proposition 3・Corollary 1、§4を確認した。Focusの局所二次型・pinched fibre・monodromyは既知結果である。本稿では明示的なsymplectic線形変換と閉fibreのcompactificationを直接計算し、actual neckの固定点・canonical moment・Moser存在域との接続を確認する。既知の局所分類から退化族に一様な解析評価を推論しない。Vũ Ngọc, Topology 42 (2003), Theorem 2.1（[一次原稿](https://arxiv.org/pdf/math/0208245), PDF p.4）のsemi-global分類も照合し、単純nodeの同じ線形monodromyからformal power series不変量の一致を導かない。

Vũ Ngọcの同一次原稿§3（PDF pp.6–8）、Lemma 4.1と§4（pp.9–11）、§6（pp.14–16）、§7 “Exact version”（p.18）を照合した。通常のconstant-zero Taylor不変量と、primitiveをデータに加えた残余作用の定数項を区別する。ZungのPDF p.4のerratumは位相分類をhomeomorphicと訂正しており、smooth foliated equivalenceの根拠にはしない。本稿のblock/Mayer–Vietorisとsourceへのexact transport適用を独立点検した。Nodal surgeryのCG/Flemingの適用範囲、例外面積による容量規約、支持と選択順序は [研究ノート](notes.md#nodal-blow-upの実面積と比較写像の支持) に整理する。

一般symplectic存在構成の `glue:area-normalized-blowup` と `glue:components` は、例外面積によるradial Kähler構成とCGの局所比較を用いる。全compact nodal neighborhoodsを確保後にnormal collarsを離し、独立primitiveのexact一致を仮定しない。これは `global_gluing.tex` の構成経路の入力であり、actual KE距離比較の追加解析仮定ではない。

Maksymenko, Comment. Math. Helv. 80 (2005), 655–690, DOI [10.4171/CMH/30](https://doi.org/10.4171/CMH/30) の[掲載版](https://ems.press/content/serial-article-files/43060)で、Main Theorem p.658、Lemma 4.1 p.665、§6.1 Lemma 6.4 p.668を確認した。Path-component分類だけからfixed Reeb treeは従わず、本稿では支持を明示した葉層のdiffeomorphismsを使う。第二cycleのparameter monodromyと、abstract labelled treeの固定は区別する。

## SNC相対primitiveとnormal holonomyの入力

| 入力・本稿の結果 | 確認した範囲と制限 |
| --- | --- |
| IKM 掲載版Lemma 4.8、Theorem 4.6の証明、§5 | 成分上の正則葉period消滅とsmooth basic representativeの対応は既知。本稿 `snc:reeb-leaf-kernel` は整数格子とSNC完全列を確認し、障害の次元を $\sum_a g_a$ とする。 |
| TMZ Definitions 2.11–2.12、Theorem 2.13（arXiv:1410.0609v3, pp.16–17） | Compatible regularizationはexact deformation後の結論。固定された元の形式・任意指定connection/holonomyの同時実現や固定複素構造でのKähler性を自動的に与えない。 |
| BSV 掲載版Propositions 2.5・2.7・2.10、Remark 2.11（pp.30–31） | OrthogonalityとscH、positive real divisor coefficientsに対するadapted primitiveの存在。Prop.2.10に $H^1(M)=0$ やmonotonicityは不要。指定core germ・normal connection・marked full leavesの相対実現は別途証明する。 |
| `snc:fixed-holonomy`、`snc:minimal-holonomy-controls` | 固定connection・coupling chartsのbasic＋exact-cutoff経路は各成分の $g_a$ 個の独立葉periodが零 iff 実行可能。全障害を消すholonomy調整のrankは $\sum_a g_a$。全 $2g_a$ periods消去は過剰な十分条件。 |

Basic補正は全critical collarsの外へ支持を取れるが、全full critical-leaf collarsで零のclosed connection補正は障害空間に作用しない（`snc:saddle-support-obstruction`）。非零障害のholonomy補正は一般に元のfull saddle collarsを変更し、$D$ 上のmarked full leavesを固定して新しいcoupling chartsでliftする。Unitary phasesだけの固定には整数periodのgauge自由があり、固定connection/gaugeの命題と同一視しない。有限endpointはactual collar座標による $r$ の明示式で連続性を確認する。既知の成分上の原理と本稿のSNC統合・coupling適用を区別する。書誌・一次URL・正確な頁は [研究ノート](notes.md#sncの固定coupling-chartsと葉のperiod障害)、証明は `relative_compactification.tex` を参照する。

## Normal action・第二period・作用atlasの接続

| 結果・入力 | 適用範囲 |
| --- | --- |
| `neck:regular-period-matching`、`neck:normal-action-counterexample` | 可縮な正則bandと既定base同定の下で、第二作用は整数shear・符号・定数までの一致が必要十分。Exact matchingでは固定primitiveの定数差も零。既知action-angle理論の適用であり、normal momentだけからは従わない。 |
| `ke:transition-residual-period` | Canonical frameの比 $a(p)$ は残余periodを $-2\pi\operatorname{wind}(a_t\circ p\circ\gamma)$ だけ変え得る。Normal periodの一致と作用原点の一致を区別する。 |
| `atl:critical-action-obstruction`、`atl:fixed-form-bent-branch` | Critical actionの有理直線性は任意denominatorのmatroidal chartにも必要。固定actual形式・normal action・両端/toric/saddle点germs・marked treeを保つ非線形面積変更で破れ得る。 |
| `ga8:affine-persistence`、`ng8:central-criterion`、`ng8:straight-neck` | 同時symplectic transport、共通primitive・reference、実面積と整数framing、切片を個別に確認する。葉の補間には同じ $\operatorname{Diff}_0(P\operatorname{rel}\text{ collars})$-orbitを使う。抽象木やnormal actionだけでは不十分。 |

Evans arXiv:2110.08643v4 のTheorem 1.42、Lemma 2.15・Remark 2.17、Lemma 2.25が正則bandの入力である。一次URLと頁は [研究ノート](notes.md#正則bandの第二作用と非直線critical-action)。一般baseでのexactnessや、特異fiber近傍の分類をこれらの正則定理だけから導かない。新証明の独立内部点検、一次資料照合、組版の完了範囲は検証資料へ分けて記録する。

## Coreの層別構造と相対fillingの一次資料

- Evans–Mauri, *Constructing local models for Lagrangian torus fibrations*, Ann. Henri Lebesgue **4** (2021), 537–570, Definition 2.1、Lemma 2.16、Remark 2.18。[掲載PDF](https://ahl.centre-mersenne.org/item/10.5802/ahl.80.pdf)、[arXiv:1905.09229v3](https://arxiv.org/abs/1905.09229v3)。本稿は指定contact formを固定したcompact cone fillingを直接証明し、任意contact rescalingが既存葉を保つとは仮定しない。
- Cieliebak–Eliashberg, *Flexible Weinstein manifolds*, MSRI Publications **62** (2014), 1–42, §4A Lemma 4.1。[一次PDF](https://library.slmath.org/books/Book62/files/eliashberg.pdf)。Holonomy変形は既知。原典の上端constant scalingを許す版だけを根拠にせず、本稿は小さいcontact isotopyの明示liftで両端primitiveの完全固定を証明する。
- Eliashberg, *Weinstein manifolds revisited*, [arXiv:1707.03442v2](https://arxiv.org/abs/1707.03442v2), §1 pp.2–3。Exact Moser移送、Morse coreのisotropic stratificationとWhitney条件の区別を確認。一般critical germでWhitney条件を無条件に引用しない。
- Abbondandolo–Majer, *Stable foliations and CW-structure induced by a Morse–Smale gradient-like flow*, [arXiv:2003.07134v2](https://arxiv.org/abs/2003.07134v2), Introduction pp.1–2、Theorem 1。原典はclosed manifold上のflow。本稿はcompact domainへ無条件適用せず、境界から離れたtrapping compact内のbroken trajectoriesから必要なclosure関係を直接示す。

Leung–Symingtonの分類は掲載版 JSG 8 (2010) のTheorem 2.1（pp.148–149）とTable 1（p.144）に統一した。旧arXiv版のTheorem 2.6を掲載版の番号として用いない。Evans–Mauriのcontact formに関する注は掲載版・arXiv v3ともRemark 2.18（掲載頁544）である。

以上の指定箇所と本稿の適用は複数担当で読み合わせた。PrimitiveのC1評価・全cutoff support・nontrapping、relative reduced foliation、whole-fiber trim、閉quotient、core/collar費用も重点監査済み。全旧局所証明・全一次資料の包括的監査とは区別する。

`ke:component-flux-space` はCohen–Suciuの既知のboundary cohomology（Proposition 2.5、Corollary 2.6、§6.9、主稿の参考文献 `CohenSuciuBoundary`）を一般位置直線配置へ適用する。各componentの相対障害空間は $H^1(S;\mathbb R)/\operatorname{im}H^1(K;\mathbb R)\cong H_2(K;\mathbb R)$、次元は $\binom{d-2}{2}$。`ke:nonextendible-small-core-germ` は固定actual形式で非零障害を小さいsymplectic collar flowとして実現する。既知cohomologyの新規性や任意の指定germの延長を主張しない。

## 固定成分coreのcusp入力と有限target幾何

Rochon–Zhang, *Adv. Math.* 231 (2012), 2892–2952, [arXiv:1106.0873v2](https://arxiv.org/abs/1106.0873v2), §5 (5.3)–(5.6), Theorem 5.1を一次資料で確認した。SNC全体におけるbounded $C^\infty_{fc}$ potentialを用い、smooth divisor専用のfull expansionは使わない。$K_{\mathbf P^2}+D=\mathcal O(d-4)$ のamplenessと本稿の $dd^c=i\partial\bar\partial$ を照合し、$u=-2\sum\log s_a+v$ を使用する。正則化・有限型性・compact exact Moserと局所core fillingの証明は本repoの `ke_component_core_geometry.tex` が正本。

`topo:coordinate-retraction` によりclosed-cornerのtargetの内在距離は全複体距離の制限と等しい。六labelのgallery還元と `topo:diameter-six-labels` の $D_d=2\sqrt5$（d≥6）は解析仮定から独立。直径対の線形安定性 `topo:diameter-six-stability` だけはVの `thm:intro-diameter-C5`・`sec:finite-diameter`（確認commitは上記と同じ）の $D_5=\sqrt{13}$ を使用する。四galleryと120三角形は本repoの保存された有理数検算により確認されている。現行のuniform distortionと全射性からactual曲面の正規化直径も $D_d$ へ収束する。具体的な数値 $D_5=\sqrt{13}$ の適用には上記五次の有限target距離結果を用いる。

## 大域実現を支える接続とパラメータの選択

### 1. Actual normal circleとflowの共通領域

固定 compact の source-free 基底で normal 深度だけを動かす場合は、主稿 `ke:fixed-base-neck-moser` で解決した。$\Omega_{t,d}^{\rm low}$ の大域下界、capped background の射影下界、固定 pair chart の体積上界を使い、射影包含の大域 Chern–Lu と actual ball 上の局所 Chern–Lu を順に適用する。共通の縮小 moment interval は `ke:neck-deep-moment-strip`。遅いresidual exhaustionの束座標・共通flow領域は `ke:neck-corner-diagonal-matching` で確保した。任意に指定した縮小速度への一様性は主張しない。Source gate 近くでは射影距離による buffer を rescaled normal 距離へ読み替えない。 Source 模型では `coarse:lem:pair-arm-density` と `coarse:lem:complete-volume-upper` を oriented 側に使い、正則ベクトル場の Bochner 不等式で central source まで法線生成場の $O(L_t^{-1})$ 評価を得た（`ke:source-short-circle`）。

### 2. 同じglobal fibrationへの相対接着

`ke:actual-global-fibration` により固定stageの全域接着を証明した。K2の全intersection saturationを入力とし、閉moment link・actual invariant primitive・非零moment帯のsaddle-moving補間・whole-fiber trimを実証する。全曲面被覆はfixed-shellの上界と同じnormal flowの逆像bufferを使い、部分fibrationの外を各componentの固定compactへ閉じ込める。各componentのcoreと変更collarのactual ambient径・選択した接続費用は、`ke:component-logarithmic-connectors` により $C(1+\log(N_j+1))$。固定componentのcusp上比較と動径経路を用いる。内側のprimitiveはcompact-relative Morse–Smaleに選び、次元順の閉isotropic filtrationを確保する。独立に先指定した全periodやcritical valuesを合わせる定理ではない。Actual Lagrangian性と連結fiberの全射を、次の距離評価の前に確保している。

### 3. 全曲面のscalar下界

Sharp normal比較領域は、sourceを除かない固定残余compact上の正則annulus bundleである。固定した $\kappa>0$ に対する $s=\kappa L$ の粗い上界は、独立に証明したsource-arm tensor比較で供給する。その前段はpositive-Poisson bufferとlocalized rank-one Schwarzであり、global scalar障壁へ依存しない。残余境界はfull-triple、固定外側shellは射影下界と座標微分の上界を用いる。全境界を明示した最大値原理により

\[
|d\log s|_{g_t}^2
\le1+\varepsilon_j+A_j\mathfrak n_j/s+C_js/(\kappa L)
\]

を得る。比較領域の境界 $\kappa L$ と、clipped mapのplateau $L/K_j$ は異なる。新しい下側cut $\mathfrak m_j$ は旧corner cut $m_{\mathrm{old}}=6b_j$ と独立であり、全固定段階の定数と非成分深度の上界を決めてから選ぶ。

Global Hermitian depthsを $\ell_i=-\log\|L_i\|^2$ とし、

\[
\Theta_{i,t}
=\left[\frac{\log(\ell_i/\mathfrak m_j)}
 {R_t-\log\mathfrak m_j-\log K_j}\right]_0^1
\]

とする。少なくとも一座標が1、非零座標は高々三つなので、active covectorsは高々二本である。一active方向はsharp normal、二active方向はfull-tripleのdominant-product co-Gramで制御する。この全域微分評価を任意のrectifiable curveに積分するため、neck・corner・coreの往復回数に比例する誤差は生じない。先に $\Theta_t$ の全域Lipschitz評価を証明し、それをMoser前後の比較に使う。共通anchorの領域分解を確定し、保持neckの各点を同じmomentの旧corner辺torusへ接続する。既証のLipschitz評価でその参照点から値比較を移し、core cap制御と合わせて $\sup_xd_\square(\Theta_t(x),f_t(x))\to0$ を得る。参照点の費用は既証のsource-inclusive同一moment接続から取り、後続の全域上界を入力にしない。固定残余基底のMoser被覆・同一moment接続・中央帯は、有限下限以上のcutに一様な形で使用する。

### 4. 共通momentの全fiber合併と上界

保持cornerの旧softmaxと全域の $p_T\pi_t$ の値の整合は `ke:global-base-parameterization` による。Core capの位置だけでなく、moment profileとcap境界のproper arcを用いる。潰される内部木では全枝に同じlongitude $\sigma_t(\mu)$ を使うので、辺の中央値の逆像は厳密に同一moment上の全fiber合併である。

Source側では中央全点径と共通interval全体の同一moment退出がともに $O(1)$。`ke:source-arm-uniform-tensor` は三境界のnormal covector評価とvolume上界からsource軸を含むarmの二側比較を与え、`ke:source-all-moment-exit` は水平・動径の直接経路で証明する。中央固定点には短いgate退出を先に用いるため、この接続はDMV/Gaussianに依存しない。残余基底は旧辺全体の $m_j\le B<m_j+1$ を使って $N_j$ より先に固定する。その接続定数 $C_j^{\rm neck}$ とcomponentの対数費用から、まず $H_j\le C(1+\log(N_j+1))+C_j^{\rm neck}$ を得る。許容cut条件 $C_j^{\rm neck}\le1+\log(N_j+1)$ を加えれば、全 $f_t$-fiberのambient径は $H_j=C(1+\log(N_j+1))$ で抑えられる。`ke:component-neck-tail-depth` はanchor外の尾部にも深度 $CN_j$ を与える。これは残余定数の増大率の解析評価ではない。Gaussian体積定理は有効な独立補助結果として保持する。

Target最短路は `topo:six-label-gallery` により高々60本のsquare線分で選べる。各junctionに同じnormal momentのcorner portalsを取り、旧full-cornerのambient endpoint上界と $H_{j,t}$ を有限回足す。これはtarget最短路に対する有限galleryの使用であり、sourceの任意の経路の出入り回数を制限する議論ではない。再parameter化後の $f_t$ に厳密に写るsquare liftsは要求しない。

### 5. 一つの遅い対角選択

固定 $j$ ごとに $b_j$、残余compactsとその接続定数、K2のnormal cutoff $n_j$、共通moment区間を先に決める。次に既存下限と $C_j^{\rm neck}\le1+\log(N_j+1)$ を満たす $N_j$、core・collarを決める。その後、sharp barrier専用の補助cut $\mathfrak n_j$ と境界定数 $A_j,C_j$、有限費用を全て確定する。$\mathfrak n_j$ は $n_j$ と独立であり、既存のcoreや $N_j$ を選び直さない。最後に $\mathfrak m_j$、$K_j$ を大きく選び、$t_j$ を小さくする。$\varepsilon_j\to0$、$b_j,\mathfrak m_j,K_j\to\infty$ とし、

\[
\frac{1+\log\mathfrak m_j+\log K_j+\log(N_j+1)}{R_t}\longrightarrow0
\]

と各固定段階の構成・比較に必要な全てのparameter閾値を課す。値比較の乗法係数は固定族の定数となり、別の $C_j$ を表示する必要はない。これにより上下界、各componentの費用、全fiber合併径を同じ $j(t)$ と同じ $f_t$ で制御する。固定triple内の $O(\log R_t/R_t)$ をそのまま大域の収束速度とする主張ではない。

## 主要な外部解析入力の重点監査

以下は本稿の接続に必要な証明を読み合わせた範囲であり、外部主稿全体の独立再検証を意味しない。

1. **Capped volume下界。** IV `coarse:cor:degree-d-volume-lower` のadjunction規格化、smooth Hermitian frameの誤差吸収、六種類の局所determinant下界を点検した。Sourceでは射影Morse座標だけに置き換えず、元のplane coordinatesのcap項を保持して、rescaling後の二方向の係数が $c/L$ 以上になることを使う。正のminorの和なので相殺は起こらない。これをcompact minimum原理へ入れる順序であり、先にactual tensor比較を要求しない。
2. **Full-triple比較の最小入力。** `full_triple_comparison.tex` の `coarse:rem:full-triple-face-input` に、固定深度 $m_0$ の境界面全phaseでの $\omega_t^2\ge c_*V_L$ がvolume障壁の下側に十分なことを明記した。固定 $t$ のradial closureと角度torusはexact triple chart内でcompactである。拡大simplexが下側、縮小simplexが上側の障壁となり、後者は人工境界で発散する。深部内部全体のdensity floor、actual距離buffer、actual metricの完備性をこの段階で入力にしない。$v=\log(\omega_t^2/k_L^2)$ と $dd^cv=\omega_t-k_L$ の同じRicci規格化も照合した。
3. **Small perturbationからtensor比較へ。** O. Savin, *Comm. Partial Differential Equations* 32 (2007), 557–578, Theorem 1.3・§4 Proposition 4.1、[掲載版PDF](https://www.math.columbia.edu/~savin/Small_pert.pdf)、[doi:10.1080/03605300500394405](https://doi.org/10.1080/03605300500394405) を一次資料で確認した。Complete模型のcoarse tensor下界は半平面へのSchwarz、上界はdeterminant比較から先に得る。全深度比のnormalized windowsで模型係数の高階評価を確保した上で、determinant作用素の単調な拡張、零近傍の一様楕円性と $C^2$ bound、$\|v\|_{C^0}=O(m^{-1})$ を照合した。Small $C^{2,\alpha}$ の後にbootstrapと線形化を使って $C^q$ 誤差 $O(m^{-1})$ に進む。模型側のdominant-product squeezeとfacet幅 $\beta=(b^2d_*)^{1/3}$ も点検し、active co-Gramの係数1がこの順序で得られることを確認した。
4. **Complete volume上比較。** IV `coarse:lem:complete-volume-upper` の一般形は $u=\log((\pi_D^*\omega_t)^2/h^2)$ の $\sup_Du<\infty$ を仮定する。Ricci下界から使えるLaplacian型最大値原理とAM–GMにより $\Delta_hu\le\epsilon$ の点で $e^u\le(1+\epsilon/2)^2$、従って $\omega_t^2\le h^2$ となる。Hessian型原理や、完備性だけによる $u$ の上有界性は用いない。実際のfinite ball・annulus–disc・product windowsとangular coversでは、固定 $t$ のclosureへの延長、model densityの境界発散、deck周期性を各適用で確認した。この点は外部正本の一般形にも反映してある。
5. **Component極限とSNC cusp。** Song [arXiv:1706.01518v1](https://arxiv.org/pdf/1706.01518v1) のDefinition 2.3（p.8）、Lemma 3.7（pp.15–16）、Lemmas 4.4–4.5（pp.22–23）と、Rochon–Zhang [arXiv:1106.0873v2](https://arxiv.org/pdf/1106.0873v2) `5 (5.3)–(5.6)・Theorem 5.1（pp.38–39）を一次資料で照合した。`ke:source-inclusive-fixed-shell` は同じ入力をsourceを含む固定compactへ適用する証明を本repo内に持ち、shell横断と全曲面ambient距離、同一frameと異なるframeの閉形式差を区別する。Total-space source $xy+tz=0$ のcanonical特異点、stable family、$K_{\mathbf P^2}+D=\mathcal O(d-4)$ のampleness、fixed-gauge収束を区別する。SNC上の $x^\nu C^\infty_{fc}$ remainderとradial cusp微分から固定endのmoment漸近を得ており、smooth divisor専用のfull polyhomogeneous expansionは使わない。本稿の新しいsource-arm tensor比較とscalar外側境界はこのcomponent収束を使わないが、core移送等の既存入力から除いたわけではない。

Complete simplex模型の存在はZhang [arXiv:1505.04728v2](https://arxiv.org/abs/1505.04728v2) Theorem 2.1・Proposition 2.2を一次資料で確認した。同Theorem 2.1が引用するCheng–Yau (1982), Theorem 4.4の原論文の証明そのものは今回再精読していない。Zhangの退化族に関するTheorem 2.4のQ-factorial仮定をsourceを持つ本族に適用してはいない。DMVのTheorem 1.2についても、固定Euclidean補助測度、正閉current、$L^2$ 規格化、周期coverの個数とBishop比較の実次元4を照合した。ただし現行の有界source退出はこのGaussian経路から独立である。

## Normal momentを保つ相対変更と五次の同時実現

`ke:moment-relative-replacement` と `ke:relative-replacement-gh` は、同じ保持cornerの全葉、sourceのcompact nodal neighborhoods、同じcanonical normal moment・anchor cuts、同じcomponent core領域を保つ相対変更に対し、基底値の差を
\[
\sup_x d_\square(f_{j,t}(x),\widehat f_{j,t}(x))
\le C\eta_{j,t},\qquad \eta_{j,t}=C(1+\log(N_j+1))/R_t
\]
で抑える。変更後のmarked Reeb productとcore coneの実際の商データ、全overlapのwhole-fiber一致は入力である。閉商を先に構成し、同じcorner inset・neck profile・小さいcore panelsでparameter化する。Reduced方向の変更をC1まで小さくする必要はなく、任意の指定変更を実現する定理ではない。これらの条件下ではGHの距離比較を引き継げる。五次では `ng8:quintic-full-moment` が初期source葉を選ぶことで所定targetの全moment実現と全open overlapsを与え、`ke:quintic-simultaneous-realization` がこの相対変更の条件を検証して同じ射影のatlas/GHを構成する。六次では `ke:petersen-full-moment` と `ke:sextic-simultaneous-realization` が等重み・初期source葉選択の下で同じ条件を満たす。先指定された追加保持集合への適用はstrict cutsを改めて確認する。

`ng8:fixed-fiber-relative-dh` は、各固定tのfree compact bandで、作用不変primitiveとaffineな境界作用からStokesによりtotal reduced areaのaffine性を得る。Reference constantsのt依存を許し、actual KE形式のt=0へのsmooth extensionを仮定しない。一方、重み(1,−1)の標準模型を \(I_1+I_2\le c\)、\(\mu=I_1-I_2\) で切ると、周期2π規約で \(\operatorname{Area}(P_\mu)=\pi(c-|\mu|)\) となる（`ng8:source-dh-wall`）。Source横断の全intervalへfree-bandのaffine性を流用できないことを示す局所模型であり、actual P0全体の面積公式ではない。相対Moserには端germsとmarked identificationsに加え、保持集合の補集合ごとの正の有限配分が必要である。補集合が分かれる場合、総量と個別marginだけでは足りない。


`ng8:componentwise-critical-area` は可動成分ごとの質量保存を正の有限配分行列と同値にし、`ng8:strict-area-cuts` がstrict Hall cutで判定する。`ng8:p0-small-area-flexibility` は、固定stage・固定tの小さいmoment intervalで、sourceのfull compact pinched torusを含む飽和annuliを保持した微小面積変更を実現する。`ke:actual-anchor-fan-criterion` と `ke:anchor-stokes-budget` は同じactual coreのanchor periodsからchartを構成する十分条件を与える。詳しい有限条件・規格化・障害と証明の所在は研究ノート「相対critical-areaの有限条件とactual source」「Actual coreの有限anchor period条件」を参照する。

`ke:raw-moment-error-insufficient` では、固定stageで \(\mu_t=-L_t^{-\alpha}\)、\(\nu_t=-L_t^{-\beta}\)、\(0<\alpha<\beta<1\) と取ると、\(|\mu_t-\nu_t|\to0\) でもlongitude差は \(\beta-\alpha\) へ向かう。近似matchingを用いる場合はnormal momentの絶対誤差でなく、profileを通した基底値差を制御する。

## 公表用比較とactual計量の区別

**既存GH定理との比較：** Fernández de Bobadilla–Pełkaの [Proposition 6.13・Theorem 6.14](https://arxiv.org/html/2312.13248v4) は、部分Lagrangian fibrationに加え、properな族の全nearby fiberについて補助Kähler計量のGH収束と深度座標による明示的近似写像を与える。本稿の対象は、actual負KE形式でのcoreを含む全域π_tと同じp_Tπ_tによる全ambient距離比較、および五次/六次の指定範囲での作用atlasの同時実現である。FBPの補助形式のparameter qと、本稿のactual形式を固定したstage/cutsを区別する。標準flat三角形の双対複体とunit-square targetは位相的には同じでも、曲面点の接錐角2πと3π/2により定数倍を許しても等長でない。詳細は主稿 `intro:dual-complex-metric-scope`。

Zhang Theorem 2.4(i)の元の尺度のpointed GHには基点・部分列の選択があるが、(ii)の局所semi-flat比較は全parameterで成立する。Part IVの固定模型に使うTheorem 2.1とは別の定理であり、source全空間へ退化定理を直接適用しない。


Fernández de Bobadilla–Pełka, arXiv:2312.13248v4 の Theorem 6.14、Example 5.8、Introduction、Remarks 5.9・7.4を一次HTMLで照合した。境界・角付き部分領域のivy-like fibrationと、properなら全nearby fiberについての構成Kähler計量のGH収束を扱う。Remark 5.9の作用座標はramificationとouter boundaryを除く領域であり、branch/coreを跨ぐ本稿のatlasと区別する。Evans–Mauri Remarks 2.11–2.12のLiouville同次性も既知原理として直接引用する。本稿の全域core fillingとactual負KE距離の評価への依存入力としては使わない。Fu–Hein–Jiang, GAFA 35 (2025), 542–632, DOI 10.1007/s00039-025-00708-y の掲載版 §1.1 Main Theoremを確認し、孤立楕円特異点を持つ具体的sexticのactual負KE cusp閉鎖・Tian–Yau bubbleという範囲をIntroductionで比較した。両者の全証明の再監査ではない。

同一classのMoser同値 $\phi_t^*\omega'_t=\omega_t$ だけでは、$\phi_t^*g'_t=\omega_t(\cdot,\phi_t^*J\cdot)$ と $g_t=\omega_t(\cdot,J\cdot)$ の差を評価できない。Actual距離の結論には本稿の小さい局所移送とscalar/portal評価が必要である。

## 内部点検済みの範囲と残る確認

- 五次同時実現から逆向きに、全K2 period、source wallの滑らかな自由需要、Diniによる初期thin tails、成分別relative Moserと最後の点固定補正、全開germs、作用格子の平行移動付き三面延長を独立点検した。旧free-neck補題をsource-inclusive帯へ用いないことも全逆参照で確認した。固定reference葉からの変更はmoment非依存の $H_{r,t}$ を合成して扱い、source点/saddle点の局所固定、K2/core supports、marked product、whole-domain connectorsが葉の微分又はthin幅に依存する新たな閾値を要求しないことを照合した。主要式は `ke:eq:quintic-affine-full-transition`、選択順序は `ng8:quintic-full-moment` 末尾。全旧P0証明・全外部解析の再認証ではない。

- Core正則化→固定actual形式へのexact Moser→actual作用での平均→同じmoment link→相対葉族→全域fibrationの接続について、支持・量化・構成の同一性に限定した独立内部監査を完了した。恒等end collarsは全K2交わりを含み、全fiber trimは補間後partitionに適用する。元のcoreと内側平行linkの共通collarで一致し、被覆を保つ。SNC構成にも閉isotropic filtrationを明示した。`ke:contact-rescaling-collar-scope` の反例は固定contact formとcontact構造だけの一致を区別する。

- 有限cutのclosed-corner定理と、全target端点のportal選択、$\mu=0,\pm\delta$ のtori、全fiber合併、六label galleryの費用を独立点検した。Raw/actual momentとtail bufferの選択、固定anchor点、ambient端点比較の適用を明記した。
- 共通anchorでの全保持neckの正確なmoment区間、全domainを含むcap/core分割、core境界のfirst-exit、marked graphの明示自明化を独立点検した。同一momentのcorner参照torus、有限cutに一様なMoser被覆・接続・中央帯と、全域値比較の非循環性も確認した。Cornerの座標補間・全平均・相対Hamiltonianの定数とcutoffsが段階一様であることを照合し、残余接続費用のcutへの吸収から上下両側の固定族係数を得た。
- Source中心のsmooth centered Moser、canonical momentの零、位相商、閉pinched torus、primitive cycleとfocus二次型を独立に点検した。K2のfirst-exit→逆flow→moment→全torusの順序、inverse Morse領域と非incident piecesの分離、全stageと全複素parameterでの固定marked treeも再点検した。
- K2–K3の接続に必要な全intersection saturation、fixed-stage stratum coverage、whole-fiber trim、actual Lagrangian性、compact Hausdorff quotientへの全射とconnected fibers、固定 $d\ge5$ の範囲、core・変更collarの固定compact費用を点検した。
- 新しい中央 $O(1)$ 径、全moment source退出、sharp scalar barrier、global physical-depth補正とactive cover、全域co-Gramと $\Theta_t$–$f_t$ 比較、共通moment portals、全fiber合併、有限gallery上下界を、作成担当以外の読み手が内部点検した。特に全境界、source軸、同じcanonical moment、依存の非循環性、固定段階から遅い対角選択への順序を照合した。
- YauのTheorems 1–2、Savinのsmall perturbation、Songのfixed-gauge収束、DMVの掲載版Theorem 1.2、Rochon–ZhangのSNCに関する指定箇所は一次資料で確認した。外部KE原稿の全証明や旧主稿全体の独立再監査、公表前の網羅的な先行研究・新規性調査、形式証明を完了したという意味ではない。
- 解析証明の数学的点検、保存された有限有理数検算、その再実行、組版、GitHubへの反映は別の確認である。各実行状態は現行の検証資料を参照し、本書の「証明あり」を計算・組版による証明の検証と読み替えない。

**曲面主稿改訂47の検証（2026-11-23）。** Part IVの固定座標・模型に関する局所安定性率の最適性を引用し、指定証明と入力を独立に点検した。Zhang・Ruanの指定一次箇所を実読し、導入の比較範囲は別担当も確認した。LuaLaTeX/latexmkで324頁に組版し、主要log六分類は全て0。1・18–20・323–324頁の6頁を150dpiで実表示し、追加段落・隣接する改頁・関連書誌に欠字・重なり・切断・数式/URLの溢れを認めない。PDF/source hashと確認担当は検証JSONに記す。既存FBP・simplex・source・輸送・core・atlasの指定点検は保持し、一律に再実施したとはしない。全324頁の逐頁検査、全証明・全外部入力の再監査、外部査読、形式証明、包括的新規性確認ではない。静的構成検査は通過し、既存整数証明書は今回再実行していない。

研究資料v3.35・依存表v3.24、主稿改訂47。Part IV v1.15の `simplex:prop:boundary-floor-sharpness` を短く引用し、固定depth coordinates・比較模型k_Lに関する局所仮定クラスでのO(1/m)の最適性を明記した。Actual compact射影的族の誤差下界やfacet shift補正後の最適性は主張しない。Zhangの固定normalized compactと全phase、Ruanの固定縮小polytope上の定量的なtorus平均比較を一次本文で確認し、指定canonical simplexへの全深度比一様な小誤差を局所解析の比較点とした。FBPの明示GH近似・補助Kähler計量とactual射影の比較、cubical/flat simplicial計量の非homothety、既存のsource・輸送・core・atlasの指定点検を保持する。現行組版と実表示の実施範囲は検証JSONに記す。

## 再開時の確認

Sourceのfocus判定・全飽和近傍の移送と、nodal blow-upの面積・支持・選択順序を本文に明示し、必要箇所を内部点検した。有限閉whole-fiber quotient、同じ合成写像の連結fibers、fiber Euler関数の有限支持とcoarse fiberのEuler公式を本文に整理した。一般存在・P0・作用atlasの量化を分けて点検した。次は公表前監査を続け、Introduction・主定理のscopeを全域構成から逆向きに照合する。五次では初期source葉を選ぶ全moment実現から全域atlasを構成し、上の相対変更命題で同じ射影のGHを得る。六次の等重みでは内部二端cutsをbalanced separator・中央freezeで満たし、全momentと両端の全open germsを構成済みである。先指定した追加保持集合のcritical-area条件は独立に調べる。無限個のbranch fibersと有限個のbranch strata、πのLagrangian fibersと合成写像のfiber合併を区別する。既存P0の範囲と優先順位を保ち、任意のfocus不変量への先指定を追加しない。外部repoの最新 `main`、AGENTSと方針を確認し、上表のラベルの存在と追加仮定を照合する。未取得・アクセス不能なら、確認済みコミットと未確認範囲を残し、利用可能な独立課題を進める。解析的結果を外部repoへ追加した場合は、そちらを先に保存してから、この表の参照版と本repoの依存箇所を更新する。外部入力の更新・本repoでの適用証明・組版・計算検証は別々に記録する。

## 確認した現行ソースの保存版

2026-11-23に現行本文と今回の追加証明を確認した保存版は次のとおり。既存の対象限定監査と今回の実読・実行を区別し、mainが進んだ場合はこの版との差分を確認する。

| 正本 | 確認した保存版 | 数学・組版の範囲 |
| --- | --- | --- |
| multiscale-kaehler-einstein | [2926300](https://github.com/uedakazushi/multiscale-kaehler-einstein/tree/2926300c2425c7e68550ac08ee81a2afa639a0c6) | Part I v1.10・総説v1.14・研究資料v1.19。固定cutoffの体積・Stokes予算を追加し、別担当も実読。I73頁、指定5頁を150dpi表示、主要log六分類0。総説22頁とII–IIIの既存記録は維持し再実行なし。 |
| kaehler-einstein-degeneration | [1ee0aca](https://github.com/uedakazushi/kaehler-einstein-degeneration/tree/1ee0acaf876b1334c964d60c409feb3b18b62373) | Part IV v1.15・V v1.10・研究資料v1.28。局所boundary-floor仮定クラスでの固定座標・模型に関する率の最適性を独立点検。正本担当がIV126頁・指定9頁の150dpi実表示・log六分類0を確認。既存simplex/解析入力の科学pinと点検範囲、Vと証明書は保持。 |
