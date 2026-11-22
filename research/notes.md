# 現行研究ノート：一般型曲面のLagrangian torus fibration
更新：2026-11-22 / v3.28（主稿改訂43）

主稿 `papers/surface-lagrangian-torus-fibration.tex` と整数接着 `papers/quintic-integer-gluing.tex` を正本とする。以下は曲面・KE局所幾何・作用・アフィン接着に関する現在有効なノート。三次元の原稿と相対円板群・補集合の計算は [threefold-lagrangian-torus-fibration](https://github.com/uedakazushi/threefold-lagrangian-torus-fibration) を正本とし、こちらに重複保持しない。

**現行の到達点（改訂43・公表準備）。** 各固定次数d≥5の同じactual負KE–Lagrangian射影による全域GH実現に、確率KE体積の極限を統合した（`ke:global-volume-measure`）。同じf_tの押出しは成分頂点の等重み原子測度、π_tの押出しは固定B_d(T)のcore頂点の等重み原子測度へ弱収束する。固定成分compact上の値比較、対数的Chern–Weil公式と全体積の一致から、既存の対角選択のまま質量の取りこぼしがないことを示す。全cubical距離と有限な測度の台、確率体積と未正規化のrescaled体積を区別する。五次の同じ射影の作用atlas/GH同時実現も保持し、この測度結論が適用される。六次の同時atlas、任意先指定大source近傍、atlasのparameter極限・Hessian性は未解決である。指定証明の内部点検と全主稿再監査・外部査読・形式証明・包括的新規性確認を区別する。

## 同じ射影のKE体積極限

正本は `ke_global_metric_realization.tex` の `ke:global-volume-measure` と `ke:global-volume-scope`。Ric(ω)=−ω、dV=ω²/2 の規約で、各成分の体積は2π²(d−4)²、全体積はそのd倍である。Part I `lem:CW`・`thm:facemass` の直接Stokes公式と、Song Theorem 1.2(4)の既知の体積保存を区別して引用する。

固定K_i⊂W_iのgraph像では非成分深度が有界、成分深度はL_t−O(1)以上なので、既存のclipped mapが最終的に厳密にe_iとなる。全域値比較から同じf_tの像がe_iへ一様収束し、固定compactの体積収束とexhaustionで残部質量を任意に小さくできる。Moving coreへの包含、新しい対角選択、neckの一様体積漸近は不要。p_T^{-1}(e_i)={v_i}とcompactnessからπ_t版も全d≥5に成立する。五次atlas版は一様値比較で移る。

確率測度の極限は有限な頂点集合を台とするが、GH極限の全square/edgeの距離は保持する。Rescaled metricの未正規化体積はR_t^{-4}倍なので零測度へ行く。Full-supportを要求しない測度付きGHの意味を本文に明示した。体積保存・exhaustion原理自体の新規性は主張せず、同じactual射影の位置と重みを同定した帰結とする。

## 公表原稿の読み方と五次anchorの有限判定

主定理 `ke:global-realization` を一般設定の直後に置き、`ke:proof-inputs`、`ke:proof-route`、`ke:cut-selection-order` から最短の証明経路を読む。長い技術的概説は証明本体への案内へ整理したが、既存の定理・証明ラベルと引用を保持し、統合定理の証明・帰結は変えていない。

五次の一つのactual coreでは各normal faceはpair of pantsであり、internal regionがない。`ke:k4-protected-anchor-selection` は、同じmeridian framingとclutching、固定保持集合・marked relative orbitの下で、所定targetsを次の正確な有限条件へ帰着する。Normal periodを $M_a<0$、puncture periodを $c_{ab}$、critical leaf側に最も近い保持annulusのcritical leaf側の境界からpunctureまでの全tail面積を $L_{ab}$ とし、$Q_{ab}=c_{ab}+L_{ab}$ と置く。Tailには保持annulus自身とその向こうに隔離された自由部分も含む。内部annulusがなければend collarを使う。

指定successor $b=f(a)$ の実現は $Q_{ab}<-M_a$ と、他の二つの $Q_{ac}<0$ に同値である。全 $Q_{ab}<0$ なら全successorsを許し、非負値が一つだけでそれが $-M_a$ 未満ならそのsuccessorが強制され、残りの場合は不可。四面の許容集合が非空のとき、forced arrowsの終点が互いに異なり長さ2・3のcycleがないことが、一つの有向四角形へ延長できるための必要十分条件である。既に4-cycleなら許される。証明は主稿に置き、ここには複製しない。

この有限組合せ部分は、各面が「自由」又は他の三頂点の一つを強制する全 $4^4=256$ patternsについて、六つの有向四角形の直接列挙と照合した（可解79、相違0）。数学的根拠は本文のpath componentsを巡回連結する証明であり、この計算は独立な小規模検算である。Actual KEのperiodを数値計算したものではない。

### 標準P0のactual anchorへの適用

`ke:k4-actual-end-anchor` は、全K2 end collarsだけをanchor上で保持する標準選択に対し、有限判定の入力を実際に検証する。正weightsの和は1、$\rho_a=2\pi w_a$ を固定する。Source torus label $B=\theta b_j$、$5.4<\theta<5.5$ の葉を保持collarの最内境界に取る。広いconstruction domain $\min\ell>3b_j$ と、$5b_j<B<9b_j$ の共通end葉族を使うため、retained corner cut $6b_j$ より浅いことは障害にならない。

厳密なmeridian規格化と二深度比に一様な評価から $Q_{ab}=\nu_b-\rho_b=-\rho_b+O(b_j^{-1})<-\rho_b/2$ を得る。選択順は正の $\rho$ → 大きい $j$ → $N$ → 小さい $t$ で、残余compact定数をcorner誤差へ掛けない。$\mathcal O(1)$ のsectionを一punctureで単純零点に取るclutching計算と、既存graph/averaging/Hamiltonian isotopiesにより、同じactual cyclesで $\sum_b\beta_{ab}=-\alpha_a$ を確認する。全六つの有向四角形が許容され、同じLiouville domain・primitive・skeletonから局所K4作用chartを得る。詳細な証明は本文を正本とする。

面積指定は元のmarked relative isotopy class内で行う。補助Moser primitiveへのcompact supportのexact補正で有限marked source点のfirst jetsを零にして、それらをisotopy全体で固定する。Sourceのfull compact nodal fibersの飽和近傍は $\delta=4\pi/N$ の決定後、$|\mu|<\delta/2$ に選び、anchor変更の支持 $|q_a-\delta|<\delta/4$ と離す。大きいanchor変更は全relative isotopyのmoment cutoffで先に組み込み、同じanchorを持つ二族となってから既存small interpolationを使う。全K2 end/cornerの開overlapで同じ全葉を保つ。

この局所系単独を全域atlasへ読み替えない。全neck intervalと両端の作用整合は以下の有限endpoint条件と全moment実現で別に証明する。既指定の大きいsource近傍・追加anchor保持annuliへの適用には引き続きstrict cutsの確認が必要である。

### 五次の両端actual periodsと有限接着条件

正本は `ke:k4-actual-neck-periods`、`ke:k4-equal-weight-periods`、`ke:k4-cyclic-weight-periods`。各componentの正weightsを $\sum_{j\ne i}w_{i,j}=1$、$\rho_{i,j}=2\pi w_{i,j}$、$x_{i;jk}=\mathbf1_{k=f_i(j)}$ とする。同じneck primitiveとactual meridiansで、両端のclosed差は $\kappa_{i;k}=\chi_{ij;k}+\rho_{i,k}$、$\kappa_{j;k}=\chi_{ij;k}+\rho_{j,k}$。Normal periodの零とK2 torusの整数relationから共通の $\chi$ を得る。Component側のclosed差へclutchingを積分すると $\sum_k\chi_{ij;k}=-2\pi$ であり、非閉primitive自体へhomologyを適用してはいない。

Actual smoothingのwindingをsource-inclusiveな有限tのnormal formで計算すると $\beta_{j;k}=\beta_{i;k}+(n_{ij;k}-1)\alpha$ となる。従って両端affine germsが整合する必要十分条件は
\[
 n_{ij;k}=1+x_{i;jk}+x_{j;ik},\qquad
 \rho_{i,k}+x_{i;jk}\rho_{i,j}=\rho_{j,k}+x_{j;ik}\rho_{j,i}.
\]
各二重線の実数切片差の和は零で、独立な実条件は高々二つ。未知のfinite-t primitive定数は両側で相殺し、exact補正やsource shearによって切片の不一致を修復する必要も自由もない。

全weightsが1/4なら、切片条件は $f_i(j)=f_j(i)$ と同値であり、既存の六つの対称四角形系とsource配分(3,1,1)になる。異なるallocationを固定済みのrelative orbitへこの配分を無条件に移さない。非等重みには、五角形successor $s$ と正の $\sum a_i=1$ を用い、$f_i$を$i$削除後の四角形、$w_{i,j}=a_j+a_i\mathbf1_{j=s(i)}$ とする明示解がある。隣接pairでは(3,1,1)、非隣接pairでは(2,2,1)。これは正weights全解の分類ではない。

これらのprimitive比較・closed差の総和・smoothing winding・有限係数比較・非対称例を担当と別担当が読んで点検した。両端条件だけでは全域を結論せず、次節の面積実現と全葉接着を組み合わせる。

## 五次の全moment実現と同じ射影のatlas/GH

証明の正本は `ng8:uniform-k2-end-periods`、`ng8:thin-source-tail-choice`、`ng8:quintic-full-moment`、`ke:quintic-simultaneous-realization`。入口の系は `ke:quintic-simultaneous-main`。同じcanonical neck primitive、normal moment、固定K2全葉・anchor cuts・core領域を使う。

各二重線の三basinsについて、K2 end actionを $R_k(\mu)=\chi_k+\nu_k(\mu)$ と書く。全深部triple評価、同じlogarithmic primitiveのpullback、centered averagingとexact transportから、sourceを跨ぐ全共通intervalで $|\nu_k(\mu)|\le C/b_r$。保持end collarの面積も $2C/b_r$ 以下になる。任意の二深度比を許し、非正則pullbackから別の $d^c$ primitiveを作り直さない。

指定affine actionを $J_{i;k}=\chi_k+\rho_{i,k}+x_{i;jk}\rho_{i,j}-x_{i;jk}\mu$ とすると、actual target面積は
\[
a_k^{\mathrm{tar}}(\mu)
=\rho_{i,k}+x_{i;jk}\rho_{i,j}-x_{i;jk}\mu
-\nu_k(\mu)+n_{ij;k}\min(\mu,0).
\]
Critical側のshearは $n_{ij;k}-1$、end側は $-1$ なので、負側の差は $n_{ij;k}\mu$。同じStokes計算で
\[
\operatorname{Area}(P_\mu)=-\sum_kR_k(\mu)-\mu+5\min(\mu,0)
=\sum_k a_k^{\mathrm{tar}}(\mu)
\]
となる。Sourceの固定点を跨ぐ全量をaffineと仮定しない。最小residue $\rho_*>0$ を先に固定し、$C/b_r<\rho_*/16$、$\delta<\rho_*/32$ とすれば拡張区間 $|\mu|\le2\delta$ で各targetは $\rho_*/2$ より大きい。

初期source allocation・順序・marked relative classを固定した三つのrooted treesを同じ残余pants内に選ぶ。各rootは対応end collar、各sourceは割り当てたtreeに載る。Thin neighborhoodsの質量から固定end massを引いた差が全momentで零へ一様収束することを、sourceの可積分reduced density、Darboux-ball分割とDiniの定理で証明する。非原子性だけからgraphの面積零を推論しない。全tailを $\rho_*/4$ 未満にした後で、sourceを通る初期regular circlesと中央の全nodal neighborhoodsを固定する。既固定の大きいtailをannulusの幅だけで縮める主張ではない。

Pantsにはinternal regionがなく、ordered-source cutsは各targetが対応全tailを上回る条件になる。Targetと保護質量に同じsource wallがあるので、その差は滑らか。自由部分の成分別relative density-Moserで全momentのcritical actionsを実現する。Coreへの通常のmarked interpolationの後、sourceを含まないanchor帯でも同じtargetへ相対面積補正を施す。両open germsは既に正しい面積を持つので補正はそこで恒等。有限source sectionsのfirst jetsを消すexact補正が、source配分・framingを保つ。中央の全nodal neighborhoodsは支持外である。

自由需要の滑らかさは、保護質量を $\kappa_k=K_k-n_k|\mu|/2$ と書くと直接見える：
\[
a_k^{\mathrm{tar}}-\kappa_k
=\rho_{i,k}+x_k\rho_{i,j}+(n_k/2-x_k)\mu-\nu_k-K_k.
\]
中央自由成分への三需要は $a_k^{\mathrm{tar}}-L_k>0$、tail内に隔離された自由成分への需要は元の全質量である。保護annuliを除いた補集合が連結であるとは仮定しない。最後のanchor帯は $\mu\ne0$ なので保護集合をK2 endsだけにでき、点固定のfirst-jet補正は追加の面積条件を作らない。旧 `ng8:relative-dh` と `ng8:straight-neck` はnodal neighborhoodsを避けた自由neck専用であり、このsource-inclusive証明は全Stokes式とwall項を用いる。

解析領域 $P_r$、cutoffs、$N_r$ と全小複素 $t$ の閾値は、thin widthsと葉の選択より先に固定する。同一momentのconnectorは領域全体に対する評価なので葉の微分上界を要しない。同じ初期thin葉族から通常P0と作用指定版をそれぞれ構成し、中央の全nodal neighborhoodsとK2全葉を共通に保つ。各normal/corner/core cutが新しい全葉でも飽和することを確認し、閉Hausdorff quotientと全open overlapsを貼る。Period 1の未除算作用は全chartで一斉に $2\pi$ で割り、既存atlasの規約と合わせる。共通normal actionの原始性とstar transitionsを確認して分母1の全域atlasを得る。

固定reference foliationからthin代表への同定 $H_{r,t}$ はmomentに依存せず、既存の $D_{r,\mu,t}\circ S_t$ の前へ合成できる。$S_t$ は先に固定したsource discsから定まり、新annuliを集合として保つ必要はない。Source・saddle点の小近傍をend補正の支持から離し、その遠方の全円葉は像として運ぶ。Core primitive・支持・domainも先に確定できる。Marked productと基底値比較はこの同定の微分を使わず、thin幅に依存する追加の小parameter条件は不要である。

全平行移動を含む接続は `ke:eq:quintic-branch-action-coordinates`、`ke:eq:quintic-core-branch-extension`、`ke:eq:quintic-affine-full-transition` に明記した。正規化した共通normal actionを $h$、各core face座標を $(s,\zeta)$、$(s',\zeta')$ とすると
\[
\zeta'=\zeta,\qquad s'=-s+(y_k+y'_k)\zeta+w_{i,j}+w_{j,i},
\]
ここで $y_k=\mathbf1_{f_i(k)=j}$、$y'_k=\mathbf1_{f_j(k)=i}$。三面の平行移動が共通で、各四角形のpredecessorの一意性がK4格子の関係を保つ。非対称weightsにも適用できる。これは既に全open collarsで一致する実際の葉と作用を入力し、整数行列だけで葉を接着する主張ではない。

同じmarked $T$、同じmomentで比較するので、`ke:moment-relative-replacement` の値差は $C(1+\log(N_r+1))/R_t$ 以下。既存P0のdistortionと合わせ、同じ新射影の全域GH・全coarse fiber収縮を得る。$t$ に滑らかな葉族、任意の先指定source近傍、最適rateや六次の同時実現は含まない。新証明とatlas/GHへの指定接続を複数担当が内部点検した。全既存主稿の再認証・形式証明・外部査読とは区別する。

同時実現は各 $t$ の同じ射影の性質である。作用atlasのparameter極限、固定基底上の極限integral affine構造、$d_\square$ の作用座標でのHessian性・Monge–Ampère性は未証明であり、SYZ型の比較で暗黙に追加しない。

## 固定成分の漸近錐とactual曲面の中間尺度

三研究の共同編集・監査は [研究方針](../00_research_plan.md) と [依存表](ke-dependencies.md) の責任分担に従う。固定補空間の正本はmultiscale、退化族の局所解析はKE-degeneration、actual fibrationと直接大域評価は本repoとする。

$H_i=\{L_i=0\}$、$D_i=\bigcup_{k\ne i}(H_i\cap H_k)$ とすると、$U_i=H_i\setminus D_i$ は $\mathbb P^2$ から一般位置の $d-1$ 直線を除いたもの、$K_{H_i}+D_i=(d-4)H$ である。Part I `cor:arrangement-cone` の $(n,m)=(2,d-1)$ に対応する錐は $C_{2,d-1}=\{u\ge0:|\operatorname{supp}u|\le2\}$、各quadrantはunit Euclideanである。

固定 $U_i$ にはPart I v1.7の `thm:contract`, `thm:rough`, `cor:based-ball-approximation` により、properな1-Lipschitz全射 $\mathcal S_i:U_i\to C_{2,d-1}$ と有限定数 $K_i$ を取れる。一度この写像と定数を固定すると、任意の $o\in U_i$、$A,R>0$ に対し
\[
d_{\mathrm{GH}}\!\left(
\overline B_{(U_i,R^{-1}d_{\mathrm{KE},i})}(o,A),
\overline B_{C_{2,d-1}}(R^{-1}\mathcal S_i(o),A)
\right)\le\frac{3K_i}{2R}.
\]
両球にはambient距離を制限する。指定compactを錐の原点へ送るように選べるが、その選択では $K_i$ がcompactに依存する。この定量評価は固定空間の空間的blow-downであり、退化族のmoving領域へ一様に適用するための新しい入力ではない。

Part I `def:incidence-link`・`lem:positive-star-product` は、面copy $\alpha$ を保つincidencesだけで残余cone $\mathcal L_\alpha$ を貼り、全ての $\alpha$ 座標が正の領域を $Q_\alpha^\circ\times\mathcal L_\alpha$ と同定する。閉star全体のambient距離は一般に積距離ではなく、face copiesを潰すと単射性も失われる。`lem:star-ball-isometry` は $m_\alpha=\min_{i\in\alpha}\sqrt{c_i}a_i>2A$ の下で、半径 $A$ のambient閉球を積空間の閉球と厳密に同定する。外へ出る経路の下界 $2(m_\alpha-A)>2A$ が、最短路の近道を排除する。`prop:cone-limits`・`cor:moving-limit-classification` はこの評価から、有限位置の錐と $(\mathbb R^{|\alpha|}_{\boldsymbol c}\times\mathcal L_\alpha,(0,z))$ を全ての部分列極限として分類し、全射性により任意のscaling sequenceで各型を実現する。分類の表現の一意性は主張しない。定理文と構成を読み、担当・主担当による指定証明の共同点検結果を同期した。証明と閉starの障害例はPart Iを正本とする。

`lem:cone-link-metric`・`prop:link` は曲面側担当も独立に点検した。Linkの別成分間では $d_\Sigma^{\rm len}=+\infty$ とし、$\bar d_\Sigma=\min(\pi,d_\Sigma^{\rm len})$ を用いる。Coneの等半径距離は $2r\sin(\bar d_\Sigma/2)$、coarse sectionの誤差が $A_s$ ならradial divergenceの誤差は全方向に一様に $(K+2A_s)/r$ である。$\bar d_\Sigma$ のpath metricは元のextended length metricを回復し、cone pointを保つ等長写像はこの計量を保つ。CAT(0)性は必要ない。回収するのは等長型であり、cell subdivision・component名・normal-depthの重みではない。実際、$v_i=\sqrt{c_i}u_i$ は全faceで整合する等長な座標変更である。Coarse sectionのfamiliesをgenuine geodesic raysと同一視せず、全rough raysのbounded-distance商も主張しない。曲面側の成分label $i$ は構成の標識であり、これを無標識の計量から回収する必要はない。固定空間のmoving/link定理は `ke:intermediate-component-cone` の入力ではなく、同系の $R_t(\epsilon_t+\eta_t)=o(a_t)$ を除くものではない。

同じPart Iでは、`lem:deep-sector-partition`・`lem:cellwise-LDP`・`lem:exp-tight` からambient open集合に対するLDPを証明し、`lem:level` から `thm:tail`・`thm:joint`・`cor:Laplace` への鎖も対象を限定して点検した。現行の測度論では、全faceのordinary volume-IRFAから得るactual conditional residual measuresの一様subcritical momentsを用い、残余距離の単位shellの質量を指数的に抑える。一面normal depthの積分と狭いvertex sectorの下界を組み合わせて `lem:vertex-tightness` が閉じるので、metric-IRFAと全faceのordinary volume-IRFAでexact tail/joint/Laplaceが成立する。Volume error自身の指数的減衰は追加仮定しない。最小減衰率のcuspだけで混合重みを正規化する点は保つ。この強化は測度論担当と主担当の共同点検結果を同期したものであり、曲面側の今回の独立監査範囲には加えない。これらの測度結果は本稿のscalar/portal比較やsource Gaussian tailの新規入力ではない。証明と詳細な検証状態はPart Iを正本とし、確認commitは [依存表](ke-dependencies.md) に置く。

**測度と基点の規約。** `thm:intro-measure` のLDPは $\mu/\mu(X)$ を用いるが、KE face translationと交点数係数には非正規化 $\mu=dV_g$ を用いる。Full collarの $\mu_F=\chi_F\mu$ と $\Pi_T=(t_I-T,\pi_F)$ を明示し、normal torusを積分済みの $\lambda_F$ へ収束させる。確率測度を使う場合には $\lambda_F,\mathfrak m_F$ をともに $\mu(X)$ で割る。これらの面質量は確率分割ではなく、その総和を1とする主張ではない。非空のnormal集合とconnected faceを固定し、strip TVにはordinary volume-IRFA、球のpmGH/TVにはmetric-IRFAと有限のnormal offset・残余基点の収束を使う。Boundaryが空の場合もLDPとtotal volume formulaは成立するが、非自明なtail/joint/Laplaceの臨界公式は非空境界と固定基点について述べる。Introductionと本文の仮定・測度・定義域を独立に照合し、純測度のcutoff選択から不要なco-Gram定数への依存を除いた。

Part I v1.7の `thm:translation` はordinary volume-IRFAを用い、任意の $\min_iT_i\to\infty$ に対して、$t_I-T_I$ とresidual射影による押出し測度を $e^{\sum_iT_i}$ 倍すると、$e^{-\sum_i s_i}\,ds_I\otimes\lambda_F$ へ収束することを示す。固定strip $[-A,A]^I$ と全residual spaceの積の上で全変動誤差を評価する。Metric-IRFAとcentered offsets・residual基点の収束を加えれば、各固定半径のambient閉球の押出し測度も全変動収束し、pointed measured GH収束を得る。Ball制限ではnormal Euclidean sliceにより全ての正の半径の球面が極限測度零となる。測度側にsmooth volume-IRFAを追加する必要はない。曲面側では定理文を照合し、証明の共同点検結果を同期しており、今回独立に全鎖を再監査したとはしない。

同版の `lem:CW`・`thm:facemass`・`app:CW` は曲面側担当が直接点検した。規約は $dd^c=i\partial\bar\partial$、$\Theta=iF_h$、$[\Theta/(2\pi)]=c_1(L)$、$dV_g=\omega^m/m!$。Rochon–Zhangの背景形から $\omega_{\mathrm{KE}}=\Theta+dd^c\psi$、$\psi=u-2\sum_i\log q_i$、$q_i=-\log(\varepsilon\|s_i\|^2)$ と書ける。$\psi$ 自体は非有界でも $d^c\psi$ はcusp normで有界であり、有限体積と一様に勾配が有界なcutoffだけでStokesの境界項が消える。一般good metricとのbounded potentialやexact tailを仮定しない。法方向の周期 $2\pi$ とadjunctionから $\mathfrak m_F=(2\pi)^k\operatorname{vol}(F^\circ,g_F)$ を得る。この $2\pi$ はPart Iの角度座標の周期であり、本稿のperiod-1 normal generatorの規約を変更するものではない。一次資料の確認箇所とMumfordへの依存を外した理由は依存表へ置き、証明全文はPart Iに保持する。

Abel–Mellin側は `lem:Mellin-conditional-moments`・`lem:Mellin-weighted-TV`・`thm:Mellin-recursion` の共同点検結果を同期する。必要なのは一面だけでなく全deeper faceに整合したordinary volume-IRFAであり、固定normal depthsでのactual conditional residual measuresの全subcritical momentsを一様に抑える。一般Borel densityではdepthsに関するessential supremumを用いる。Unweighted全変動収束とこのmoment上界を組み合わせるので、選んだerror dominator $b_F$ のweighted可積分性は追加仮定しない。残余parametersの一様性はcritical boundaryから離したcompact集合上の主張であり、全parametersをcritical boundaryへ動かす一様極限と混同しない。`prop:Mellin-incidence` はcomponent別cutoffを持つmixed transformのAbel係数から $G\subset F$ を検出する。個々の面質量の数値だけからincidenceを回収する主張ではない。証明と有効な反例はmultiscale側に一元化し、本稿のactual族に新しい測度極限や解析仮定を追加しない。

**Abel係数と有理型延長。** Part I `ex:Abel-not-meromorphic` は、深さ1のexact cuspに抽象有限測度 $d\mu=(2\pi)^{-1}e^{-t}(1+1/t)\,dt\,d\theta$ を与える。残余質量は1、ordinary volume-IRFAの誤差は $1/t$ だが、$\varepsilon=1-s\downarrow0$ で $M(1-\varepsilon)=\varepsilon^{-1}+\log(1/\varepsilon)+O(1)$ となる。Abel極限 $\varepsilon M\to1$ があってもsimple poleを除いた残りが非有界なので、$s=1$の近傍へのmeromorphic continuationはない。この初等例を独立に点検した。KE体積そのものの反例ではない。`rem:Mellin-continuation` の残余 $L^1$ coefficient/remainder評価を持つjoint polyhomogeneityと、fixed compact subcritical parameters上の一様Abel recursionを区別する。

**残余periodの標識と向き。** Part II `prop:partI-translation` のcurve factorsは、component-labelled collarとdeeper facesからfactor/cusp labelsを伴う。`thm:intro-star`・`thm:star-chart` の配置復元にはKähler orientationも保つ。`thm:intro-unoriented`・`thm:unoriented` はfactor/cusp labelsを保持し、全curve factorsを用いるgeneric結果であり、向きだけを忘れたdataからprojective equivalenceと全体複素共役まで復元する。部分的なperiod集合や無標識のmetricに同じ結論を移さない。曲面側では該当定理文・定義を照合した範囲であり、Part IIの全proof再監査ではない。これらの複素・双曲periodは本稿の第二作用periodとは別のdataである。

**既存のIgusa積分との比較。** Chambert-Loir–Tschinkelのresidue measures・Clemens complex・Mellin主要係数とheight-ball測度の極限を、先行する一般原理として扱う。Part Iは対数深さ $t_i=\log(-\log\rho_i)$ とordinary recursive $L^1$ 入力、residual KE measures、actual metric-ball tailのBusemann phaseを接続する。Algebraic height ballsとactual距離球は同じ集合族ではない。指定一次箇所を確認した文献担当の結果を同期し、書誌・確認範囲は依存表、詳細な比較はmultiscale側を正本とする。網羅的な新規性確認とはしない。

主稿 `topo:component-cone-germ` は、$0<r<1/2$ の閉球で $u\mapsto e_i+u$ がこの錐と全cubical target $(\mathcal C_d,d_\square)$ の厳密な等長を与えることを証明する。Starを出る経路は別の座標が1となるgateを二度通るため長さが $2(1-r)>2r$、star内の錐では半径 $r$ への動径射影が非伸長である。従って固定成分の無限遠錐は、compact極限の成分頂点のmetric tangent coneとlabel付きで一致する。これは有限複体の距離に関する命題であり、単独ではactual族の一様解析を与えない。

さらに `ke:intermediate-component-cone` はP0の同じ全射 $f_t$ の歪み $\epsilon_t$ を用い、$x_{i,t}\in f_t^{-1}(e_i)$、$a_t\to\infty$、$a_t/R_t\to0$、$R_t\epsilon_t/a_t\to0$ のとき $(X_t,a_t^{-1}d_{g_t},x_{i,t})\to(C_{2,d-1},0)$ を証明する。$a_t=R_t\sqrt{\epsilon_t+R_t^{-1}}$ はこの条件を満たす。固定半径の球上で同じ写像の歪みは $R_t\epsilon_t/a_t$、半径のずれは動径射影とsourceの最短路で調整できる。さらに非空領域 $A_t$ で $\eta_t=\sup_{A_t}d_\square(f_t(y),e_i)\to0$ なら、$R_t(\epsilon_t+\eta_t)=o(a_t)$ の下で任意の $y_t\in A_t$ に一様なpointed GH収束となる。基点間距離を $R_t(\epsilon_t+\eta_t)/a_t$ で抑え、geodesic空間の等半径閉球のHausdorff比較で移す。同じP0の共通anchorから選んだ一成分のcoreと変更collarには $\eta_t\le Cq_t$、$q_t=(1+\log(N_{j(t)}+1))/R_t\to0$ が成り立つので、$a_t=R_t\sqrt{\epsilon_t+q_t}$ と取れる。これは既存P0への直接系であり、任意の中間尺度、tensor収束、二つの極限の交換、効果的な収束速度は未証明である。証明全文は主稿を参照する。

限定した依存監査では、固定SNC cuspから $\Psi\le 2AN_j$ のcompactを先に選ぶ `ke:component-logarithmic-connectors`、$P_j,C_j^{\rm neck}$ を $N_j$ より先に固定する `ke:same-moment-corner-reference`、source-armの局所tensor比較からscalar障壁への接続を点検した。Global clipped-depthのLipschitz評価は $f_t$ との値比較を使わず、same-moment接続はglobal portal上界を使わない。指定した鎖では循環やfixed-spaceの定理からmoving領域への無条件な移行を認めなかった。IV `pair:lem:diagonal-fixed-end` の固定base→end cut→有限誤差と予算→全小複素parameterの閾値という量化も独立に点検した。K2/K3については次項の指定証明鎖も独立に点検した。全外部証明・全一次文献・主稿全体の包括的再監査ではない。

## 全移動基点の中間尺度と固定shell

主稿 `topo:cubical-local-models` と `topo:cubical-moving-blowups` は、有限cubical targetの全局所模型と全移動基点の拡大極限を分類する。成分頂点では $C_{2,d-1}$、supportが二元の辺（$e_i+e_j$ も含む）では $\mathbb R\times\mathcal Y_{d-2}$、三座標が全て1の頂点では全角 $3\pi/2$ の錐、それ以外では $\mathbb R^2$ となる。$\mathcal Y_m$ は原点で貼った $m$ 本の半直線。局所閉球は全targetのambient距離に関して等長であり、移動基点の極限ではこれらの空間の任意の有限基点を許す。

`ke:distortion-to-pointed-balls` は、全射の全域歪みが $\delta$ 以下なら、任意の中心・同じ半径の閉球の基点付きGH距離を $3\delta/2$ 以下で比較する。これを同じP0の写像に適用し、`ke:intermediate-moving-classification` は $a_t\to\infty$、$a_t/R_t\to0$、$R_t\epsilon_t/a_t\to0$ の下でactual曲面の全移動基点の部分列極限を上の四型に分類する。任意の許容尺度と退化列で各型を実現できる。全域歪みの速度は未評価なので、この誤差条件を除いた任意の中間尺度、tensor収束、極限交換へは拡張しない。有限幾何とGH移送の証明は複数担当で独立に内部点検した。

`ke:source-inclusive-fixed-shell` は、sourceを含む固定残余compactで同一の正則体積frameを保ち、固定endのmoment $\pm4\pi/(-\log r^2)$ とshell横断費用を証明する。先にcompactと $r$、最後に全ての小さい複素 $t$ を選ぶ。Songの固定smooth locus収束とRochon–Zhangのcusp展開の一次資料を確認した。異なる正規形のprimitiveの一致やresidual period消滅は追加しない。`ke:global-clipped-cogram-lower` は固定parameterの有限評価へ定式化を改め、誤差消失は統合定理の最後の対角選択でのみ用いる。上下界・Part IV入力の指定証明鎖に循環やprotected距離のambient距離への無条件な置換は認めなかった。全主稿・全外部結果の包括的再監査ではない。

## Normal momentを保つ相対変更と五次の同時実現

`ke:moment-relative-replacement` と `ke:relative-replacement-gh` は、同じ保持cornerの全葉、sourceのcompact nodal neighborhoods、同じcanonical normal moment・anchor cuts、同じcomponent core領域を保つ相対変更に対し、基底値の差を
\[
\sup_x d_\square(f_{j,t}(x),\widehat f_{j,t}(x))
\le C\eta_{j,t},\qquad \eta_{j,t}=C(1+\log(N_j+1))/R_t
\]
で抑える。変更後のmarked Reeb productとcore coneの実際の商データ、全overlapのwhole-fiber一致は入力である。閉商を先に構成し、同じcorner inset・neck profile・小さいcore panelsでparameter化する。Reduced方向の変更をC1まで小さくする必要はなく、任意の指定変更を実現する定理ではない。これらの条件下ではGHの距離比較を引き継げる。五次では `ng8:quintic-full-moment` が初期source葉を選ぶことで所定targetの全moment実現と全open overlapsを与え、`ke:quintic-simultaneous-realization` がこの相対変更の条件を検証して同じ射影のatlas/GHを構成する。六次と先指定された追加保持集合への適用は別に残る。

`ng8:fixed-fiber-relative-dh` は、各固定tのfree compact bandで、作用不変primitiveとaffineな境界作用からStokesによりtotal reduced areaのaffine性を得る。Reference constantsのt依存を許し、actual KE形式のt=0へのsmooth extensionを仮定しない。一方、重み(1,−1)の標準模型を \(I_1+I_2\le c\)、\(\mu=I_1-I_2\) で切ると、周期2π規約で \(\operatorname{Area}(P_\mu)=\pi(c-|\mu|)\) となる（`ng8:source-dh-wall`）。Source横断の全intervalへfree-bandのaffine性を流用できないことを示す局所模型であり、actual P0全体の面積公式ではない。相対Moserには端germsとmarked identificationsに加え、保持集合の補集合ごとの正の有限配分が必要である。補集合が分かれる場合、総量と個別marginだけでは足りない。

`ke:raw-moment-error-insufficient` では、固定stageで \(\mu_t=-L_t^{-\alpha}\)、\(\nu_t=-L_t^{-\beta}\)、\(0<\alpha<\beta<1\) と取ると、\(|\mu_t-\nu_t|\to0\) でもlongitude差は \(\beta-\alpha\) へ向かう。近似matchingを用いる場合はnormal momentの絶対誤差でなく、profileを通した基底値差を制御する。

## 相対critical-areaの有限条件とactual source

正本は `neck_action_matching.tex` の `ng8:componentwise-critical-area`、`ng8:strict-area-cuts`、`ng8:p0-small-area-flexibility`。保持集合Kを固定し、自由成分をUα、critical regionsをDhとする。保持質量κh、自由成分質量Mα、目標ahに対し、可動部分の目標rh=ah−κhを置く。同じmarked相対isotopy classでの実現は、各非空cell Dh∩Uαに正のx hαを置き、row sumをrh、column sumをMαにすることと同値である。各incidence連結成分で総量が一致し、孤立rowを除く全ての真の非空row集合Sに
\[
\sum_{h\in S}r_h<\sum_{\alpha\in N(S)}M_\alpha
\]
が成り立つことが必要十分。有限個の条件であり、parameter familyが可解なら正の滑らかな選択が取れる。自由部とtarget incrementsだけに滑らかさを要求し、sourceを含むK内部のreduced measureを滑らかな面積形式と仮定しない。

証明は、各自由成分で積分零の面積差に固定支持のprimitiveを構成し、parameter-relative Moserを適用する。Densityはcritical graphの近傍で1にできるが、Moser isotopyがcritical graphを固定するとは主張しない。全full critical-leaf neighborhoodsまで固定すると可動面積が強制される場合があり、source固定の条件と混同しない。既存のdisk保護集合に対する `ng8:parametric-moser` の仮定は変更していない。

保持annulusの内側が一つのbasinだけに接すると、その自由成分の全質量がそのbasinに残る。総面積・個別protected-area marginだけではこの制約が見えない。`ng8:interior-area-cut-obstruction` は両端のopen germsを満たしても中央でstrict cutが破れる正のsmooth面積模型を与える。全rh、Mαがmomentについてaffineなら端点での有限検査で足りるが、smoothnessだけでは足りない。これらはactual KE族の反例ではない。

Actual P0では各sourceを通る正則閉葉の飽和annulusを保持する。小さいmoment intervalでは、全compact pinched torusとその近傍を固定しながら、外部の自由cellで滑らかな密度を変えられる。Incidence graphは連結であり、spanning-treeの有限線形右逆から、総和零の十分小さいδahを実現する正の密度ρ≥1/2を明示できる。許容εは固定t・stageに依存する。支持はKから離れ、開いたend germsでは恒等であり、free principal connectionによるliftをsource上で恒等に延長する。Lagrangian性はactual normal Hamiltonianと同じmoment levelから確認する。Lift自体をsymplectomorphismとは呼ばない。

Finite cutの原理はFord–Fulkerson, *Maximal flow through a network*, Canadian J. Math. 8 (1956), 399–404, [DOI 10.4153/CJM-1956-045-5](https://doi.org/10.4153/CJM-1956-045-5), Theorem 1 p.400・証明pp.400–402に対応する既知原理。出版社一次PDFを確認した。原論文の無向networkの記述を有向二部命題そのものとはせず、必要な有向の配分問題を本文で直接証明する。一般の最大流原理・Moser原理の新規性は主張しない。

### 球面の木配分とsource wall

`ng8:spherical-incidence-tree` と `ng8:tree-edge-area-test` は、end collarsとcritical leavesを避ける飽和regular annuliを保持した球面pants木について、incidence graphの木性とcell massesの一意なedge-cut公式を証明する。同じregion内の中間free gapsは全て固定面積で、external basinではcritical側に最も近い保護annulusより奥の全tail面積が下限となる。Internal regionでは両側subtreeのtarget増分の総和が二端cellsの余裕を決める。保持annulus自身の幅を縮めてもtrapped tailの面積は一般に消えない。正genusのcycle例では一意性が破れる。

`ng8:actual-source-area-wall` は周期1のnormal action μについて、sourceをn_h個含むactual領域の面積と保持質量を、それぞれsmooth function−n_h|μ|/2と書く。Equivariant Darboux ballsを取り除いたfree quotientで証明し、元のresidual座標の保存やt一様性は要求しない。`ng8:source-corrected-area-demand` の自由需要のsmoothness条件は target area−n_h min(μ,0) がsmoothであること。同じprimitiveとtransported cycle frameでのcritical actionsにはStokesの整数項を入れ、元との差ではsource wallが相殺する。Source shearは整数勾配を変えるが実数切片を修復しない。新proofの独立内部点検とanchor側への接続を進めている。

## Actual coreの有限anchor period条件

正本は `global_action_atlas.tex` の `ke:anchor-liouville-actions`、`ke:actual-anchor-fan-criterion`、`ke:anchor-stokes-budget`。周期1の未除算periodを用いる。Actual primitiveλ、normal faceのM=λ(V)=q−ρ、anchor q=δ、残余周期Aを固定すると、同じLiouville flowによる第二作用は
\[
I_\beta(q)=\frac{A}{\delta-\rho}(q-\rho).
\]
Collar外のqは作用の局所延長であり、元のcanonical circleが全coreで定義されるとは主張しない。Neck側とのclosed primitive差のperiodをκ、cycle変更をβN=εβ+kαとすると、I_N=c+pqとの一致条件は
\[
p=k+\varepsilon A/(\delta-\rho),\qquad c+\rho(p-k)=\varepsilon\kappa.
\]
Exact補正はこれらの周期を動かさず、Liouville homogeneityだけで整数傾き・切片一致を得ることはできない。

Actual corner cyclesとclutchingを保ったanchor critical periodsを、K4では−Mで選ぶ一つのbasinと残り0、Petersenでは四つのexternal values 0とinternal interval [0,−M]に指定できれば、同じdomain全体のLiouville fillingに標準fan近傍を構成できる。作用写像のrank2からprojective ratioの厳密単調性を得て、整数行列とstar latticeでambient normal actionのprimitive性を確認する。K4の4-cycleとPetersenのlabelled quartet、保持cornerの負のmeridian periods、同じprimitiveによる全Stokes条件は明示的な入力である。

実際のclutching Σ[βb]=−[α]、境界周期cbを用いると、normal quotientの面積は−Σcb−Mとなる。非閉λをhomology式に直接積分せず、sectionとwindingで証明する。Puncture collarsだけを固定する場合には負のinner boundary periodsから正のmarginが得られ、既存相対Moserでanchorを作れる。Source annuli等も保持する場合は前節の成分別cutを別に確認する。Anchor slope A/(δ−ρ)が無理数の固定fillingには作用適合rational fan chartがなく、これは既存P0や任意のfibrationの不存在ではない。

五次の標準保持集合ではactual代入から全moment実現・両端作用・全open overlapsまで構成した。既指定の追加保持annuliや六次のPetersen targetsには、保護成分ごとのstrict cutsとframingを改めて確認する。Source wallの周期規約、初期選択と変更後の保持対象を混同しない。

## K2/K3の全fiber接着で用いる条件

K2の正本は `ke_neck_corner_exhaustion.tex` と `ke_relative_corner_patch.tex`。`ke:quantitative-order-hamiltonian` は微分だけでなく比較Hamiltonian自身も $O(b_j^{-2})$ で評価するので、cutoffの $H\,d\chi$ 項に長いnormal stripの直径が入らない。自然性は全orbitを含む共通plateauでvector fieldの段階から用いる。Neckの葉によるtrim $B=7b_j$、corner sourceの下限 $6b_j$、実像の上界 $8b_j$、広いpatch $(5b_j,9b_j)$ の余裕により、first-exitで全逆軌道を共通域に保つ。逆flowの一致、momentの同定、深いnormal下界、全torusの同定の順なので循環しない。`ke:neck-corner-saturated-union` の結論は点の一致ではなく双方の同じ全fiberである。第二cycleは共通torusから移送して選ぶ。

K3の正本は `ke_component_link_cover.tex`, `ke_core_invariant_primitive.tex`, `ke_relative_reduced_foliations.tex`, `ke_actual_core_gluing.tex`。選択順は残余領域と $b_j$ → $n_j,\iota_j$ → $N_j$ →有限shellとflow buffers →parameter閾値である。Linkをmoment cutsから先に作り、その全shellの被覆を用いてadapted primitiveを作り、最後に外向性を確認する。Centered scalar primitiveのexactnessと一階評価、共通normal方向の周期性による $V(F_C-F_N)=0$ から、切替後も $Z^{\rm ad}\Psi>0$ を保ち、core外にtrappingを作らない。

Relative simple-saddle familyは、全critical leafを含むpants上のbasic drift方程式から実際に同じboundary-relative $\operatorname{Diff}_0$ orbitへ入る。Liouville側の族は既存anchor葉からの輸送であり、任意指定germの延長を仮定しない。Primitiveの切替 $B/b_j\in[5.2,5.4]$ は全K2交わりの下限 $11/2$ より内側で終わるので、全交わりを含むend collars上で補間を恒等にできる。Sourceのmoment零近傍と反対側componentのbandは支持外である。Whole-fiber trimは補間後のpartitionに対して内側平行linkを選んで行い、指定compactをその内部に保つ。`ke:actual-link-cone-filling` と `glue:closed-whole-fiber-quotient` が連結fiber・頂点連続性・Hausdorffな全域商を与える。

この指定鎖を独立に内部点検し、対象内で追加仮定や修正を要するギャップは見つからなかった。`ke:positive-residue-finite-type`, `ke:compact-relative-morse-smale`, `ke:actual-limit-weinstein-core` の固定形式へのexact Moser復帰と閉isotropic filtrationも本文の論証を確認した。これらの内部点検と、全外部入力の原典の包括的再検証・形式証明・新規性確認は区別する。証明全文は上記の主稿各節を正本とし、このノートへ複製しない。

## 全域実現定理と現在の点検範囲

主稿 `ke:global-realization` と統合証明 `ke:global-metric-realization` は、任意の固定 $d\ge5$ と既存一般性条件の全平面退化について、actual負KE形式の全域fibrationと、同じ $f_t=p_T\pi_t$ の全曲面ambient距離に関するdistortion消失を与える。潰される内部木上の全fiber合併も一様に収縮する。**原稿に証明があり、必要な証明箇所と接続を複数担当で内部点検している。** 形式証明、全主稿・全外部入力の包括的再監査、外部査読、網羅的な新規性確認は未実施である。現在は公表に向けた一次文献・依存結果・主稿構成の点検を優先する。

対象・結論の範囲と優先順位は [研究方針](../00_research_plan.md)、外部定理のpath・label・確認commitは [KE依存表](ke-dependencies.md) を参照する。ここには証明全文を複製せず、核心、入力の区別、有効な障害を残す。十分遅い対角選択と一つの許容された木系を使う結論であり、最適rate、任意の先指定木系への適合、全次数のmatroidal atlasは含まない。

一般存在定理、P0、作用適合atlasでは存在量化されるfibrationが異なる。一般存在は各所定Kähler形式に対するあるfibration、P0はactual KE形式に対し同じ $p_T\pi_t$ の距離を制御するある族、五次・六次のatlasは作用period・critical-region areasを合わせて選んだfibrationの結論である。五次の新定理 `ke:quintic-simultaneous-realization` は、初期source葉を選ぶ全moment構成により同じ $\pi_t$ の全域作用atlasとGHを証明する。六次は別々の存在であり、その同時実現へ読み替えない。さらに $d\ge7$ のP0構成では、core頂点の局所基底そのものにmatroidal chartが存在しない（`ke:global-core-nonmatroidal`）。これは当該構成のcoreに対する結論であり、一般型曲面上の任意の別fibrationの不存在ではない。

## 閉whole-fiber quotientと合成写像のEuler関数

`glue:closed-whole-fiber-quotient` では有限閉piecesのlocal fiber relationsの和が既に推移的である。交わるlocal fibersが同じ全ambient subsetだからであり、単なるgerm一致や有限閉貼合せだけでは足りない。閉同値関係からcompact Hausdorff quotientを先に得る。`ke:global-base-parameterization` のcell写像は有限閉pieces上で貼り合い、quotientの普遍性で連続写像に降りる。各labelled cellの内部と境界同定の全単射性から、compact-to-Hausdorffの同相判定を使える。この順序に循環はない。

`topo:connected-preimages` はcompact Hausdorff間のconnected-fiber全射が閉写像であり、任意の連結部分集合の逆像も連結であることを直接示す。従って `topo:cubical-composite-connected` により $f=p_T\pi$ の全fibersは連結。$p_T^{-1}(w)$ が内部木の場合、その全逆像は三次元部分を含み得る。$p_T$ のcell-like性から合成fiberの可縮性は導かず、Lagrangian性は個々の $\pi$-fibersの主張として保持する。

正本 `invariants_examples.tex` の `inv:euler-pushforward` と `inv:cubical-fiber-euler` は
\[
\pi_*\mathbf1=\sum_{\nu=1}^{d\binom d2}\mathbf1_{\{b_\nu\}}
+\binom{d-3}{2}\sum_{i=1}^d\mathbf1_{\{v_i\}},\qquad
\chi(f^{-1}(w))=\#\{\nu:p_T(b_\nu)=w\}
+\binom{d-3}{2}\#\{i:p_T(v_i)=w\}
\]
を与える。Node値は $B_d(T)$ 上で相異なるが、cubical像では衝突し得るので重複度を数える。正則torusとbranch fiberのEuler数は零、pinched torusは1、coreは $\binom{d-3}{2}$。有限層化と局所productに対し $\chi_c$ の加法性・積性を用い、写像全体のsubanalytic性やskeletonのWhitney性を追加仮定しない。Euler総数の一致だけで幾何学的gluingや全空間同定を代用しない。閉写像とEuler積分の一般原理自体は既知であり、本稿では実際の構成への仮定照合を行う。

## SNCの固定coupling chartsと葉のperiod障害

正本は `relative_compactification.tex` の `snc:reeb-leaf-kernel`、`snc:fixed-holonomy`、`snc:minimal-holonomy-controls`。Capを含むReeb商 $q_a:D_a\to T_a$ のkernel $L_a\subset H_1(D_a;\mathbb Z)$ はrank $g_a$ のprimitive Lagrangian格子であり、maximal subtreeの外の辺から選ぶ正則葉円周で生成される。SNC全体では
\[
H^1(D;\mathbb R)/q^*H^1(\Gamma;\mathbb R)
\cong\bigoplus_a\operatorname{Hom}(L_a,\mathbb R),\qquad
\dim=\sum_a g_a.
\]
固定normal connections・actual coupling charts・full fiber partitionの下で、同じ二形式とresiduesを持つprimitive差をbasic formとexact cutoffで処理できるための必要十分条件は、この商classが零であること、すなわち各成分の選んだ $g_a$ 個の正則葉periodの消滅である。Normal meridianのperiod差が零なのでcircle-bundle liftの選び方には依存しない。これは指定された補正経路の判定であり、任意のfibrationの不存在判定でも点固定core germのflux障害の消滅でもない。

残るbasic classはregular annuliのedge bumpsで表せ、全critical leaves・crossingsの近傍と有限個の指定値を避けて支持を取れる。Basic補正後のLiouville場の曲線方向は同じ葉に接するため、点ごとの固定ではなく全葉の保存を得る。非零障害は正則葉periodに双対な $\sum_a g_a$ 本のclosed formsで消せる。全 $2g_a$ component periodsの消去は十分だが過剰であり、二本のelliptic cubicsでは必要な独立方向は計二つ。これらのholonomy変更はcrossing disks・指定flat patchesを避けられるが、一般に元のfull saddle collarsまで全て固定はできない。`snc:saddle-support-obstruction` により、全full critical-leaf collarsで零のclosed connection補正は障害空間に作用しないからである。$D$ 上のmarked full leavesは固定し、変更後のpositive-normal葉は新しいcoupling chartsでliftする。

Connection/gauge固定とunitary holonomy phases固定は異なる。Periodsが $2\pi\mathbb Z$ のclosed form $\eta_a$ はphasesを変えずにreal primitive classを $-w_a[\eta_a]$ だけ動かす。これはlarge gaugeに伴うnormal framing変更であり、固定coupling chartsの命題に含めない。位相値だけを指定する問題の整数格子自由は別途扱う。

有限endpointの連続性はflowの位相同定だけに依存させない。Actual collarのcone座標 $r=e^{t-T(q)}$ はcomponent face・transition capで $r=1-\mu_a/w_a$、product crossingで $r=\max\{1-\mu_a/w_a,1-\mu_b/w_b\}$。これにより $D$ への任意の接近で $r\to1$ となる。Graph座標はcapの厳密単調endpoint式とcrossing invariantで連続に延び、実際の $D$ 上の指定全葉へ到達する（`snc:time`、`snc:endpoint`）。

一次資料との関係は次の通り。既知の原理と本稿での適用証明を区別し、網羅的新規性は未確認とする。

- **IKM：** Izosimov–Khesin–Mousavi, *Coadjoint orbits of symplectic diffeomorphisms of surfaces and ideal hydrodynamics*, Ann. Inst. Fourier 66 (2016), 2385–2433, [DOI 10.5802/aif.3066](https://doi.org/10.5802/aif.3066)。掲載版Lemma 4.8（p.2421）、Theorem 4.6の証明（p.2423）、§5（pp.2424–2425）を確認。成分上のlevel periods消滅とsmooth basic representativeの対応は既知であり、本稿では整数格子、SNC graphへの完全列、固定coupling chartsへの適用を証明する。
- **TMZ：** Farajzadeh Tehrani–McLean–Zinger, *Normal crossings singularities for symplectic topology*, Adv. Math. 339 (2018), 672–748, [DOI 10.1016/j.aim.2018.09.035](https://doi.org/10.1016/j.aim.2018.09.035)。確認版 [arXiv:1410.0609v3](https://arxiv.org/abs/1410.0609v3) のDefinitions 2.11–2.12（p.16）、Theorem 2.13（p.17）はHermitian structures・connectionsを含むcompatible regularizationsをexact deformationの後に与える。固定された元の二形式・任意指定connectionの同時実現や、固定複素構造に対するKähler性の保存をそのまま主張する定理ではない。
- **BSV：** Borman–Sheridan–Varolgunes, *Quantum cohomology as a deformation of symplectic cohomology*, J. Fixed Point Theory Appl. 24 (2022), article 48, [DOI 10.1007/s11784-022-00965-6](https://doi.org/10.1007/s11784-022-00965-6)。掲載版Propositions 2.5・2.7（p.30）はorthogonalityとcommuting normal Hamiltonians、Proposition 2.10・Remark 2.11（p.31）はpositive real divisor coefficientsからadapted primitiveとscHの存在を扱う。この命題には $H^1(M)=0$ やmonotonicityは不要だが、任意に先指定したconnection・holonomy・core germ・marked Morse全葉の実現は結論しない。Remark 2.2のdivisor isotopyは、固定divisorの下で形式を変形する経路と区別する。

`snc:output-data` と作用period接着の関係は次節に整理する。Divisor-relative Moserでnormal actionsを移すことと、独立な第二period・critical valuesを指定することは別条件である。

## 正則bandの第二作用と非直線critical action

`neck:regular-period-matching` は、可縮な正則action chart上のexact $T^2$ bundlesについての判定である。Normal cycle $\alpha$ を保ち、$\beta_-\mapsto k\alpha_++\varepsilon\beta_+$（$k\in\mathbb Z,\ \varepsilon=\pm1$）とする既定base同定 $h$ の上のsymplectic matchingは、ある定数 $c$ に対する
\[
\mu_+\circ h=\mu_-,\qquad
J_-=k\mu_-+\varepsilon J_+\circ h+c
\]
と同値である。固定primitiveに関するexact matchingはさらに $c=0$ と同値。Normal actionだけでは第二作用を決めない。`neck:normal-action-counterexample` の定数shiftはsymplecticだがexactではなく、非線形shiftは指定base同定と整数shearを保つsymplectic matchingを妨げる。Base同定を変更すれば同じ物理的torus partitionにもなり得るため、fibrationの不存在とは異なる。一般のbaseではprimitive差にbaseの $H^1$ が残り得るので、この局所判定を無条件な大域exactnessへ拡張しない。

この判定は既知のaction-angle理論のspecializationである。Evans, *Lectures on Lagrangian Torus Fibrations*, [arXiv:2110.08643v4](https://arxiv.org/abs/2110.08643v4) のTheorem 1.42（p.16）、Lemma 2.10・Theorem 2.12（pp.24–25）、Lemma 2.15・Remark 2.17（pp.25–26）、Lemma 2.25（pp.28–29）を一次資料で照合した。番号・頁は掲載書籍と混同せず同arXiv版に固定する。Theorem 2.26（p.29）の大域fiber-preserving同値にはglobal Lagrangian sectionsの仮定がある。

Canonical primitiveの規格化にも独立の差がある。`ke:transition-residual-period` は、volume framesの比 $a(p)$ による残余cycleのperiod差を $-2\pi\operatorname{wind}(a_t\circ p\circ\gamma)$ と記録する。Normal cycleでは差が零でも、残余cycleでは非零になり得る。Exact模型 $xyp=t$ のlogarithmic frameとneck frameでは、比が $1/p$ ならprimitive差は $d\arg p$、正の一周の差は $2\pi$（作用を $1/(2\pi)$ 倍で測れば差は $1$）である。同一physical leafの接着を妨げるものではなく、別々のcanonical primitivesを無条件に同じ作用原点として扱うことを禁じる。

### 固定した形式と端のgermsからも直線性は従わない

`atl:critical-action-obstruction` によれば、branch上でnormal action $\mu$ が非定数なら、作用適合matroidal chartの存在には $J^{\rm crit}(\mu)=p\mu/q+c$ が必要である。各regular sheetの作用座標からfan faceへの変換が整数affineであり、fanのbranch rayが有理直線であるためである。これは $q=1$ に限らない。

`atl:fixed-form-bent-branch` は $\Omega=d\mu\wedge d\theta+\omega_P$ を固定し、critical leafのregular arcだけを動かしてbasin面積を $A_0+\epsilon b(\mu)$ にする。変更はnormal action、両端のopen germs、全toric collars、saddle点近傍のMorse germ、marked treeを保つ。得る葉族はLagrangianだが、$J^{\rm crit}=J_0^{\rm crit}+\epsilon b(\mu)/(2\pi)$ なので $b''(\mu_0)\ne0$ の点には任意のdenominatorを許しても局所作用適合matroidal chartがない。既知の局所正規形だけではfull critical leafの作用を制御できないことを示す。

既存の五次・六次atlas構成はこの障害を避けるため、同じembedded marked class内でcritical-region areasを指定し、framingの整数slopeと作用の切片を合わせる。`ng8:straight-neck` の両端は同じ $\operatorname{Diff}_0(P\operatorname{rel}\text{ collars})$-orbitに取る。`ga8:affine-persistence` はfibration・cycles・primitiveを同時に運び、`ng8:transport-intercept` は一つの全空間primitiveを使う固定非零moment上のexact transportで値を保存する。これはnormal action単独による第二period一致ではない。既存の一般symplectic存在、選んだ五次・六次fibrationの作用atlas、全固定次数のP0は異なる結論として保持する。

## Focusの半大域不変量と全飽和近傍の移送

正本は `ke_staged_neck_averaging.tex` の `ke:source-focus-transversality`、`ke:focus-neighborhood-period`、`ke:focus-local-primitive-shift`、`ke:focus-whole-neighborhood-transport`。指定写像 $(\mu,A(\mu,p))$ がsourceで非退化focus型である条件は $d_pA(0,q)\ne0$。$A=(a-a(q))^3$ は同じ葉の分割を持つが二次項が退化するため、foliationの型だけで指定写像の非退化性を結論しない。

一重pinched torusの十分小さい飽和近傍 $N$ は、可縮node blockとregular annulus blockの二つのcollarsによる貼合せであり、$H_1(N;\mathbb Z)=H_2(N;\mathbb Z)=\mathbb Z$。正則torusのnormal vanishing cycle $\alpha$ は消え、残余cycle $\beta$ が $H_1(N)$ を生成する。Closed primitive差 $\zeta$ のexactnessは $\int_\beta\zeta=0$ と同値で、normal periodは自動的に零。Annulusの縦座標に沿う $f(s)ds$ はnode近傍を固定した非零残余periodを作れるが、外側regular torusの近傍まで零にはできない。

全飽和近傍で同じfibrationをsymplectic map $\Phi$ によりpush-forwardすると、compact fiber、strata、cycles、return periodsと通常のTaylor不変量 $S$ が保存される。さらに $\Phi^*\lambda'-\lambda=dQ$ なら全作用積分と追加定数 $S_0=\int_{\gamma_0}\lambda$ も保存される。Primitiveのclosed変更は $S_0$ を動かし得るが、$A(c)-A(0)$ で定義する $S$ には影響しない。周期1 normal momentは $c_2=\mu/(2\pi)$ とし、Eliasson基底座標・向き・return cycle・log branchを一緒に運ぶ。独立chartのflat自由度と、$2\pi k c_2$ のcycle/branch自由を区別する。Sourceでは $(\eta,\mathcal A\lambda_t)$ から $(\omega_t,\lambda_t)$ へ同じexact Moser mapで運ぶ。別canonical frameへの置換は `ke:transition-residual-period` のwindingを別に確認する。

一次比較：Vũ Ngọc, *Topology* 42 (2003), 365–380, [DOI 10.1016/S0040-9383(01)00026-X](https://doi.org/10.1016/S0040-9383(01)00026-X)。確認版 [math/0208245v1](https://arxiv.org/pdf/math/0208245v1) のTheorem 2.1（PDF p.4）、Proposition 3.1・Definition 3.1（pp.6–8）、Lemma 4.1・§4（pp.9–11）、§6（pp.14–16）、§7 “Exact version”（p.18）を用いる。$S=0$ と $S=X^2$ の実現は同じ線形focus型・vanishing cycle・一重monodromyでも半大域同値でない既知の具体例。$S_0$ の追加も既知であり、本稿の新規な分類結果とはしない。Zung [math/0110147](https://arxiv.org/pdf/math/0110147) のPDF p.4脚注は、同じfocus数のfoliationについて旧文言を「homeomorphic, not necessarily diffeomorphic」へ訂正している。一般のsmooth foliated equivalenceをこの位相分類から推論しない。異なる $t$・stageの不変量一定や任意指定focus不変量は本稿の結論に含めない。

## Nodal blow-upの実面積と比較写像の支持

`global_gluing.tex` の `glue:area-normalized-blowup` は、指定された複素blow-up上で例外曲線の面積 $e$ を直接実現する。$dd^c=i\partial\bar\partial$、$\omega_{\rm st}=\sum dx_j\wedge dy_j$ の下でlogarithmic potentialの係数は $e/(2\pi)$、標準球の半径は $\sqrt{e/\pi}$。Classは $\pi^*[\omega]-e\operatorname{PD}[E]$ である。Fleming, *Kähler packings of projective complex manifolds*, European J. Math. 7 (2021), 1382–1400, [DOI 10.1007/s40879-021-00491-8](https://doi.org/10.1007/s40879-021-00491-8), [arXiv:1905.03140](https://arxiv.org/abs/1905.03140), Lemmas 4.4–4.5、Proposition 4.6、Construction 4.7のradial原理を適用する。容量の文字やFubini–Studyの規約をそのまま流用せず、$e=\int_E\omega$ で照合する。

Chakravarthy–Groman, *Almost toric fibrations on symplectic blow ups*, [arXiv:2510.00994v1](https://arxiv.org/abs/2510.00994v1), Theorem 1.1、Propositions 3.1・3.6、§4の相対比較は、選んだaffine-convex領域の全逆像の外で恒等とする。球の外全体で恒等という強い支持条件には置き換えない。固定Delzant rectangleの人工三辺をcutし、人工divisor chainの近傍を固定した比較を元patchへ戻す。全boundaryの和がanticanonicalであることを本稿全体に要求する適用ではない。

選択順序は、互いに素な飽和patchとaffine-convex領域を固定し、容量triangleがその内部に収まるよう $\epsilon$ を選び、全compact nodal neighborhoodsを確保し、これらを避けてnormal-conjugacy collars・cutsを選び、最後に $t$ を小さくする。既知のradial blow-upと相対surgeryの本稿への適用であり、任意の独立primitiveのexact matchingを追加しない。全域quotientとEuler予算への接続は本ノート冒頭と本文の対応する補題に整理し、次はIntroduction・主定理のscopeと既知結果比較を全域構成から逆向きに照合する。

## 主要解析入力の確認範囲

Capped volume下界の六型determinant、full-triple比較の固定境界面でのdensity下界、模型側SchwarzとSavinの小摂動定理、Songのfixed-gauge収束、Rochon–ZhangのSNC remainderを重点点検した。一般のcomplete volume上比較では、対数体積比の上有界性を明示し、Ricci下界から得るLaplacian型最大値原理とAM–GMで証明する。有限窓・angular coverでの実適用は、固定parameterのcompact closureとmodelの境界発散からこの上有界性を確認する。外部正本にも同じ仮定を明記した。定理ラベル・一次資料・監査の限界は [KE依存表](ke-dependencies.md#主要な外部解析入力の重点監査) にまとめる。Cheng–Yau (1982)原論文の証明の再精読、全旧証明・全先行研究の包括的確認は未了である。

## Sourceを含むsharp scalar評価から全曲面の下界へ

正本は `papers/sections/paper/ke_sharp_normal.tex` と `ke_global_ambient_lower.tex`。正則global normal frameで $s=-\log|x'_g|^2$、$U=|d\log s|_{g_t}^2$ とすると、$\Delta s=0$ とrank-one Bochner計算から $\Delta\log U\ge U-1$ を得る。Source-inclusive方程式 $x'_gy'_g=th_t(p)$ に対し、$\mathfrak n_j\le s\le\kappa L$ の比較領域は $h_t(p)=0$ でもannulusと固定残余compactの積であり、sourceを除く人工境界を必要としない。

補助cut $\mathfrak n_j$ は、neck/corner構成の $n_j$ とは独立の記号とする。三種類の境界を分ける。残余境界は既存full-tripleの係数1評価、外側固定shellは射影下界と固定座標微分からの有限上界 $A_j$、内側 $s=\kappa L$ は既証のsource-arm tensor比較による有限上界 $C_j$ を使う。Arm比較はpositive-Poisson bufferとlocalized Schwarzから独立に得られ、このscalar障壁を入力にしない。明示的な障壁
\[
 B(s)=1+\varepsilon_j+A_j\mathfrak n_j/s+C_js/(\kappa L)
\]
が `ke:sharp-scalar-normal-barrier` の中心である。外側でsharp cusp漸近を仮定せず、下側clipを後から十分深くして $A_j\mathfrak n_j/s$ を吸収する。残余frameのbase-only差とMorse変換の $O(t)$ 誤差は、active上側cut $s\le L/K_j$ と $K_j>4$ の下でphysical depthへ転送する（`ke:sharp-global-one-active`）。

旧corner cut $6b_j$ と独立に $\mathfrak m_j\gg A_j\mathfrak n_j/\varepsilon_j,N_j$、$K_j\gg C_j/(\kappa\varepsilon_j)$ を選び、最後に $\log\mathfrak m_j+\log K_j=o(R_t)$ とする。Global clipped map
\[
 \Theta_{i,t}=\left[\frac{\log(\ell_i/\mathfrak m_j)}{\log((L/K_j)/\mathfrak m_j)}\right]_0^1
\]
には少なくとも一つのplateauがあり、active方向は高々二つ。二方向はfull-tripleのdominant-product比較、一方向は上のscalar評価で扱う。`ke:global-depth-lipschitz` は全曲線に対する長さ評価を先に与え、領域間の往復回数に依存しない。

`ke:global-depth-base-comparison` は、cornerの旧softmaxとcoreの頂点値を比較し、neckでは `ke:same-moment-corner-reference` の参照torusへ値比較を移す。固定残余基底を全marked tree・source discs・旧corner辺の残余像を含むよう先に選ぶ。旧辺は $B=6b_j+r_c$, $0\le r_c<1$ なので、この選択はcomponent cut $N_j$ に依存しない。各保持neck点 $x$ には同じcanonical momentを持つ旧corner辺の任意の点 $y$ があり、既証のsource-inclusive同一moment接続から $d_{g_t}(x,y)\le C_j^{\rm neck}$。従って、$\Lambda_{j,t}=\sqrt{1+\epsilon_{j,t}}/S$ として
\[
 d_\square(\Theta_t(x),f_{j,t}(x))
 \le \Lambda_{j,t}C_j^{\rm neck}
   +d_\square(\Theta_t(y),f_{j,t}(y))
   +C\eta_{j,t}.
\]
最後の項は両点で同じmoment profileを使うことによる。これは点の選択であり、torus bundleの大域sectionを仮定しない。経路はfiber又はmoment levelの内部に留まらなくてよい。Source固定点・軸・pinched fiber・saddle fiberも同じ集合に含まれる。

依存順序は、局所的なsource退出と同一moment接続、全曲線での $\Theta_t$ のLipschitz評価、cornerでの値比較、全neckへの移送、同じ $f_t$ の距離下界である。全域上界やGH収束を参照点の存在・費用に使わない。`ke:fixed-base-neck-moser` と `ke:fixed-base-moment-connectors` は、固定残余近傍に依存する有限下限 $m_P$ 以上の全cutに一様であることを定理文に明示する。正の固定bufferと $C_P/m$ の短円評価を用いるので、固定stageを先に選んでから $t\to0$ とする用途に適用できる。

`ke:common-profile-log-depth` の $\sigma_t(\mu)=\log(1/|\mu|)/R$（向きにより $2-$ を付ける）という解釈も保持する。直接の座標比較を要する用途では、`ke:source-arm-moment-depth` の $s\asymp_j|\mu|^{-1}$、中央帯の $s_x,s_y\ge\kappa_jL$、projected coordinatesの $O(t)$ 差を使える。全域値比較自体は上の参照torusによる移送で証明する。CP/PBE/TC全体を証明したのではなく、本稿の下界に必要な入力を直接与える。

### 固定族の係数で書ける上下両側の誤差

同一momentの参照点を使うと、基底値比較の定数の依存も整理できる。K2のcutoffsは $\log(b/b_j),\log(a/n_j),\log(c/n_j)$ の固定幅の関数であり、正規化した全固定階のnormは段階に依存しない。Cornerの座標補間、全平均Moser、相対Hamiltonianのactual変位は $C/b_j$ 以下、global section normsのunit差も有限個の固定triple chartsで一様である。Coreでは下側clipを非成分深度上界より大きく取ると $\Theta_t=e_i$ なので、coreの段階定数は値の誤差の係数に入らない。

残る $C_j^{\rm neck}/R_t$ は、残余基底を先に固定してから既存の許容cut条件 $C_j^{\rm neck}\le1+\log(N_j+1)$ を課すことで吸収できる。従って `ke:global-depth-base-comparison` の係数は固定次数・固定族にのみ依存する $C$ とできる。主稿の `ke:eq:global-realization-explicit-cut-budget` は、上下両側を合わせて
\[
\operatorname{dis}(f_{j,t})\le C_d\left\{\varepsilon_j+b_j^{-1}+K_j^{-2}
 +\frac{1+\log R_t+\log\mathfrak m_j+\log K_j+\log(N_j+1)}{R_t}\right\}
\]
を与える。残余接続定数、scalar障壁の境界定数、fixed-compact convergenceは、cutの下限と最後のparameter閾値を決める際に依然必要である。これらの有効な増大率を評価しておらず、$R_t$ のみの最適収束速度とは区別する。

## Portal上界と潰される木の全fiber合併

正本は `papers/sections/paper/ke_global_ambient_upper.tex`。`ke:global-ambient-upper` は、保持corner内の旧経路を全曲面の経路として用い、同一momentのneck接続、source退出、各componentの固定stage費用を有限のtarget galleryでつなぐ。保持corner自体の新しい内在距離評価は要求しない。対象ごとに固定した有限定数は最後の遅い対角選択で $o(R_t)$ とする。

`ke:collapsed-tree-common-moment` により、中央辺区間 $\kappa<u<2-\kappa$ では、$p_T$ の潰す内部木上の全fibersが同じcanonical momentを持つ。`ke:collapsed-tree-full-fiber-collapse` は一つのtorusだけでなく、その木上の全 $\pi_t$-fibersの合併を評価する。Sourceの中央帯・非中央armとcore側endpointを含めてこの評価を行い、全域上下界を `ke:global-metric-realization` へ統合する。経路がfiber又はmoment level内に留まるという主張ではない。

### 端点の選択と全fiberの分類

旧辺の保持部分は正確に $|\mu|\le\delta_j$ の全toriである。$u=\kappa,2-\kappa$ は境界toriを含み、$u=1$ のportalは $\mu=0$ のregular corner torus上に取る。Sourceやbranchとの接続には同一moment集合全体のambient評価を使う。各 $(a,J)$ でanchor torus上の点 $p_{a,J}\in S_{a,j,t}\cap A_{t,J}$ を一つ先に固定し、頂点とその近くの辺ではその点を使う。Portalの連続選択は要求しない。

| Target点 | 全 $f_{j,t}$-fiberの位置と接続 |
| --- | --- |
| Support 3、inset disk | 保持cornerの一つの旧全torus。非正規化内在径 $C/m_j$。 |
| Support 3、neck panel又はcore sector | 一つの構成後fiber。対応する同一moment集合又は一つのcomponent compactで評価。 |
| $E_{ab}(u)$、$\kappa<u<2-\kappa$ | 厳密に $\mu=\sigma_t^{-1}(u)$ の内部木上の全neck fibersの合併。 |
| $E_{ab}(u)$、$0<u\le\kappa$ 又は $2-\kappa\le u<2$ | 一つのcomponent core・変更collar。等号の端点ではcore coneのlevel 1とneck anchorが同じ全fibers。 |
| 頂点 $e_a$ | Component $a$ のskeleton。 |

K2の全交わりの飽和、whole-fiber trim、開collarでの全葉の一致により、交わる局所fibersは同じambient subsetである。従って局所fiber関係の有限和が既に推移的であり、support 3で異なる局所fibersを継ぎ足した余分なglobal fiberは生じない。

`topo:finite-endpoint-comparison` は、anchor誤差 $a$、squareの端点距離誤差 $\lambda$、junctionと初終点の接続費用 $\kappa'$ から
\[
 d_X(x,y)\le d_\square(Fx,Fy)+M_d\lambda+(M_d+1)\kappa'+2a,
 \qquad M_d=3\binom{\min(d,6)}3\le60
\]
を与える。Actual上界では $a=C\eta$、$\lambda=E+2C\eta$、$\kappa'=H/R_t$。旧full corner内の経路は全曲面の経路として有効であり、保持corner内へ閉じ込める必要はない。抽象的な(F)もambient fiber径の条件であり、fiber内在経路の長さを仮定しない。

### Closed cornerの有限cutと収束の区別

`ke:slow-cut-closed-corner-gh` は $m\ge m_*$、$R\ge R_*$、$\log(m+1)+4\log R\le R/8$ の有限条件で
\[
 \operatorname{dis}(\pi_{t,J}^{(m)})\le C\left\{m^{-1}+\frac{\log(m+1)+\log R}{R}\right\}
\]
をactual像上の射影 $\pi_{t,J}^{(m)}=P_{t,m}\circ\phi_{t,m}^{-1}$ と内在距離・protected距離の双方に与える。全fiberの非正規化内在径は $C/m$。証明では $B=(m+1)R^4\le L^{1/8}$、$\delta=\log B/R\le1/8$、$S=R-\log m-\log R>R/2$ とし、full-triple比較を深度 $m/2$ で用いる。同じ有限下限でMoser bufferとpullbackの正値性を得る。Raw座標と $\mathcal C_J$ の距離は全許容cutで $C/R+C/(mR)$ 以下となり、固定retractionの定義域にも一様に入る。固定 $m$ の後に $t$ を小さくする適用は許されるが、誤差消失にはさらに $m_t\to\infty$、$\log m_t=o(R_t)$ が必要である。これは固定族についての評価であり、次数一様性や最適rateを示すものではない。

## 有限の飽和全被覆でも局所加法誤差だけでは足りない

有効な障害として `ke:full-cover-oscillating-bypass` を `ke_global_ambient_lower.tex` に保持する。Rectangle上の計量を $g_N=dy^2+a_N(x,y)^2dx^2$ とし、上下の薄い列で $a_\pm(x)=1\pm c\sin(2\pi Nx)$、中央帯の幅を $h_N=N^{-3}$、係数を $1+c$ とする。上下各半分ではprimitive $A_\pm(x)=\int_0^xa_\pm$ により局所intrinsic/protected distortionは $O(N^{-1})$、恒等写像のfibersは一点である。しかし安い側を周期ごとに選ぶ経路の長さは $1-2c/\pi+o(1)$ となり、全域下界の誤差は消えない。

これはactual KE族の反例ではなく、有限の飽和全被覆・連結overlap・zero fiber diameterから局所加法誤差を有限回だけ足してよいとする推論への反例である。正しいbuffer原理には局所誤差とfirst-exit幅の比 $\epsilon/b\to0$ が必要（`ke:buffered-local-lower-globalization`）。本稿のP0では全曲線のscalar微分評価を使い、この往復回数の問題を回避した。

## 固定残余基底のnormal比較と相対接着の入力

固定 source-free compact 基底上の moving normal strip では、actual 計量で一定の buffer と $O(m_t^{-1})$ の短円を証明した（主稿 `ke:fixed-base-neck-moser`）。$\varphi_t=\log(\omega_t^2/\Omega_{t,d}^{\rm low})$ とし、大域の $\varphi_t\ge-C$ と $dd^c\log\Omega_{t,d}^{\rm low}\ge c\omega_{\rm FS}$ を、正則包含の Chern–Lu 不等式に組み合わせる。最大値原理から $\operatorname{tr}_{\omega_t}\omega_{\rm FS}\le C e^{A\varphi_t}$。固定 pair chart では体積包絡が $\varphi_t\le C$ を与える。入れ子座標間の固定射影幅から actual 球を確保し、局所 Chern–Lu を complete annulus–disc に適用して actual 二側比較を得る。法線深度を $m_t$ から $m_t/2$ に広げ、残余基底にも固定した余裕を取ることで、Moser map の source と像の両方が同じ内側 strip を覆う。

Residual collarを三重点へ動かす共通flow領域と葉の一致は、以下の遅いexhaustionで確保した。Source gate の $|x|\asymp |t|^{1/2}$ では固定射影座標の距離下界は法線の rescaling 幅を検出しない。 一方、source 模型 $xy=tz$ の法線円は gate まで残余方向の rank-one 下界と annulus–disc の体積上界で短くなる。正則ベクトル場 $x\partial_x-y\partial_y$ の Bochner 不等式で gate の $O(L_t^{-1})$ 評価を central bidisc に伝播できる（主稿 `ke:source-short-circle`）。固定 shell 上の成分KE収束と cusp 下界を使い、対角選択で十分遅く縮む source 領域に限り、共通 Moser source・像と actual focus–focus germ を構成した（`ke:source-diagonal-moser`）。所定の速さで動く法線境界の下界は別問題である。固定残余領域内の閉じた pinched torus は次の共通neckで構成する。

Source と通常 pair の共通化を主稿 `ke:projected-source-normal-form`, `ke:projected-source-neck` で証明した。固定残余基底で射影を保つ正則 Morse 座標 $x'y'=t h_t(p)$ を用いる。capped density と短円評価は $O(t)$ 座標変更で保たれ、固定 shell の対角選択で source を含む一つの actual Moser map を得る。共通 primitive の moment と基底射影の組で商は $I_t\times P$。指定した残余葉の持ち上げから、閉じた一重 pinched torus と saddle fiber が得られる。三重点側との共通開領域と全intersectionのfiber一致は、以下の部分fibrationで実現する。

三重点と射影neckの座標接続の正本は `papers/sections/paper/ke_neck_corner_transition.tex`。全三重点を避ける共通の無限遠超平面内に各二重線の射影補空間を選び、三平面の式 $q_0q_1q_2=tU$ のunitを三乗根で対称に除く。射影Morse変換の後にbase-only gaugeを施すことで、三つの端を同じexact triple chartと比較できる。固定 $\sigma>0$ のarm $\ell_i,\ell_j\ge(1+\sigma)\ell_k$ では、座標比の主枝対数 $e_{ka}$ が全phase・全固定階で $\|e_{ka}\|_{C^q(h)}\le C_{q,\sigma}e^{-c_\sigma m}$ を満たす。深度の相対幅が一定の正規化正則chartでCauchy評価を使い、$L_t$ に依存する微分損失を避ける。

三つの分離したarmで積を保つsmooth補間を行うと、一つのtorus作用が各端の射影neckのnormal circleに厳密に一致する（`ke:three-arm-coordinate-interpolation`）。補間帯では非正則なのでKähler性を主張せず、共通toric模型との小摂動から平均と凸pathのtame symplectic性を証明する。Canonical primitiveの差はbase-only closed formと一価関数のexact differentialに分かれ、normal periodは一致する（`ke:transition-normal-primitive`）。残余cycleのperiodは同じとは限らない。

`papers/sections/paper/ke_relative_corner_patch.tex` はcentered averagingの順序比較を定量化する。模型に近いprimitiveを選ぶと、比較Hamiltonianそのものが $O(e\delta)$ であり、領域の直径を掛けずにcutoffできる。Actual tripleでは $e,\delta=O(m^{-1})$ なので $O(m^{-2})$。三つの端にそれぞれ指定したnormal-first構成を、一つのactual corner bundleへ組み込める。小さいreduced circle graphを固定collarの外で恒等なdiffeomorphismへ延長する明示式も `ke:reduced-collar-graph` に置く。単一armでは、共通moment stripと外側marginを指定すればactual reduced葉のgraph評価も証明した（`ke:single-arm-reduced-graph`）。Normal生成場の長さを $a$ とするとmoment差が $O(a b^{-2})$、normal微分が $\ge ca$ なので、normal深度が極端に大きくても逆係数 $a^{-1}$ の損失は相殺される。Graphの $C^1$ はmomentを固定した残余座標に関するものとし、無重みのmoment微分には同じ一様性を主張しない。Source-inclusive neckとの共通moment stripとflow領域は、`ke:neck-corner-diagonal-matching` で別途確保する。

単一armで必要なmoment区間の存在も `ke:arm-common-moment-strip` で実証した。残余深度 $b\asymp b_0\to\infty$、$b_0/L\to0$ とし、normal端を $\ell_i=Kb$ または $\ell_j=Kb$（固定 $K>1+2\sigma$）に取ると、canonical momentは
\[
 \mu,\nu=\pm\frac{4\pi}{Kb}
 +O\!\left(b_0^{-2}+\frac{(b_0/L)^2}{b_0}\right).
\]
従って $I_t=[-c_*/b_0,c_*/b_0]$ の各levelが全残余annulusで一意に存在し、固定比のarm marginを持つ。Source-inclusive neckとの共通区間・共通flow domainには、下記の固定段階の選択を追加して使う。

微分評価の障害：単に $\ell_i-\ell_k\to\infty$ では足りない。例えば $f=\zeta_i/\zeta_k$、深度 $(N+\log N,N+\log N,N)$ では $|f|=N^{-1/2}$ だが、cusp単位ベクトルでの微分は $N^{1/2}$ と増大する（`ke:coordinate-czero-obstruction`）。座標比の値が1に近いことを、Moserの正値性に必要な微分小摂動へ読み替えない。

固定残余compactの各座標では、`neck:prop:volume-envelope` から法線方向の積分評価を得た（主稿 `ke:neck-integrated-normal-energy`）。$s=-\log(|u|^2/r^2)$、$d(s)=\min(s,M_t-s)$ とし、周期1生成場の軌道平均エネルギーを $E_t$ とする。$\Omega=du/u\wedge dz$ に対する対数体積の角度平均 $\bar F_t$ は $-2\log d(s)+O(1)$、かつ $E_t=8\pi^2\partial_s^2\bar F_t$。よって $\int_m^{M_t-m}E_t(s,z)\,ds=O(m^{-1})$ が残余点 $z$ に一様に成立する。例外深度の測度は $E_t>A/m^2$ に対し $O(m/A)$ であり、例外集合の位置は $z$ に依存する。

同じ $z$ に沿う動径経路には一つの角度を選んで長さ $\int_a^b ds/d(s)+O(1)$ を得る（`ke:neck-axial-upper`）。両端円が短ければ任意の端点を結べる。固定 source-free 基底で同じ normal moment を持つ点については、残余点を変える接続も原稿 `ke:fixed-base-moment-connectors` で解決した。深度は、$|\mu|=O(M_t^{-1})$ なら両側とも $M_t$ と比較可能、それ以外は符号に応じた片側深度が $|\mu|^{-1}$ と比較可能である。一定深度の水平持ち上げ・動径弧・短い円弧を合わせると、level全体の actual ambient 直径は $O(1)$、Moser像でも同じ、正規化後は $O(R_t^{-1})$ となる。葉内経路やMoserの $C^1$ 評価は使わない。Sourceを含む中央levelは以下の全点径で扱える。Sourceを含む全intervalへの拡張は以下のscaleごとの退出評価で得た。Moving residual collarと全域基底値の対応、および全曲面の下界は別に扱う。

Moser 流では軌道全体の最大速度を軌道平均エネルギーの平方根で置き換えられる（`ke:neck-averaged-speed`）。外側の深部領域の実計量での境界距離 $\delta_t$（上限1）が $m_t\delta_t^2\to\infty$ を満たせば、局所 Chern–Lu と体積上界から共通の source・像を得る（`ke:neck-shrinking-buffer`）。この縮小条件は残余 collar を動かす場合にも候補となる。

固定残余基底上で両側の moving cut $m_t$ における canonical moment は符号が逆で絶対値が $m_t^{-1}$ と一様比較可能である（`ke:neck-deep-moment-strip`）。よって同じ actual Moser map の下で、深部に共通の縮小 moment interval を置ける。K1の局所的な成功後も、第二periodとreduced葉の同時整合、source・branch・coreの被覆、全曲面のshortcutとportalを別々に検証する。任意のMoser移送による定性的存在と、\(p_T\pi_t\) の距離歪み消失も区別する。

大域距離の証明には、関連KE側の条件付き近似写像を入力にする経路と、同じ $p_T\pi_t$ に対して全域上下界を直接示す経路を区別する。本稿では後者を実行した。CP/PBE/TCの対象族での検証自体は結論せず、人工的な基底計量をactual全空間の距離と同一視することもない。

## 共通の end collar での actual fiber の一致

主稿のラベル `ke:normal-flow-naturality` が自然性の正本。全円軌道を含む共通plateauで同じcentered kernelを選ぶと、$G^*K_N\omega_N=K_\alpha G^*\omega_N$ であり、全trajectoryがそこに留まる限り $\phi_NG=G\phi_\alpha$ が厳密に成立する。Primitive $\lambda$ の一致を仮定せず、flowを決める $K\omega$ を比較する。Canonical normal momentの一致と合わせれば、corner torusはneckの同じmoment reduction上の円の全逆像として一致する。

主稿 `ke:neck-corner-diagonal-matching` は、残余cut $b_j$ と固定compact $P_j\Subset P_j^+$、それらの定数を支配するnormal cutoff $n_j\gg b_j$、共通moment区間 $I_j$、最後に $t_j$ の順で選ぶ。三重点側の $a=4n_j$ と $c=4n_j$ におけるmomentはそれぞれ $\pm\pi/n_j$ と比較でき、$I_j$ を狭くして全levelをdeep normal stripへ収める。全circle orbit・第二段の像・第一段の全trajectoryを共通plateauとneckの内側tubeに含められる。この共通collarの一致を、次の全intersectionの制御へ用いる。

Reduced graphに合わせて残余foliationをmomentに滑らかに依存させることは `ke:moment-dependent-neck-foliation` で許される。変更をsource・saddleの近傍とcollar外で恒等にすれば、閉pinched torusとsaddle fiberの型を保つ。固定 $t$ ごとの滑らかさでよく、無重みのmoment微分の一様な小ささは不要。残余基底は元の射影点 $p$ であり、$h_t(p)$ はsource近傍以外でglobal座標としない。Endのradial座標は $Z_{k,t}=C_D^2/h_{k,t}$ を使う。

`ke:neck-corner-saturated-union` はcorner cut $m_t=6b_j$ とneckの境界葉 $B=7b_j$ を分離する。先に $5b_j\le b\le9b_j$、normal深度 $\ge n_j/2$ の広い領域でnormal-first構成へ補正する。Neckの全normal trajectoriesはouter tube内にあり、frame差を引いてもlocal normal深度 $\ge3n_j/4$。Projected normal深度から旧plateauへの移行にはscaled Morse逆写像の粗評価と、固定annulus上で最後に選ぶ $t_j$ の条件を用いる。非incidentなtriple chartと二重線のouter tubesは最初に分離する。そこで $|d\log b(Y_N)|\le C/(n_jb_j)$ を使うfirst-exitにより、neck imageは $b<8b_j$ に留まる。Cornerの最小深度と元の射影の線形性から交点で $b\ge6b_j-C$ を得る。逆normal flowの自然性でmomentを同定した後にnormal深度 $\ge4n_j$ を結論する順序で、循環を避ける。Reduced graphと葉でのtrimから全intersectionが全torusで飽和し、source・saddleを含むactual部分fibrationとなる。End markingは共通torus同定に合わせて選び、任意に独立な第二periodの一致を含めない。この部分構成を `ke:actual-global-fibration` でcoreへ接着し、全曲面を覆った。

## Source reductionと全段階に共通なmarked tree

Sourceの幾何学的入力を `ke:source-reduction-pinched-fiber` にまとめる。固定 $t\ne0$ の $x'y'=th_t(p)$ では、canonical volume frameはsourceでも非零に延びる。Centered homotopyのchain primitiveは固定点で零なので、Moser場とflowもその点を固定する。正規化したnormal momentはそこで厳密に零であり、actual座標での商は $(\mu,p)\circ\phi_N^{-1}$ を用いる。Moser map自体が元の射影 $p$ を保存するとは仮定しない。

零momentの商は位相的には残余曲面であっても、source点で通常の滑らかなsymplectic曲面とは扱えない。標準product模型では $m=(|u|^2-|v|^2)/2$, $w=uv$ として reduced form は $\sqrt{m^2+|w|^2}^{-1}$ に比例し、$m=0$ で特異になる。この模型のDarboux座標がactual残余射影を保つとは主張しない。葉のliftのLagrangian性はambient接空間で直接示す。相異なるregular leavesにsourceを置く条件が、閉じたcritical fiberを一重pinched torusとし、branch fiberとの混在を除く。Normal orbitはprimitiveな消滅cycleである。Focusの局所型とmonodromy自体は既知であり、Zung, *A note on focus-focus singularities*, Differential Geom. Appl. 7 (1997), 123–130, §§2–4, Corollary 1（[一次原稿](https://arxiv.org/abs/math/0110147)）と照合する。異なる $t$ やstageのsemi-global symplectic不変量の一致は結論しない。Vũ Ngọc, Topology 42 (2003), Theorem 2.1（[一次原稿](https://arxiv.org/pdf/math/0208245)）の分類は、同じ単純focus型でもformal power seriesの追加不変量があることを示す。

`ke:fixed-marked-tree-exhaustion` は $D\setminus Q$ 上の一つのembedded marked pants foliationを最初に固定する。単純sourceは $t=0$ を含むparameter disc上で一価に追跡し、その小円板に支持を持つisotopyで運ぶ。全source葉とcritical pantsを含む固定compactの外にend graph補正を置くため、全stageと全ての十分小さい複素 $t$ で同じ標識付き木を使える。K3の相対葉族補間と全fiber単位のtrimもこの木を変えない。これは抽象木・source・成分labelsの固定であり、全torusの二つのcycleの族全体での自明化や、$t$ に滑らかな全域fibration族を与える主張ではない。

一般のMorse関数のpath componentが同じことだけから固定Reeb treeは従わない。Maksymenko, Comment. Math. Helv. 80 (2005), Main Theorem p.658 はpath components、Lemma 4.1 p.665 はgeneric KR-mapの同値を扱う。Regular annulusの葉を保つDehn twistは§6.1, Lemma 6.4 p.668（[掲載版](https://ems.press/content/serial-article-files/43060)）。本稿の固定木には、既に構成した実際の葉層のdiffeomorphismによる移送を使う。

## Source中央部の体積・momentとactual接続

正本は `papers/sections/paper/ke_source_connectors.tex`。$xy=tz$、$t=\tau^2$、$(x,y,z)=(\tau X,\tau Y,XY)$ として固定bidiscを使う。`ke:source-central-density` はdensityを $L^{-2}|dX\wedge dY|^2$ と両側比較する。下界はcapped canonical density、上界は正しいoriented gateのannulus–disc volume上界と中央の最大値原理による。Canonical potential $u_t=\log(\omega_t^2/|dX\wedge dY|^2)+2\log L$ は有界で $dd^cu_t=\omega_t$。射影を保つMorse座標にも適用できる。

`ke:source-central-moment` は同じcanonical primitiveで $|\mu_t|\le C/L$、固定点で $\mu_t=0$ を与える。Normal平均potentialの凸性と中央からoriented arm断面までの割線を用いる。Base-only変更はnormal momentを変えず、独立な加法定数の調整を行わない。`ke:source-central-mean-distance` は固定Euclidean体積に関するtrace積分と平均二乗ambient距離を $O(1)$ に抑える。部分積分と線分の二点積分による。ほとんどの点からなる部分集合の径は得られるが、全点・固定点・特定moment levelの径にはならない。

`ke:source-central-short-escape` はactual inradiusを $O(L^{-1/2})$ に抑える。Density上界から $\operatorname{tr}_{g_t}g_{\rm E}\ge cL$ を得て、大きさ $O(1/L)$ の非負Laplacian barrierを作る。Ricci下界による距離二乗のLaplacian comparisonと最大値原理で、全中央点からあるgateへの短い退出を得る。`ke:source-central-arm-connectors` はgateから正しいarm内を $s_x=\kappa L$ 又は $s_y=\kappa L$ まで進め、全費用を $O(1)$ とする。終点の残余座標・momentは指定しない。

固定連結source-free compact基底では `ke:fixed-base-central-band` により、固定 $A>0$、$m_t\to\infty$、$m_t=o(M_t)$ の下、$|\mu|\le A/M_t$ のcentral band全体がactual径 $O_{P,A}(1)$ を持つ。異なるmomentも含み、Moser像には $O(m_t^{-1})$ の端点費用だけを加える。両normal深度 $\ge\kappa_A M_t$ をmomentの片側下界から導き、水平・動径・円弧を組み合わせる。

Source側の `ke:source-central-band-reduction` は、固定residual disc、人工境界からの余裕、normal最小深度の下で、$|\mu|\le A/L$ の全点を固定rescaled coreへ $O(1)$ で接続する。この帰着と下記のGaussian体積比較により、中央帯の全点径は $O(1)$ となる。一般の同一moment集合についても、`ke:source-all-moment-exit` が指定した残余境界への退出条件 `ke:eq:source-moment-exit-input` を証明する。Central inradius、平均距離、全source fiberの径、長いnormal armsを含むneck全体の径を区別する。

`ke:source-potential-modulus` はGuedj–Guenancia–Zeriahi（参考文献キー `GGZDiameter`、Proposition 1.4）の局所距離評価を用いる十分条件を記す。Potential $u_t$ に一様な連続度 $m$ があり $\int_0^{r_0}\sqrt{m(r)}\,dr/r<\infty$ なら、固定coreのambient径は $O(1)$。このsquare-root-Dini modulusや一様Hölder評価自体はまだ証明していない。現行の $O(1)$ 径定理は下記のslab/Gaussian比較により無条件で得ており、このmodulusを必要としない。有界potentialから自動的に導いたり、同論文の大域Kähler class仮定を局所族へ無条件に適用したりしない。

## Source中央全点径：potential bufferとGaussian体積比較

正本は主稿の `ke:source-central-diameter` と `ke:fixed-base-source-central-band`。固定した $d$・族・residual基底について、固定点と座標軸を含む中央source全体のambient径は $O(1)$、正規化後は $O(R_t^{-1})$。Source-inclusiveな $|\mu_t|\le A/L_t$ の全中央帯と閉pinched torus全体にも拡張できる。追加のTCや一様Hölder仮定は使わない。

証明の依存順は次の通り。

1. `ke:source-tube-potential`：固定physical tubeをcentral coreと正しい二half-armsで覆い、actual densityとcapped densityを二側比較する。射影Chern–Luから $g_t\ge c g_{FS}$、nested physical tubesから固定actual bufferを得る。
2. `ke:positive-poisson-log-gradient`, `ke:source-potential-buffer`：非零正則frame $dx\wedge dy/t$ を固定した $u=\log(\omega_t^2/|\Omega|^2)+2R+C\ge1$ は $\Delta u=c_4$。Bochnerと距離cutoffで $|\nabla\log u|\le C$。中央点の固定小球では $u$ が有界となり、capsの積下界から両normal深度が $\kappa L$ 以上となる。縮小するrescaled bidisc内に球を閉じ込める必要はない。
3. `ke:source-shell-gaussian-tail`, `ke:source-wide-gaussian-tail`：固定source-free shellへのambient距離の $W_*^{1,2}$ normを有界potentialから抑える。Dinh–Marinescu–Vu, Theorem 1.2（参考文献 `DMVMT`）は固定補助Euclidean potentialに適用するので、actual potentialのHölder性は不要。$x=e^{Lw}$ の固定サイズcoverでは約 $L$ 個の周期を除して、広い中央帯のactual体積tailを $CL^{-1}e^{-aA^2}$ とする。
4. `ke:source-central-volume-anchor`：固定source-free residual annulusと $L/4\le s_x\le L/3$ のslabを取る。Density $L^{-2}$、logarithmic normal幅 $\asymp L$、一周期の角度から体積は $cL^{-1}$。Source-free中央帯の既存接続によりshellへの距離は $O(1)$ であり、sourceの全点径を入力にしない。
5. `ke:source-central-diameter`：距離 $D$ の中央点の小球は広い中央帯に入り、体積上界は $CL^{-1}e^{-a(D-\delta)_+^2}$。前項のslabと全曲面のRicci下界によるBishop–Gromov比較から、同じ球の体積下界 $cL^{-1}e^{-C(D+1)}$。係数 $L^{-1}$ が相殺し、$D^2\le C(D+1)$、全点で $D=O(1)$。

固定基底の残りはsource-free中央帯の $O(1)$ 接続でつなぐ。Canonical primitiveのbase-only変更はnormal momentを変えず、actual Moser像には両端の短いtrajectoryだけを加える。経路はfiber又はmoment level内に留まらなくてよく、intrinsic fiber径の主張ではない。全intervalの同一moment接続は次の結果で与える。木上のfiberとのtarget対応と全曲面のno-shortcutは別に扱う。Gaussian tailだけ、短円の長さだけ、又はMoser像のorbit直径だけで全点評価を結論しない。

## 全moment intervalのsource退出

正本は `ke_source_all_moment_connectors.tex` の `ke:source-arm-uniform-tensor`、`ke:source-direct-central-exit`、`ke:source-all-moment-exit`。中央帯・source軸・固定点を含めて、同じcanonical momentを持つ指定残余境界への退出費用は **$O(1)$**。経路自体はlevelに留まらなくてよい。固定stageの同一moment集合全体の径も $C+C_P$ 以下となる。定数は固定source chart・族・次数に依存するが、source退出の定数を残余exhaustion stageに依存させる必要はない。

核心は $xy=tz$、$s=-\log|x|^2$ の領域 $n_*\le s\le\kappa L$、$|z|\le\beta$ における $U=|d\log s|_g^2$ の制御である。Rank-one Bochner計算から $\Delta U\ge U(U-1)$。固定normal境界では射影下界から $U\le Ce^{n_*}/n_*^2$、残余境界ではsource-free tensor比較から有界、moving境界 $s=\kappa L$ では正のpotentialが有界なのでorientationを保つ固定半径のactual球を取り、localized Schwarzから有界となる。三境界の最大値原理で全armの $U$ が有界となる。

このnormal covectorの下支配と、射影下界による残余covectorの下支配を合わせ、cusp–disc積 $h$ に対して $h\le C\omega_t$ を得る。既存のvolume上界 $\omega_t^2\le Ch^2$ と複素次元2の固有値比較から $\omega_t\le C'h$。固定 $x$ で $z$ をshellへ動かす水平経路は有界長であり、momentとnormal深度の二側比較から最後の動径補正も有界長となる。

中央点は `ke:source-central-short-escape` の $CL^{-1/2}$ 退出でgateへ運び、短円の上界を積分して $s=\kappa L$ へ接続し、上の水平経路へつなぐ。従って全moment退出にも中央全点径にも、Gaussian可積分性を入力にしない証明がある。これは中央のtensor二側比較を主張するものではない。

**依存の順序。** Capped density・complete volume上界 → 射影下界・正のPoisson potential → orientationを保つactual球 → 境界Schwarz → arm tensor → 直接退出。固定normal境界の粗い上界にSong/Rochon–Zhangの成分収束は不要であり、full-triple比較・global sharp scalar評価・中央全点径をこの鎖の入力にしない。Source-free側面のtensor比較は、その独立なactual first-exit証明を使う。

深度 $S$ ごとのGaussian tailとgood slabの体積 $S^{-1}$ の評価は独立の補助結果として保持する。Positive potentialだけによる一般のscale bufferは半径 $c/(1+u)\gtrsim R^{-1}$ であり、moving境界 $s=\kappa L$ では $u=2\log(1/\kappa)+O(1)$ によって固定半径となる。この区別が三境界証明を非循環にする。Actual Moser像には両端の既存の短いtrajectoryを加え、同じcanonical momentを移送する。

## 旧corner値と全域基底のparameter化

正本は `ke_global_base_compatibility.tex`。`ke:common-edge-moment-profile` は全triple endsのcanonical momentを共通simplex profileと比較する。Moment誤差はnormal生成場の長さ $\mathfrak a$ を含む $O(\mathfrak a/m)$、normal longitude微分は $\asymp\mathfrak a$ なので、逆写像で重みが相殺し辺座標誤差 $O(1/(mR))$ となる。Momentの加法定数は既存primitive periodの厳密同定で固定する。

`ke:corner-cap-disk` は小さいtarget像だけからdisk構造を推論しない。閉linkのnormal facesとroundingを列挙し、joint momentの単調性で各cap境界が一本のproper arcであることを示す。この三capを取り除いたdiskを、各vertexの $O(\eta)$ 近傍内の境界延長でuncapする。さらにsimplex座標で一様にinsetし、残るannulusを3vertex panelsと3edge stripsへ分ける。Stripでは全枝共通profileと各end profileの単調補間を用い、core sectorでは境界homeomorphismをdiskへ延長する。

`ke:anchor-trimmed-neck-domain` は、共通anchorで残るneckを正確に $|\widehat\mu|\le\delta$ と同定する。Endでは残余momentが $\asymp b_j^{-1}\gg\delta$ なのでroundingが同じnormal cutへ厳密に戻り、真のrounding領域は残余深度 $\asymp N_j$ にあって旧neckの外である。各moment側の連結性から、区間外の尾部は対応するcoreの内部に全体として入る。平行linkとの差は変更collarに含める。これで $\sigma_t$ の定義域と全域被覆が一致する。

結果は `ke:global-base-parameterization` の全保持cornerにおける旧softmaxとの誤差 $C\eta$、各component core/変更collar像の頂点への $C\eta$ 近接である。$\eta=A(1+\log(N_j+1))/R_t$。`ke:collapsed-tree-common-moment` はcore近傍以外の $p_T$-fiberが厳密に同一moment上の内部木全体となることを別に保証する。`ke:neck-base-value-control` は全保持neckで辺値との $C\eta$ 近接、source critical valuesでは $e_i+e_j$ への近接を与える。

旧softmaxの閉辺にはregular torus fibersがある一方、全域基底のcellular辺はbranch locusである。従って全保持cornerでの厳密な値の一致は一般に不可能であり、insetによる一様に小さい誤差が適切である。位相同定だけからこの値の制御を結論しない。

## Component coreの固定段階移送と相対条件

正本は `ke_component_core_transfer.tex`。成分極限 $\omega_i^\infty$ へのfixed-gauge smooth収束から、$\beta_t=d^c\log((E_t^*\omega_t)^2/(\omega_i^\infty)^2)\to0$、$d\beta_t=E_t^*\omega_t-\omega_i^\infty$ を得る。固定compact上のMoserはactual変位・$C^1$誤差を $o_t(1)$ とする。$\beta_t$そのものがd-exactという主張ではない。

境界germを点ごとに保存するには、primitive差のcollar $H^1$ classがcoreの $H^1$ から延びることが必要となる。Fiber periodsが全て零でもbase-circle fluxが残る例を `ke:core-relative-flux-example` に保持する。これはfiber partitionの不存在例ではない。平均形式にもparameter方向の同変Moserを入れる $A_t b_t A_0^{-1}$ はexact symplectic germとなり、normal momentの加法定数も保つ。

`ke:component-flux-space` は $\mathcal O(K,S)=H^1(S;\mathbb R)/\operatorname{im}H^1(K;\mathbb R)\cong H_2(K;\mathbb R)$ を同定する。一般位置 $m=d-1$ 直線で $b_1(K)=m-1$、$b_1(S)=\binom m2$、$\dim\mathcal O=\binom{m-1}{2}=\binom{d-2}{2}$。Cohen–Suciuの既知のboundary cohomology（Proposition 2.5、Corollary 2.6、§6.9）の適用であり、独立の新規性は主張しない。境界でcoreへ消えるcycleのperiodが相対延長条件を検出する。`ke:nonextendible-small-core-germ` では非零障害を表すclosed form $a$ に対して $\iota_Y\omega=a$ と置く。小さいflowのfluxは $\epsilon[a]$ なので、同じactual KE形式を固定してもcore全体へ延長できないgermが恒等写像に任意に近く存在する。この障害は、自由に構成するfibration又は全葉partitionの不存在を意味しない。

`ke_component_core_geometry.tex` により、任意の固定compactと全collarでKE形式・primitiveに厳密一致するsmooth compactification、正residueの有限型KE core、その小さい飽和近傍のLagrangian fillingを得た。この局所core fillingの存在と、既存full collarの葉を保つことは別条件である。後述のactual link構成はその相対問題を解く。`comp:finite` の出力葉が指定葉に一致することは、二形式の一致だけからは従わない。条件付き系 `ke:conditional-component-core-filling` は、その入力があればactual移送・接着・十分遅い対角選択でcore全体の正規化径を消せることを示す。

## Saddle を動かす相対葉族補間

`ke_relative_reduced_foliations.tex` の `ke:simple-saddle-family-trivialization` と `ke:saddle-moving-relative-interpolation` を証明した。Compact reduced surface上のsmooth first-integral族を対象とし、各connected critical leafが一つのsimple saddleを含み、boundary collarの葉partitionとcontinuation markingが固定されると仮定する。全critical valuesの相異性は不要。各critical pants上でcritical-value速度に一致するglobal basic関数ζを作り、∂μf+df(Y)=ζ、dζ=a dfを解く。これにより全critical leavesと全regular annuliを同時に同定し、anchorで一致する二族をmoment cutoffで補間できる。異なる値のfirst integral表示を一致させる必要はない。

`ke:actual-saddle-moving-neck-interpolation` は自由Hamiltonian normal bandへ持ち上げ、actual Lagrangian性とS¹×figure-eight、全corner葉、normal markingを保つ。補間はsourceのcritical momentから離して行うためcentral pinched torusを変えない。Liouville moment M=μ−ρの場合、時間は s(μ)=log((μ−ρ)/(μ*−ρ)) で再parameterizeする。この葉族補題は別担当と内部点検済み。全link被覆・primitive補正・coreの全域接着は次節の別の証明で確認した。この葉族補題単独の帰結ではない。

## Actual core の全域相対接着

**主稿 `ke:actual-global-fibration` に証明を統合し、追加証明を別担当と内部点検した。** 任意の固定 $d\ge5$ と既存一般性条件の族について、K2の部分fibrationから全 $X_t$ 上のactual KE–Lagrangian fibrationを構成する。Markingの組合せ型を保ち、第二作用やcritical valuesの数値は先指定しない。全曲面の距離歪みはこの構成定理の結論ではなく、`ke:global-ambient-lower` と `ke:global-ambient-upper` の別の証明で扱う。

### 正確な period と閉 link

正本は `ke_component_link_cover.tex`。Positive-residue primitiveの周期1 meridian積分を $M_a$ とすると、$q_a=M_a+2\pi w_a$ は既存canonical normal momentの向き付き値と**厳密に**一致する。有限直線ではlog volume frameとの比の単純極、無限遠ではaffine volumeの3重極とlog volumeの単純極の差を使う。Holomorphic unitのwindingは固定collar上のhomotopyで零。非正則な座標補間では $G^*\lambda$ を使い、$G^*d^c=d^cG^*$ としない。

残余尺度 $b_j$、normal cutoff $n_j$、共通幅 $\iota_j$ の後で $N_j\iota_j\gg1$ と $N_j\gg n_j$ を選ぶ。$\delta_j=4\pi/N_j$ のnormal moment facesを取り、cornerでは $(q_a-\delta_j,q_c-\delta_j)$ のsmooth monotone minimumで丸める。Corner momentは全深度比に一様に $4\pi/s_a$ と比較できる。重複帯ではresidual momentが $1/b_j\gg\delta_j$ なので丸めは作動せず、normal faceと厳密に一致する。深さを近似的に合わせた切断ではない。正のresiduesにより $M_a=q_a-2\pi w_a<0$、不変primitiveのLiouville場はこのlinkを外向きに横断する。

### 固定段階でも全特異層を覆う理由

`ke:fixed-stage-stratum-coverage` は、同じcentered normal Moser flowをさらに深い**固定**tubeへ制限する。FlowはODE一意性で元のものと同一である。Fixed-shell momentの下界だけでは足りず、$|\mu|\le C_P/M<\iota_j$ の上界と逆像bufferを用いる。Source基底点もcomponent側cusp shellでは通常の滑らかな点なので含む。残余は $6.5b_j$ まで、cornerのactual imageはphysical最小深度 $6.3b_j$ から覆い、端のgapをなくす。粗い $\min\ell>2m=12b_j$ の包含だけではneck cut $7b_j$ との間が残る。

中央の全特異locusの固定ambient近傍を覆うので、部分fibrationの外部は各 $W_i$ の互いに素な固定compactのgraph imagesに入る。閉linkをその外側へ置けば全域被覆を得る。境界が全fiberで飽和し旧fiberが連結なら、そのfiberは内外を横切れない。これが `ke:whole-fiber-core-trim` の全fiber単位の切詰めである。

### Invariant primitive と nontrapping

正本は `ke_core_invariant_primitive.tex`。短円の0次評価からgeneratorの一階評価は出ない。Normal logarithmic chartでbare generatorを深度逆数の定数場として書き、RZの全cusp微分からMoser mapをC2まで制御する。Cornerも比較Hamiltonianを一階高めてC2flowを得る。必要なactual actionsで $|V|+|\nabla V|\le\varepsilon_j$、$\varepsilon_j=C_*/b_j+C_j/N_0$ となる。

Actual symplectic circleのcentered kernelについて
\[
 F=\int_0^1(1/2-s)\lambda(V)\circ R_s\,ds,
 \qquad\mathcal A\lambda-\lambda=dF,
 \qquad |F|+|dF|\le C\varepsilon_j H
\]
が成り立つ。$K\omega=0$ がexactnessの理由である。Common normal action上では $F_C-F_N$ が不変なので、source torus label $B/b_j\in[5.2,5.4]$ の帯でnormal-invariantに貼る。Retained cornerに達する前にfull torus gaugeへ切り替える。$\eta(\Psi/N)$ の零延長支持全体は広いnormal/corner construction domainsで覆える。保持されたsoftmax領域だけを作用の定義域と誤認しない。

正residue potentialは $|d\Psi|\asymp H$、$Z_0\Psi\ge cH^2$ を満たすため、補正後も $Z^{\rm ad}\Psi\ge(c-C\varepsilon_j)H^2>0$。Core外に新しいtrappingを作らない。Actual形式では先に固定compactのexact Moserを行い、$\lambda_{\rm int,t}=(\varphi_t^{-1})^*\lambda_0$ をactual actionsで平均する。Canonical positive-residue gaugeとの差はexactなのでperiodsを保つ。二形式を合わせる前のprimitive差をexactとみなしてcutoffしない。

### Cone filling、相対補間、費用

正本は `ke_actual_core_gluing.tex`。各linkのquotientは、normal facesの木 $T_{ij}$ の標識endをcorner annuliでつないだgraph $\Gamma_i$。Contact formを変更せず、compact Liouville domainの $K\setminus\Sigma\simeq(-\infty,0]\times S$ に対し $\Pi(\varphi_s(y))=[e^s,\pi_S(y)]$ とする。有限退出時間とcompactnessがcone pointでの連続性を与える。これはEvans–Mauri Lemma 2.16のcompact版であり、既存のcone原理自体を新成果とはしない。

`ke:contact-rescaling-collar-scope` は、contact構造の一致と指定葉の一致を分ける。$\beta=\cos z\,dx+\sin z\,dy$ on $T^3$、$F=\{z=\pi/2\}$、$h=\sin x$ では $d\beta|_F=0$ だが $d(e^h\beta)|_F=e^{\sin x}\cos x\,dx\wedge dy\not\equiv0$。Evans–Mauriのcompletion間の点依存radial shiftは固定linkを保つ主張ではない。本稿のcompact coneは入力のcontact form自体を保つ。

外向きcollarのLiouville葉族は一般には旧neck葉族と異なるため、前節の相対補間を $q_a=\delta_j\ne0$ の小帯へ適用する。全corner葉とsource近傍を保ち、saddleは動かせる。全fiber trim後のclosed piecesでlocal fiber relationsの有限和は既に推移的なので、閉同値関係となりHausdorff基底を得る。基底は同じ $B_d(T)$。

相対補間の恒等end collarsは全K2交わりを含む。Source labelの切替が $B\le5.4b_j$ で終わり、全交わりが $b_{\rm res}>5.5b_j$ にある余裕を使う。切詰め対象は補間後の $\widetilde f$ である。共通Liouville band内に $S^-=\partial K^-$ を取り、coreは元の $K$、外側は $U\setminus\operatorname{int}K^-$ とする。平行moment linkは補間後も全fiberで飽和し、重なるcollarでは同じ全葉になる。指定component compactsを $\operatorname{int}K^-$ に残すことで全域被覆も保つ。基底分割は元の共通anchorへ戻せる。

`ke:component-logarithmic-connectors` により、各componentのcore・変更collarの接続費用とambient径は $C(1+\log(N_j+1))$ で抑えられる。$C$ は固定した族・charts・weightsのみに依存する。全深度が $CN_j$ 以下であることと固定componentのcusp上比較を使い、normal動径の積分 $\int ds/s$ で固定compactへ結ぶ。全経路は $\{\Psi_i\le AN_j\}$ に入り、この拡大compactを先に固定してからactual metricを比較する。これは**各componentごとのambient評価**であり、異なるcores全部の合併径や任意Liouville軌道の全長、fiber内在径は結論しない。

Skeletonの連結性は $\Sigma=\bigcap_{T\ge0}\varphi_{-T}(K)$ というnested compact connected setsの表示から直接従う。保持cornerのquotientがdiskであることとproper cap arcsは `ke:corner-cap-disk` を用い、$B_d(T)$ の同定との循環を避ける。対数接続補題は別担当も独立に導出・点検済み。`ke:compact-relative-morse-smale` は境界とcritical germsを保つ小さいcontact holonomy変更とexact Moserにより、同じKE二形式上のprimitiveをMorse–Smaleにする。Stable manifoldsのclosureは低いindexにのみ落ちるため、次元順の閉isotropic filtrationが得られる。Whitney条件は主張しない。Cone fillingでは開辺上のsmooth submersionも明記した。

### 全接続予算の選択順序

旧softmax辺の全体で $B=m_j+r_c$、$0\le r_c<1$ なので、全marked tree・source discs・portal端を含む $P_{ab,j}\Subset P^+_{ab,j}$ は $N_j$ より先に固定できる。同一moment接続定数を $C_j^{\rm neck}$ とする。`ke:component-neck-tail-depth` は $q_{\rm act}=q_{\rm raw}\circ\phi_N^{-1}\ge4\pi/N_j$ の成分側尾部の裸の逆像に $s\le2N_j$ を与え、同じcentered flowの浅い固定compactと深いtubeへの制限を分けて、actual像も深度 $CN_j$ に入れる。深い側のfirst-exitには固定componentの $|d\log s_a|\le K$ と全normal/residual buffersを用いる。

従って、まず $H_j\le C(1+\log(N_j+1))+C_j^{\rm neck}$ が得られる。許容cutの下限に $C_j^{\rm neck}\le1+\log(N_j+1)$ を加えれば
\[
H_j=C(1+\log(N_j+1)),\qquad
U_{j,t}\le C_d\left\{b_j^{-1}+\frac{1+\log R_t+\log(N_j+1)}{R_t}\right\}
\]
とできる。これは残余定数のexhaustion増大率の解析評価ではなく、選択順序による吸収である。Scalar補助cutの増大率とfixed-compact収束の閾値も未評価であるため、最適な全域rateは結論しない。経路はambientであり、同一momentやfiberの内部を通る必要はない。

### 主要接着依存の点検範囲

Centered averageの $K\omega=0$、二作用の $F=K_1\lambda+A_1K_2\lambda$、common normal上の $V(F_C-F_N)=0$ を直接確認した。GeneratorのC1評価にはmapのC2が必要であり、既存C5入力からの微分階数を確認した。切替え帯 $5.2b_j$–$5.4b_j$ は広い構成域 $\min\ell>3b_j$ とnormal-first plateau $5b_j$–$9b_j$ に入り、実交点 $5.5b_j$–$8b_j$ までにfull torus gaugeへ移る。支持全体の被覆、先行するexact Moserとperiod保存、$Zq=q-\rho<0$ の向き、全fiber trim、相対葉族の境界germとcritical-leaf marking、閉quotientを読み合わせた。今回のcore経路の監査は、正則化・exact Moser・actual平均・同じmoment cut・相対補間・補間後trimの構成の同一性と量化に範囲を限定して完了した。SNC構成にも同じcompact-relative Morse–Smale補題を適用し、閉isotropic filtrationを明示した。これは全旧局所証明の包括的再監査ではない。

### 切り取った cap と旧 softmax 値

`ke:core-depth-upper` は、固定componentのstrictly plurisubharmonic potential $\Psi_i=\sum_aw_as_a-2\sum_a\log s_a+O(1)$ を使う。Link上の深度が $CN_j$ 以下なら、$E_{i,t}^{-1}(K_{i,j,t})$ における最大原理と $\Psi_i\ge c\sum_as_a-C$ からcore全体でも同じ上界が得られる。ここではLiouville補正後のpotentialを要求しない。Graph gaugeはこの固定compact上で最後に $t$ を小さく選び、corner逆写像のlog-depth変位から乗法的に比較する。

境界のactual移送はnormal facesとcorner roundingを分ける。Normal facesでは先に得たMoser長 $C_{P_j}/N_j$ と、拡大した固定graph compact上の $|d\log s_a|\le\sqrt2K$ により、深度が初めて倍になる退出を排除する。$N_j$ は $C_{P_j}$ の後、graph比較に必要な $t$ 閾値は $N_j$ の後で選ぶ。Cornerでは既存のlog-depth変位を使う。境界の上界の証明にcore全体の上界を先取りしていない。

`ke:removed-corner-target-cap` は、$x\in K_{i,j,t}\cap W_{t,J}$ に対して
\[
 d_\square(P^{\rm old}_{t,J}(x),e_i)
 \le\eta_{j,t}:=\frac{\sqrt2\log(CN_j)}{R_t}
\]
を与える。各capの径は $2\eta_{j,t}$ 以下で一様に消えるが、異なる成分cap全体の合併径は消えない。実際に構成したcompact coreだけを扱い、full corner全体のmoment不等式の解集合を同じcoreと同一視しない。

保持corner $A_{t,J}$ の旧projection像は $2\eta_{j,t}$-netであり、旧protected距離の制限を用いたGH誤差は $E_{j,t}/2+2\eta_{j,t}$ 以下。全曲面距離の上界にも旧cornerの経路を使える。一方、保持部分自身の新しい内在距離の上界にはcapを避けるdetourが必要で、全曲面距離の下界にはno-shortcut評価が必要である。

全域基底が $B_d(T)$ と同相で、保持cornerのtorus partitionが一致しても、特定の基底parameterizationで $p_T\pi_t=P^{\rm old}$ とは限らない。`ke:global-base-parameterization` はcore側のcone sectorsを上のvertex capsへ送り、全保持cornerで旧softmax値との一様に小さい誤差を実現する。小さいactual径だけから、任意のtarget parameterizationで像も小さいとはいえない。

## Source の residual cutoff と Euler 場

`ke:source-euler-bound` は固定source tube上のEuler場 $W_+=x\partial_x+y\partial_y$ をactual norm $O(1)$ に抑える。固定normal境界はcomponent KE収束、固定residual境界はsource-free tensor比較で評価し、内部へBochner最大値原理で延ばす。中央点で $|z|\ge e^{-a_t}$、$a_t=o(R_t)$ なら正の同時scalingを $O(a_t+1)$ 時間で固定residual shellまで進められ、終点はcanonical central moment帯にある（`ke:source-sublog-residual-connectors`）。この経路だけでは $z=0$ と $|z|<e^{-a_t}$ を制御しない。以下の別の体積比較で全点評価へ進む。無限のscaling時間を有界な経路長に読み替えない。

## 二段階平均によるnormal actionとperiodsの接続

正本は主稿 `papers/sections/paper/ke_staged_neck_averaging.tex`。証明全文はここへ重複させない。`ke:circle-exact-transport` / `ke:staged-neck-averaging` は、ω=dλに対してnormal circleを先に平均し、残る円の平均をnormal-equivariantに行う。η=A1ω、κ=A2η、φ*ω=η、ψ*η=κなら、Θ=φψは
\[
 \Theta^*\lambda=A_2A_1\lambda+dq,\qquad
 \mu\circ\psi=A_2\mu,\qquad
 \widehat\rho_1=\phi\rho_1\phi^{-1}
\]
を満たし、全整数cycleのperiodsを同じprimitiveで規格化する。Periodは1、ι_Vω=−dμの規約。Normal actionが一致しても、別に指定したneck fibrationの第二periodやreduced leavesは自動的に一致しない。

`ke:staged-hamiltonian-comparison` はpositive triangle (1−u)κ+(u−v)η+vω、0≤v≤u≤1内のpath homotopyを用いる。各endpointがprimitiveを同じ平均primitiveからexact差まで保つため、そのsmooth familyがHamiltonianとなる。共通domain bufferに加え、F_r(D_small)⊂F_0(D_large)というimage bufferが必要。Exact endpointだけを根拠にしない。`ke:staged-closed-corner-gh` は任意の固定primitive subgroupを第一段に選んでもO(log R/R)の局所GH率を保つ。旧bundleとの関係は、同じsoftmax labelsのfibersを対応させるHamiltonian mapである。

関連KE主稿 `pair:prop:bundle-conic` は、射影的normal bundleでh=−F_d/G、x_i'=x_i h0/h、x_j'=x_jとしてexact uv=tを得る。局所overlapをcomplete C* automorphismとする不十分な議論を使わない。(u,v)↦(ue^u,ve^(−u))はuvとaxesを保つlocal mapだがbase-only乗数ではない、という例を覚えておく。新構成もfixed compact baseに限り、tripleへ動くbaseのtransition boundsを含まない。

同稿 `pair:cor:global-primitive` / `pair:cor:actual-common-moment` は、source-free固定base B上で非消滅正則1-form τを選び、Ω=dlogv∧τからglobal λ_tを得る。Canonical normal momentはτの変更で変わらないが、residual periodsには同じprimitiveを使う。Song (arXiv:1706.01518, Lemmas 4.4–4.5)とRochon–Zhang (arXiv:1106.0873, Theorem 5.1)の固定end入力から、μ_tの端値は±4π/s_r+O(s_r^(−1−δ))+o_t(1)。rを固定後t→0とし、η_t=A1ω_tのreductionsの共通intervalを確保する。

`ke:short-circle-actual-buffer` は不変背景を不要にする。g_a=ρ_a*g_ω、η=Aω、b=ε||w||₂とすると|β(X)|≤b|X|_{g_η}。Moser場は(1−s)|Y|²_η+s|Y|²_ω≤b|Y|_ηを満たし、平方完成で|Y|_ω≤b/(2√(s(1−s)))となる。両向きtrajectory長はc_w ε、通常kernelでc_w=π/(2√3)、centeredでπ/(4√3)。Exactnessは長さ評価に不要。`ke:short-circle-image-buffer` はδ>(2c_w+1/2)εから、同じcompact飽和集合Kを含むsource Oとimage φ(O)を得る。Backward c_w ε＋半orbit ε/2＋forward c_w εの予算であり、conjugated actionを元のK上で使うための像の条件を明示した。C¹制御やintrinsic径、全neckでの仮定検証とは別。

遅いexhaustionでflow生存・共通bufferとtriple endsの葉の一致は実証した。全域被覆・core接着は `ke:actual-global-fibration` で証明した。特異領域を含む全点の距離評価は、sourceの全moment退出とscalar/portalの各節で別に証明した。KE側 `neck:lem:rank-one-circle` はresidual rank-one下界とvolume上界だけでnormal circle長を抑えるが、その下界とactual bufferを証明する必要がある。固定residual境界の影響が消えないexact negative KE productの例があるため、normal深度だけからproduct asymptoticsを推論しない。


## 全深部三重点の actual semi-flat 比較
任意の固定次数 d≥5 の一般位置全平面退化で、三重点の全深度比・全角度に一様な actual KE 比較を証明した。正確な座標 ζ0ζ1ζ2=t、ell_i=−log|ζ_i|²、L=−log|t|²、R=log L とし、k_Lをlogarithmic simplex上のcomplete toric KE form、その実計量をg_L^sfとする。十分大きい固定m1と各qのCqについて、m≥m1、min ell_i≥mで
\[
\left|\log\frac{\omega_t^2}{k_L^2}\right|\le C/m,\qquad
\|g_t-g_L^{sf}\|_{C^q}\le C_q/m.
\]
定数は固定dと族に依存してよい。次数一様性は主張しない。証明の正本はKE主稿 `coarse:thm:full-triple-tensor`。

固定toric模型の存在・完備性にはZhang (2015), §2.1, Theorem 2.1 / Proposition 2.2を用いる（退化族のTheorem 2.4とQ-factorial仮定は使わない）。ψ_L=log L−Σlog ell_iに対してψ_L−(log3)/2≤φ_L≤ψ_L、V_L/3≤k_L²≤V_Lを内外にずらした障壁で証明する。Complete模型から三つの半平面へのYau Schwarz lemma、determinant比較、内部正則性により一様cusp geometryを得る。凸性からfacet shiftのlog-density差をO(1/min ell)とし、actual計量を内外のsimplex KE metricsでvolume比較する。Savinの小摂動定理でtensor・全高階誤差へ移る。Actual metric bufferや(TC)/(PBE)を前提としない。

Actual側の大域入力は `coarse:cor:degree-d-volume-lower`。Adjunction residueでcanonical densityを固定し、backgroundによるHermitian frame errorの吸収と各正のcap方向のminorから六型のdeterminant下界を証明する。Sourceでは元のplane coordinatesを保つexact xy=tzとrescalingにより二つのcap係数≥c_d/Lを使う。Compact minimum原理からactual volume下界を得る。この依存部分の証明と適用条件はKE側の原稿に明示されている。現行整備ではその所在と仮定を確認し、全証明の独立再監査は行っていない。


## Complete simplex模型の境界での鋭い比較
KE主稿 `papers/sections/simplex_boundary_geometry.tex` が正本。`simplex:lem:rank-one-schwarz` は、complete模型から各半平面への正則写像にYau Schwarz lemmaを適用して
\[
|d\log\ell_i|_{(g_L^{\mathrm{sf}})^{-1}}\le1
\]
という係数1の評価を与える。粗いtensor比較によるtraceの有界性とcomplete最大値原理を使うので、深度比・全角度・正の深度に絶対的下限を設けず有効である。

`simplex:prop:dominant-product` ではa=ell_j、b=ell_k、δ=(a+b)/Lとして
\[
1\le\frac{k_L^2}{\omega_{\mathrm{prod}}^2}
 \le\left(\frac{\pi\delta}{\sin(\pi\delta)}\right)^4,
\qquad
g_L^{\mathrm{sf}}-g_{\mathrm{prod}}=O_{C^q}(\delta^2)
\]
を示す。下比較はexpanded quadrant、上比較は辺長La/(a+b)、Lb/(a+b)のrectangleによる。境界がsimplexと接するrectangleは内部へ縮めて比較してから極限を取る。固定product balls上では深度が中心と固定比の間にあり、potentialの小ささO(δ²)が保たれる。Angular coverを双曲平面二つの積の固定正則座標へ正規化し、Savinと線形化後のSchauder評価で同率の全固定階比較を得る。

`simplex:prop:facet-product` は、一深度bがd_*=min(a,L−a)に比べ小さい場合に、cuspと幅Lのcomplete annulusの積p_Lを比較相手とする。内側rectangleの幅βを(b²d_*)^(1/3)とし、volume-potential誤差
\[
C\bigl((b/\beta)^2+\beta/d_*\bigr)
 =O((b/d_*)^{2/3})
\]
を固定p_L-ball全体で評価する。Actual側にはO(1/b)を加える。`simplex:cor:active-cogram` はell_i≤L e^−Aのactive covectorsについて、二方向ならco-Gram誤差O(e^−2A)、一方向を含む一様評価ならO(e^−A/2)を与える。Actual側はO(1/min ell)を加える。閉cornerの距離下界には、一方向のexact Schwarz評価と二方向のdominant比較だけで足り、facet比較を追加依存としない。


## 同じactual Lagrangian bundleによる全閉cornerのGH極限
正本は `papers/sections/paper/ke_closed_corner_gh.tex`。Lagrangian主稿 `ke:actual-closed-corner` で構成した同じMoser flow φ_tと同じbundleを用いる。m=Rとし、
\[
\ell_a(w)=R+(L-3R)\frac{L^{w_a}}{\sum_bL^{w_b}},
\qquad
\mathcal C_J=\{w\in[0,1]^3:\max w_a=1\}
\]
のhexagon全phase preimageをH_t、そのMoser像をW_{t,J}、射影をπ_{t,J}とする。`ke:closed-corner-gh` と `ke:closed-corner-protected-gh` は、R^−2 g_tの二つの距離に対して
\[
\operatorname{dis}(\pi_{t,J})\le C\frac{\log R}{R}
\]
を証明する。一つはW_{t,J}内の経路による内在距離、もう一つはV_t={min ell_a>R/2}内の全経路を許した距離をW_{t,J}へ制限したもの。標的d_Jは三枚のunit squares自身の内在距離として定義され、`topo:coordinate-retraction` により全C_dの距離の制限と等しい。Source側で全曲面の経路を許す下界は `ke:global-ambient-lower` で別に証明した。

模型の証明はKE主稿 `simplex:thm:closed-corner-model`。S=R−2 log Rとし、Ψ_a=[log(ell_a/R)/S]_0^1とclipする。最大深度≥L/3からΨの像はC_Jに入り、微分がactiveなのは高々二方向である。一方向では係数1のSchwarz評価、二方向ではell_j+ell_k≤2L/Rからsharp product比較を使い、complete simplex全体の全経路の長さ下界を得る。上界ではC_Jのgeodesicを高々三枚の異なるsquares内の直線分で実現し、各線分を幅4 log R/Rだけ内部へ移す。Sharpな内部比較とcoarseな短いconnectorsを合わせて同じ率を得る。Seam collarが薄いことだけを下界の根拠にはしない。

Actual/model比較O(1/R)に加え、Moser場のC1評価からmodel計量のLie derivativeを直接抑え、φ_t^*g_t=(1+O(1/R))g_L^sfを得る。保護領域内の全経路を扱うときは、Moser trajectoryのmodel長さO(1/R)とΨのLipschitz定数O(1/R)から、端点誤差d_J(Ψφ_t(z),Ψ(z))=O(R^−2)を用いる。これにより、閉cornerのfibrationの射影そのものがGH approximationになる。

全fiberのintrinsic/ambient diameterはO(1/R)、正規化後はO(1/R²)、raw-map誤差はO(log R/R)。Squareの共通辺と共通頂点でも同じregular T² fiberである。これらを既存大域fibrationのsource・branch・coreのsingular fibersとは同定しない。全曲面の被覆・core接着と、$V_t$ 外を通るshortcutの下界は、それぞれ別の証明で確保した。新規性の網羅的確認と外部査読・形式証明は未実施。

一般のcut $m_t\to\infty,\ \log m_t=o(R_t)$ についても、同じsoftmaxとMoser mapの射影が局所GH近似になることを `ke:slow-cut-closed-corner-gh` で証明した。内在・protected距離のdistortionは $C[m_t^{-1}+(\log(m_t+1)+\log R_t)/R_t]$、fiberの元の尺度の内在径は $C/m_t$。内部squareを幅 $\delta=(\log(m+1)+4\log R)/R$ だけ縮め、pruningでは $S=R-\log m-\log R$ を使う。$m_t$のparameter微分を使わず、stepwiseな遅いexhaustionにも適用できる。この遅いcutを `ke:neck-corner-saturated-union` の対角選択へ用い、actual core接着と全域距離評価へ組み込んだ。


## 開正方形上のactual KE–Lagrangian collapse
主稿 `papers/sections/paper/ke_open_cell_collapse.tex` は、任意の固定次数d≥5、固定0<η<1/2についてKη=[η,1−η]²上の局所結果を与える。関連KE主稿 `simplex:cor:actual-dominant-product` により、独立深度a,b∈[L^η/2,2L^(1−η)]ではproduct-cuspとの誤差は全固定階でO(L^−η)である。模型側O(((a+b)/L)²)とactual側O(1/min ell)を合わせた率であり、global capped volume下界、complete模型の上下比較、Savin正則性に依存する。(TC)_dや(PBE)_dは追加仮定しない。

`ke:open-cell-moser-c1` はchain primitiveとMoser場のC1 normをO(L^−η)とし、flowのpullback metricを制御する。`ke:open-cell-collapse` はactual Lagrangian T² fibration、fiberのintrinsic/ambient diameter O(L^−η)、raw-map誤差O(1/R)を与える。Moser像領域に内在長さ距離を入れると、R^−2 g_tは平坦KηへGH収束し、projection distortionはO(L^−η+L^−η/R)=O(L^−η)。定数は固定ηに依存する。

開正方形と全閉cornerの局所結果、source・saddleを含む部分fibration、coreへの全域接着、全曲面ambient距離の比較を区別する。現在は各段階の証明を `ke:global-metric-realization` に統合している。局所GH評価だけを全域distortionの根拠にはしない。


## 負KE計量のGH極限とfiber収縮

### 二つの尺度と先行定理
全平面退化は $X_t=\{\prod_iL_i+tF_d=0\}\subset\mathbf P^3$、$d\ge5$ とし、$F_d$ は三重点で非零、二重線上では単純零点を持つとする。$\operatorname{Ric}(\omega_t)=-\omega_t$ の規約では $[\omega_t]=2\pi(d-4)H$、$\operatorname{Vol}(X_t,g_t)=2\pi^2d(d-4)^2$ である。複素構造を固定したままの負KE計量はこの規約で一意であり、ここで動かすのは複素構造である。

Song, arXiv:1706.01518v1, Theorem 1.2（https://arxiv.org/abs/1706.01518 ）の適用：中央fiberはSNCでslc、相対canonicalは $\mathcal O(d-4)$ でample、全空間は $xy=tz$ 型ordinary double pointsを持つnormal canonical varietyなのでstable degenerationの仮定を満たす。成分内部に基点を置く非崩壊極限は $d$ 個の $\mathbf P^2\setminus\{d-1\text{本の直線}\}$ の完備有限体積KE曲面である。これはcore skeletonではなく四実次元の開曲面である。Song–Sturm–Wang, arXiv:2003.04709v1, Theorem 6.1（https://arxiv.org/abs/2003.04709 ）もstable familyの多点付き極限を扱う。すべての基点列が非崩壊だという意味ではない。

Zhang, *Collapsing of negative Kähler–Einstein metrics*, MRL 22 (2015), 1843–1869, DOI 10.4310/MRL.2015.v22.n6.a16, arXiv:1505.04728v2, Theorems 1.1/2.4は、Q-factorialなsimple toroidal total spaceと相対canonicalのamplenessの下で、stratumへ動かす基点における局所torus collapseを示す。曲面では二重曲線でS¹、三重点でT²が縮む。主稿 `intro:ke-collapse` に比較を収録した。我々のsourceの局所環 $\mathbf C[x,y,z,t]/(xy-tz)$ はQ-factorialでない。Small resolutionはcrepantなのでexceptional $\mathbf P^1$ 上の相対canonicalの次数は0となる。従って「小解消すればZhangをそのまま適用できる」とは言えない。

Mandel, *Degenerations of negative Kähler–Einstein surfaces*, JLMS 109 (2024), e12818, DOI 10.1112/jlms.12818, arXiv:2206.09792, Theorems 1.1–1.2は負KE neckとその尺度別模型を構成するが、我々のcompact family全体へのgluingを完了した定理として引用しない。K3での対照例はGross–Tosatti–Zhang, CAG 24 (2016), 93–113, DOI 10.4310/CAG.2016.v24.n1.a4, arXiv:1304.1820, Theorem 1.1。楕円K3の適切なRicci-flat metric族が底へ崩壊し、hyperkähler rotationでspecial Lagrangianの解釈を得る。負KEに同じ結論を移す証拠にはしない。

Fu–Hein–Jiang, *A continuous cusp closing process for negative Kähler–Einstein metrics*, GAFA **35** (2025), 542–632, DOI [10.1007/s00039-025-00708-y](https://doi.org/10.1007/s00039-025-00708-y), §1.1 Main Theorem は、孤立楕円特異点へ退化する六次曲面のactual負KE計量とTian–Yau bubbleを扱う。掲載本文の定理と対象族を確認した。全平面SNC退化の全域Lagrangian射影による径の尺度の比較とは区別し、本稿の解析入力には用いない。91頁の接着証明全体を再監査したものではない。

Fernández de Bobadilla–Pełka の [最終preprint arXiv:2312.13248v4](https://arxiv.org/html/2312.13248v4), Theorem 6.14・Example 5.8・Introduction・Remark 7.4を照合した。Theorem 6.14(b)のivy-like Lagrangian fibrationは境界・角付きの余次元零部分領域に定義される。一方、(c)のGH収束は $W_h$ 全体を扱い、退化写像がproperなら $W=X$ と取れるため、全nearby fiberと未被覆部分の対の収束である。従ってGHの結論まで部分領域だけに限定しない。そこでのKähler形式 $\omega_q^\varepsilon$ はexact補正で構成する補助形式であり、actual KE形式とは同一視されない。本稿との比較では、全域へのcore fillingと、指定されたactual計量への定量的比較をそれぞれ明示する。

同論文Remark 5.9（PDF p.25）はexpanded skeletonのramification locusとouter boundaryを除く領域の作用affine構造を記す。Evans–Mauri [arXiv:1905.09229v3](https://arxiv.org/html/1905.09229v3) Remarks 2.11–2.12はcontact作用積分とsymplectizationでの $e^r$ 倍を作用座標にする。正則域のaffine構造やLiouville同次性そのものを新規とせず、本稿のactual periods・全branch/core接続・同じ射影の距離評価と比較する。

直結する後続情報として、2026年11月12日のMakの [IMJ-PRG講演概要](https://www.imj-prg.fr/tga/sem-ga/archives.html)を2026年11月22日に確認した。Matessi–Ruddat–Zharkovとの共同研究で、reflexive polytopeに対応するtoric Fano内のCalabi–Yau hypersurfaceのLagrangian fibration、ironing coefficientsとEvans–Mauri型Liouville flowを説明している。完成論文の定理・証明を確認した記録ではなく、actual負KE曲面への適用根拠には使わない。

同一classのMoser移送 $\phi_t^*\omega_t'=\omega_t$ は、複素構造を固定した計量の比較を含意しない。$\phi_t^*g_t'=\omega_t(\cdot,\phi_t^*J\cdot)$ と $g_t=\omega_t(\cdot,J\cdot)$ の差を制御する必要がある。本稿は小さい局所移送とscalar/portalの直接評価を用いる。文献間でKähler class・Lagrangian性・actual距離の三条件をまとめて同一視しない。

### Diameter-scale極限とactual fibrationによる実現
KE研究の `papers/cubical-gh-limit.tex` では $R_t=\log(-\log|t|^2)$、$\mathcal C_d=\{w\in[0,1]^d:\max w_i=1,\ |\operatorname{supp}w|\le3\}$ とし、$(X_t,R_t^{-2}g_t)\to(\mathcal C_d,d_\square)$ を **(G)$_d$+(CP)$_d$+(PBE)$_d$の下**で述べる。これらの条件付き定理の正本は関連repoの現行方針・Part IV–Vである。本稿の `ke:global-metric-realization` はscalar下界とportal上界による別の直接証明を与え、CP/PBE/TCを検証したとはしない。

局所plumbingのモデル $z_0z_1z_2=t$ で $u_i=-\log|z_i|$、$L=-\log|t|$ とすると $\sum u_i=L$。Cuspのradial model $\sum (du_i/u_i)^2$ を $(\log L)^2$ で割り、$r_i=\log u_i/\log L$ と置くと、制約は極限で $\max r_i=1$ となる。三重点では三枚のsquareが現れる。このradial計算は候補の説明である。Actual KE metricの一様漸近と全閉cornerの局所GH極限には、上記のcomplete模型比較と距離定理を別に用いる。

本稿で構成した写像は $f_t=p_T\circ\pi_t:X_t\to B_d(T)\to\mathcal C_d$。五次では $p_T$ は同相、六次以上では基底内の木も収縮する。**空間としてのGH収束**と**指定したLagrangian fibrationによる実現**を区別する。

主稿 `base_topology.tex` の `topo:ke-map-compatibility` に、$\operatorname{dis}(\Phi_t)\le a_t$ と $\sup_xd_\square(\Phi_t(x),p_T\pi_t(x))\le b_t$ から $\operatorname{dis}(p_T\pi_t)\le a_t+2b_t$ を得る比較命題と証明を置いた。Ambient fiber diametersは同じ量以下、GH距離はその半分以下である。一般的新規性は主張しない。この一般的な比較命題と、同じ $f_t$ に対して直接証明した全域distortionの消失は別の結果である。本稿の主定理は外部の条件付き近似写像 $\Phi_t$ を入力にしない。

**公表前の点検：** `ke:global-metric-realization` から依存する局所・全域証明を逆にたどり、文献の適用条件、固定stageの定数と最後のparameter閾値、同じ写像への上下界の適用を包括的に確認する。新証明と接続は内部点検済みだが、全主稿の再監査とは区別する。Action-affine structureだけからcanonicalなRiemannian基底計量は決まらない。


## 局所fibrationの証明と解析入力
曲面側の着手対象は複素次元2でのKE極限とLagrangian fibrationの適合性である。主稿の `papers/sections/paper/ke_fiber_compatibility.tex` に次の証明を置いた。

- `ke:short-torus-averaging`：自由な正則 $T^2$ 作用、torus不変Hermitian計量 $h$、$c h\le g_\omega\le C h$、torus上のperiod零を仮定する。作用の周期1生成場の長さの和を $e$ とすると、平均化のchain homotopyから長さ $O(e)$ のprimitiveを作り、一つのMoser flowで領域全体にLagrangian fibrationを構成する。変位は $Ce/(2c)$ 以下、ambient fiber diameterは $\sqrt C e(C/c+1/2)$ 以下。高階微分比較は使わない。
- `ke:triple-hexagon`：$\zeta_i\zeta_j\zeta_k=t$ の三つのsquareを一つのhexagonとして全phase torusで実現し、raw-depth mapとの誤差を $O((1+\log m_t)/R_t)$ に抑える。
- `ke:triple-moving-fibration`：全phaseを含む moving domain $\min\ell_a>m_t/2$ 上の一様tensor比較を追加仮定すれば、actual負KE形式に対する局所fibrationが得られ、そのambient fiber diameterは元の尺度でも $O(m_t^{-1})$。$m_t=R_t\to\infty$ とできる。負KE equationにより局所canonical trivialization上で形式がexactとなるのでperiod条件は満たされる。

これらは原稿に条件と証明を保持する局所結果である。Averaging–Moserの基本方法はRuan, arXiv:math/0309177v2, §3に先行し、一般的新規性は未確認。H-minimal/special Lagrangian性、大域接着、singular fibersの計量評価は結論しない。

**解析入力の区別：** 関連KE主稿の `coarse:prop:density-counterexample` により、負KE計量であってもbounded volume densityから一様tensor比較は導けない。五次coarse metric packageには独立な $(\mathrm{TC})_5$ が必要であり、その無条件な検証は未完成である。これは対象compact familyの反例ではない。全深部三重点のfull-orbit moving tensor比較は全固定d≥5で検証した。Source等を含むexterior全体への一様tensor二側比較の拡張は未解決である。本稿の全域距離比較は別のscalar/portal評価により得た。

### Averaging–Moserの先行研究
W.-D. Ruan, *H-minimal Lagrangian fibrations in Kähler manifolds and minimal Lagrangian vanishing tori in Kähler–Einstein manifolds*, [arXiv:math/0309177v2](https://arxiv.org/abs/math/0309177v2)。§3 Proposition 3.1（PDF p.7）はpotentialのtorus平均、Lemma 3.3（pp.7–8）はHamiltonian-gradient flowを扱う。Theorem 3.1（p.9）はhomothetic toric potentialと一様 $C^\infty$ quasi-isometryの下で、局所領域 $D_{\Delta_{c\tau}}$ に全正則fibersがH-minimal Lagrangianであるfibrationを構成する。Theorem 4.2（p.11）はsimple toroidal canonical degenerationの最大退化点へ消えるminimal torusの族であり、全域fibrationの定理ではない。関連する [math/0311098v2](https://arxiv.org/abs/math/0311098v2), Theorems 6.2・8.2（pp.15, 19–20）は、complex torus内の非compact hypersurfacesのcomplete KE Cheeger–Gromov極限とminimal vanishing toriを扱う。

本研究の補題はperiod-zero、$C^0$ tensor比較、短い生成場だけを用いてprimitiveとambient diameterを直接評価する。Ruanの高階幾何とH-minimal性の結論は求めない。既存方法の定量化として位置付け、新規性は未確認。ZhangのTheorem 2.6の個別generalized special Lagrangian torusの存在とも、全域のsingular fibrationとも区別する。

### 固定領域と移動領域の区別・相対接着への入口
主稿 `ke:fixed-simplex-scale` の計算により、固定simplex compactaは径の尺度のtriple vertexしか見ない。関連KE研究ノートの「固定領域の収束から径の尺度へ移る際の障害」に、固定compacta上ではcusp metricと完全一致し、全体で一様に粗比較できるにもかかわらず、正規化した区間長が $1$ から $3/2$ に変わる一次元例を証明付きで収録した。KE反例ではなく、sharp moving estimatesの必要性を示す例である。

主稿 `ke:relative-fiber-preserving` は、torus-saturatedな**開**collar N上で元のorbitsが既にactual ω-Lagrangianであれば、β=Hω、H=K_1+A_1K_2というchain primitiveがvertical vectorsを消すことを用いる。ω_sも同じvertical distributionをLagrangianに保つため、Moser場はverticalであり、各fiberと基底値が保存される。ωの作用不変性は不要。Centered chain primitiveでも同じ証明が成立するが、同じdβを持つ任意のprimitiveへの置換では消滅条件が保存されるとは限らない。

`ke:relative-neck-matching` は、別のactual Lagrangian fibrationがこの開overlap上で同じorbit partitionを持つなら、基底collarを同定して写像を接着できるという局所系である。各点の固定や単一境界上の一致だけを用いた接着は主張しない。点ごとの固定が必要なら、既存の `ke:relative-averaging` のcentered kernel 1/2−sと作用不変collarを使える。許容射影と遅い対角選択では共通葉・normal moment・bufferを `ke:neck-corner-saturated-union` で実証した。独立な第二periodの一致は含まない。

定数係数monomial変更ζ'=c(t)ζ^A、A∈GL(2,Z)はphase orbit partitionを保つ。一方、非定数holomorphic unitを含む変更ζ'=ζ^A u(ζ,t)は一般に保存しない。二つのtorus actionsが同じoverlapに存在するだけでは相対補題の仮定にならない。Sourceのcritical valuesについても `ke:source-marking` のcore交差仮定の下でp_T(b_t)→e_i+e_jが必要であり、固定された任意の内部markingは使えない。


## 相対接着の補助計算：primitiveの選択と障害

以下はregular torus領域での補助計算であり、仮定と証明をこのノートに保持する。主稿の `ke:relative-fiber-preserving` の証明を重複させず、primitiveの変更、整数基底の変更、collarの点固定に関する情報を整理する。選んだneckとcornerの共通葉・normal moment・bufferは上記部分fibrationで実証した。任意に独立先指定した第二periodの一致には追加確認が必要であり、補助計算の新規性も未確認である。

### Centered primitiveの整数基底変更

自由な同じT²作用に対し、全Haar平均をA、周期1の円作用をρ_{j,s}とする。Centered homotopy
\[
\widetilde K_j\xi=\int_0^1(1/2-s)\rho_{j,s}^*(\iota_{V_j}\xi)\,ds,
\qquad \widetilde H=\widetilde K_1+A_1\widetilde K_2
\]
はdH̃+H̃d=A−IとAH̃=0を満たす。後者は全平均がpullback・contractionと可換で、weightの積分が零であることから従う。整数基底や順序を変えた二つのβ_r=H̃_rωはdβ_r=Aω−ω、Aβ_r=0を満たす。従ってγ=β_1−β_0はclosed、Aγ=0であり、いずれかのtorus homotopy Hを用いると
\[
\gamma=-d(H\gamma)=df,\qquad f=-H\gamma.
\]
これはbaseの単連結性やH¹(U)=0を要しない。

ω_s=(1−s)Aω+sω、ι_{Y_s^r}ω_s=β_rとし、共通のbuffer内で両flow φ_s^rとその相対写像が定義される内側領域を取る。χ_s=(φ_s^0)^{-1}φ_s^1はAω-symplecticであり、Eulerian生成場Z_sは
\[
\iota_{Z_s}(A\omega)=(\phi_s^0)^*\gamma=d(f\circ\phi_s^0)
\]
を満たす。従ってHamiltonian isotopyで比較できる。ただし二つのflowそのものが一致するという主張ではない。両β_rが飽和collar N上で零なら、Hはorbit内で作用するためf|N=0、両flowとχ_sはNを点ごとに固定する。不変背景hに対して|Hγ|≤Ce|γ|なので、β_r=O(eδ)ならHamiltonianの大きさはO(e²δ)となる。定数は用いる有限個の整数基底に依存してよい。

### 負KE potentialからのprimitiveと定数係数monomial変更

Toric chart上の不変logarithmic volume formをΩ=dlogζ_1∧dlogζ_2とし、Ric(ω)=−ωとする。正のvolume規約で
\[
F=\log\frac{\omega^2}{\Omega\wedge\overline\Omega},\qquad
dd^cF=\omega,\qquad
\beta_{\rm can}=d^c(AF-F)
\]
と置く。ここでd^c=(i/2)(\bar∂−∂)。作用が正則なのでAとd^cは可換し、dβ_can=Aω−ω、Aβ_can=0である。同じphysical overlap上でζ′=c(t)ζ^B、B∈GL(2,Z)と変えると、orbitとHaar平均は同じで、Ω′=det(B)Ω、|det B|=1である。従ってF、β_can、ω_sが一致し、共通buffer上のMoser flowもODEの一意性により厳密に一致する。Centered chain primitiveとの比較は上のHamiltonian計算で与えられる。

定量的には、torus不変Kähler背景h、torus不変模型k、v=log(ω²/k²)に対して、固定階のC^{q+2}(h) normがO(δ)、生成場の|V|+|∇V|がO(e)とする。模型のpotential部分は不変なのでAF−F=Av−vである。Isometric pullbackは∇_hと可換し、tensor∇^jvのLie derivativeにはVと∇Vだけが現れるから
\[
\|Av-v\|_{C^{q+1}(h)}\le C_q e\delta,
\qquad \|\beta_{\rm can}\|_{C^q(h)}\le C_qe\delta.
\]
必要な逆形式の一様C^q boundsとflow bufferの下でMoser場も同率となる。全深部tripleではe=O(m^{-1})、δ=O(m^{-1})であり、固定階ごとにO(m^{-2})を得る。Centered chain primitiveについてもH̃k=0からβ=H̃(ω−k)となり、同じ短い生成場と微分評価の下でO(m^{-2})である。主稿のclosed-corner GHは既存のchain flowのO(m^{-1})評価だけで証明している。

**Fiber保存との区別。** β_canのvertical成分の消滅は、元のorbitが既にLagrangianであることから自動的には導かれない。一般のpotential averagingの例として、compact product annulusの近傍で
\[
F=|z_1|^2+|z_2|^2+\epsilon\operatorname{Re}(z_1)|z_1|^2
\]
とする。十分小さいεではdd^cFは二つの複素一次元因子のKähler formの和なので、元のphase toriはLagrangianである。しかしz_1=re^{iθ_1}として
\[
d^c(AF-F)(\partial_{\theta_1})
=-\frac32\epsilon r^3\cos\theta_1
\]
は一般に零でない。この例がKEであるとは主張しない。`ke:relative-fiber-preserving` を使う際はchain primitiveを選ぶ必要がある。ωがcollar上で作用不変なら、Fも不変なのでβ_canも零になる。

### Volume frameのgaugeとorbit partitionの変更

同じ作用を固定してΩ′=uΩ（holomorphic unit）とだけ変えれば
\[
\beta'_{\rm can}-\beta_{\rm can}
=d^c(\log|u|^2-A\log|u|^2)
\]
はclosedである。Logarithmic base Dが可縮なReinhardt domainならu=ζ^n e^fと書ける。n∈Z²はwinding vector、fは一価正則関数であり、Afは正則かつtorus不変なので定数である。従って上の差はd Im fでexactとなり、Hamiltonian比較へ入る。

一方、座標そのものを
\[
\zeta'_1=\zeta_1e^{\epsilon\zeta_2},\quad
\zeta'_2=\zeta_2,\quad
\zeta'_0=\zeta_0e^{-\epsilon\zeta_2}
\]
と変えると、積方程式ζ_0ζ_1ζ_2=tとΩ′=Ωは保たれるが、|ζ′_1|は元のphase torus上で一定でない。従ってorbit partitionとHaar averaging operator自体が異なる。小さいunit変化を小さいisotopyとして比較できても、指定neck collarに相対的なsymplectic/Hamiltonian matchingや作用周期の一致は別に必要である。

### 点固定のrelative classと両端のperiod matching

同じsymplectic pathに対する任意のprimitiveの差γ_sはclosedだが、一般にはexactでない。相対Moser isotopyの生成場のdualは(φ_s^0)^*γ_sであり、isotopyが各時刻でHamiltonianになる条件はこの1-formのexactnessである。時間積分したfluxやendpointのHamiltonian同値とは区別する。上のcentered choicesではγ_s=−d(Hγ_s)がこの障害を消す。

ω_sが滑らかなcollar N上でsに依らず、σ_s=−∂_sω_sがNで零とする。Nを点ごとに固定するprimitive、すなわちdβ_s=σ_s、β_s|N=0の存在条件はrelative class [σ_s]∈H²(U,N;R)が零となることである。通常のrelative de Rham complexとextension/cutoffを使えるcollarを取り、必要なら少し縮める。時間についての滑らかな選択とflowの存在bufferは別に課す。

絶対primitive β_sが既にあるとき、同条件は[β_s|N]がrestriction H¹(U;R)→H¹(N;R)の像に入ることと同値である。十分性は、同じrestriction classを持つglobal closed 1-formを引き、残るexact restrictionをcutoff extensionで消すことで示せる。必要性は二つのprimitiveの差がglobal closedであることから従う。

特にU=B×T²、Bは可縮なcorridor、N=N_-⊔N_+は両端のfull torus collarsとする。RestrictionはR²→R²⊕R²の対角写像なので、両端の二つのtorus period vectorsの一致が条件になる。その差は対応するS¹を運んだcylinder上のσ_sの積分である。これは指定したmarkingとaction originを保つ相対同定の条件であり、自由なbase relabellingを許すfibrationの存在障害と同一視しない。

**適用先。** 全域構成・基底値整合・全moment接続・全fiber合併・no-shortcut/portalの各証明は主稿に保持する。上の相対classの条件は点固定germを指定する別問題に有効であり、actual linkからの構成と混同しない。Potential連続度の十分条件も未検証入力として保持するが、P0の径評価には不要である。


## 複素次元2：先行研究・singular fibersの確定事項
本研究の曲面X_d⊂P³, d≥5の一般SNC gluingと、全平面模型の明示的なsingular fiber型を区別する。主要な定理は papers/sections/paper/geometry_main_statements_v17.tex の main:global、nodeの線型monodromyは invariants_examples.tex、より詳しい先行比較は geometry_introduction_v25.tex。

**一次資料の比較：**
- I. Smith, *Torus fibrations on symplectic four-manifolds*, Turkish J. Math. **25** (2001), 69–96, https://journals.tubitak.gov.tr/math/vol25/iss1/4/ 。Homologically essential Lagrangian toriとtame singularitiesという追加条件下での閉四次元多様体の制限定理。本研究の分岐・core特異ファイバーへの直接適用は、tamenessとregular torusのhomology classの検証なしにしない。
- G. Mikhalkin, *Decomposition into pairs-of-pants for complex algebraic hypersurfaces*, Topology **43** (2004), 1035–1065, DOI 10.1016/j.top.2003.11.006。[math/0205011v3](https://arxiv.org/abs/math/0205011v3) のDefinition 7（PDF pp.13–14）、Theorems 1・1′（pp.17–18）を確認。射影・toric hypersurface全域のstratified torus fibrationを構成し、ambientから誘導する形式に対して各maximal cellで少なくとも一つのLagrangian torusを保証する。全regular fibersのLagrangian性を定理から読み取らず、他のfibersが非Lagrangianだとも断定しない。
- D. Matessi, *Lagrangian pairs of pants*, IMRN **2021**, 11306–11356, DOI 10.1093/imrn/rnz126、および *Lagrangian submanifolds from tropical hypersurfaces*, Int. J. Math. **32** (2021), 2150046。[1802.02993v1](https://arxiv.org/abs/1802.02993v1) のTheorem 1.1と直後（PDF pp.1–2）、標準cotangent形式（p.6）、[1804.01469v1](https://arxiv.org/abs/1804.01469v1) のTheorem 1.1と§1.2（pp.1–3）を確認。前者はtropical curves in $\mathbb R^2$、後者はtropical hypersurfaces in $\mathbb R^3$ のPL liftを滑らかなembedded Lagrangian部分多様体へ近似する。標準形式を持つ $(\mathbb C^*)^n$ 内の半次元部分多様体の構成であり、symplectic pants全体のtorus fibrationではない。後者のtoric compactificationの完全な構成は同Introductionで今後の課題とされる。
- W.-D. Ruan, *Lagrangian torus fibration of quintic hypersurfaces. I. Fermat quintic case*, AMS/IP Studies in Advanced Mathematics **23** (2001), 297–332。[math/9904012v2](https://arxiv.org/abs/math/9904012v2) の§2（PDF pp.6–7）、Theorem 3.1（p.15）、§6（pp.36–37）を確認。Fubini–Study形式でcompact Fermat型Calabi–Yau三次元多様体の全regular fibersをLagrangian $T^3$ とする。Discriminantは厚みを持つ二次元集合で、写像はpiecewise smooth・大域Lipschitzと説明される。本稿の $\mathbb P^3$ 内の一般型五次曲面とは次元もcanonical classも異なる。負KEに対する局所構成は上記「Averaging–Moserの先行研究」を参照。
- N. C. Leung and M. Symington, *Almost toric symplectic four-manifolds*, J. Symplectic Geom. **8** (2010), 143–187, DOI 10.4310/JSG.2010.v8.n2.a2、**Theorem 2.1**, Table 1。閉almost toric 4-foldの全空間を分類し、一般型曲面X_dは含まれない。通常のalmost toricはsmooth surface base、ellipticと孤立focus singularitiesが許される。本研究はbranched baseとlog-Weinstein coreを許し、仮定が異なる。
- J. D. Evans and M. Mauri, *Constructing local models for Lagrangian torus fibrations*, Ann. Henri Lebesgue **4** (2021), 537–570, [DOI 10.5802/ahl.80](https://doi.org/10.5802/ahl.80)、[1905.09229v3](https://arxiv.org/abs/1905.09229v3)。掲載版Lemma 2.16（pp.543–544）、Remark 2.18（p.544）、Lemma 2.22・Remark 2.23（p.545）、Lemma 3.1と§3.1（pp.546–547）を確認。四直線補集合のsymplectic completion上に、cone over $K_4$ を基底とする全regular fibersがLagrangianなfibrationを構成し、branch fiberを明示的に $S^1\times(S^1\vee S^1)$、cone fiberをskeletonとする。形式の構成・変形とcontact formの正の関数倍を許すため、所定finite collarと全葉を同時に保存する相対延長とは分ける。曲面core模型の直接的先行結果である。
- M. Golla and B. Martelli, *Pair of pants decomposition of 4-manifolds*, Algebr. Geom. Topol. **17** (2017), 1407–1444, DOI 10.2140/agt.2017.17.1407。四次元pants decompositionの微分位相。
- Y. Zhang, *Pair-of-Pants Decompositions of 4-Manifolds Diffeomorphic to General Type Hypersurfaces*, J. Math. Study **58** (2025), 211–252, [DOI 10.4208/jms.v58n2.25.06](https://doi.org/10.4208/jms.v58n2.25.06)。[2102.10037v1](https://arxiv.org/abs/2102.10037v1) のFigure 1.1（PDF p.2、実画像確認）とTheorem 1.1(ii),(iv)（p.4）を確認。$d\ge5$ の $X_d$ と微分同相な四次元多様体を $d(d-4)^2$ 個のpantsとK3由来の領域などへ分解し、pants側境界にgraph fibrationを与える。その特異fiberは $\Theta\times S^1$（$\Theta$ は二つの三価頂点を三辺で結ぶtheta graph）であり、本稿の $(S^1\vee S^1)\times S^1$ とは同相でない。Hyperplane classに対する $\int_T\omega=0$ を示すが、点ごとの $\omega|_T=0$ や閉曲面全域のLagrangian fibrationは結論しない。掲載版PDFは公開URLでHTTP 403となり、今回の図・定理本文の照合は2021 preprintに限定する。
- J. Fernández de Bobadilla and T. Pełka, *Fibrations by Lagrangian Tori for Maximal Calabi–Yau Degenerations and Beyond*, CPAM (2026), DOI 10.1002/cpa.70060。[2312.13248v4](https://arxiv.org/html/2312.13248v4) のTheorem 6.14(b)は一般Kähler SNC退化のmaximal/submaximal strataに対応する部分領域のivy-like Lagrangian fibration、(c)はproperな場合には全nearby fiberの補助Kähler計量によるGH収束を与える。全域core fillingの不足とactual KE計量への比較の不足は異なる論点である。詳細は本ノート「二つの尺度と先行定理」を参照。

Leung–Wan (JDG **83** (2009))の一般型での漸近special性はMikhalkinが選んだLagrangian fibersに関するもので、全regular fibersではない。これらの結果を踏まえ、「一般型で初めてtorus fibrationを構成する」といわず、所定のKähler formで**全regular fibersがLagrangianな閉曲面上のglobal construction**を本稿で証明する主張として、証明監査と先行研究の網羅性を引き続き検証する。

**全平面分割における主定理のfiber一覧：**
- 2D top stratum: 正則Lagrangian T²、Euler数0。
- 1D branch-edge interior: S¹×(S¹∨S¹)、Euler数0。三枚のsheetが接し、各辺全体に連続的に出現するため、辺の本数は「個々のsingular fibersの個数」ではない。
- Face interiorのisolated nodal value: 一重pinched T²、Euler数1、local focus monodromy [[1,1],[0,1]]。全部でd C(d,2)個。
- 0D core vertex: P²からd−1本の一般位置直線を除いた補空間のlogarithmic Weinstein skeletonのsymplectic image。Homotopy typeは(T^{d−2})の2-skeleton、b₁=d−2、b₂=C(d−2,2)、Euler数C(d−3,2)。全部でd個。

基底の開branch辺はC(d,2)(d−4)本、三角形C(d,3)枚、bigon C(d,2)(d−5)枚。d=5なら(core, branch-edge, node)=(5,10,50)、coreのχ=1、全Euler数55。d=6なら(6,30,90)、coreのχ=3、全Euler数108。面ごとの配分として、五次の十triangleに各5 node、六次の二十triangleに各3 nodeと十五bigonに各2 nodeという値は、各明示的recipeで選んだ配置に限る。抽象的なmarked tree、一般存在定理、P0のactual構成からその配分が強制されるとはしない。一般構成に共通するのはnode総数とfiber型であり、一般dのEulerチェックは
\[
d\binom{d-3}{2}+d\binom d2=d(d^2-4d+6)=c_2(X_d).
\]
現行SNC構成の大域作用適合atlasを仮定する六次では、`q9:sextic-rigidity` と `q9:node-budget` が各bigonの二nodesをweight recipeに依存せず強制する。この追加条件下の剛性は保持し、一般存在・P0の任意の配分へは拡張しない。

**Singular fiberは一般にsmooth embedded Lagrangianではなく、各smooth stratumがisotropicなstratified fiber**として定義している。Core skeletonも一般のdで一つの固定したpants型ではない。この基本的なlocal topology、個数、Euler数の証明と先行研究との範囲比較は原稿に保持する。幾何学的gluing証明全体の独立監査はなお必要である。


## 五次整数接着：保持する独立課題
全pair productsが狭義正の四ray整数データの正weightsはmatchingと同値。G5_14両単位枝の{5,0,0}を排除し、{4,1,0}に限定したと原稿は記録する。必要支持はG5_14、G5_16、G5_17の3型26標識。存在・幾何的非同型類の個数とは異なる。三高Dの一般同時非負性と一般分母剛性は残る。
これらはP0の全域GH実現に必要な場合以外は後順位とする。証明・計算資産は維持し、独立した分類の未完了をKE研究の停止理由にしない。


## KE退化との分岐基底の位相的比較
曲面基底 \(B_d(T)\) の三価木 \(T_{ij}\) を収縮する既存の \(q:B_d(T)\to\operatorname{Sk}_2\Delta^{d-1}\) と、KE候補 \(\mathcal C_d\) の正規化同相の逆を合成すると、**labelを保ち点逆像が可縮な** \(p_T:B_d(T)\to\mathcal C_d\) を得る。一般次数の厳密な証明は `papers/sections/paper/base_topology.tex` の `topo:KE-cubical-comparison`。\(d=5\) では同相、\(d\ge6\) では両者は同相ではない（辺の局所分岐次数が異なる）。この位相的比較単独ではKEのGH極限や作用アフィン計量との一致を結論しない。Actual ambient距離でのGH実現には `ke:global-metric-realization` の解析と接着を用いる。

整数鎖複体の主張を検査するため、\(d=5,\dots,8\) の \(B_d(T)\) と \(\operatorname{Sk}_2\Delta^{d-1}\) の \(\partial_1,\partial_2\) の階数を独立に計算して、\(b_1=0\)、\(b_2=\binom{d-1}{3}\) と一致した。再現コードは `verification/verify_ke_base_topology.py`。これは有限体 \(\mathbb F_{1000003}\) 上の有限検算であり、整数係数の一般定理の証明は本文のexplicit chain contractionが担当する。


## Cubical targetの非伸長retraction・六次以上の厳密直径

**既知の組合せ的構成との関係。** $\mathcal C_d$ のcellは $\varnothing\ne A\subseteq B$、$|B|\le3$ の区間に対応するので、単体二骨格のcubical barycentric subdivisionである。この同定はfaceの式から直接確認できる。E. K. Babson, L. J. Billera, C. S. Chan, *Neighborly cubical spheres and a cubical lower bound conjecture*, Israel J. Math. 102 (1997), 297–315, DOI [10.1007/BF02773804](https://doi.org/10.1007/BF02773804) の1996年preprint §2.3、Proposition 2.2、Corollary 2.4に対応する。[確認した一次scan](https://www.math.ucdavis.edu/~deloera/MISC/LA-BIBLIO/trunk/Billera/BilleraEhrenborgcdindex.pdf) は論文が連結・逆順になっており、PDF第24頁が本文p.6、第30頁が対象の表題・著者・日付。書誌は[著者の刊行論文一覧](https://pi.math.cornell.edu/~billera/research.html)とも照合した。既知の細分の構成と、今回のunit-square長さ距離の非伸長retraction・厳密直径とは区別する。後者に一致する既存定理は短い一次文献探索では確認できなかったが、新規性を確定したものではない。

正本は `base_topology.tex` の `topo:coordinate-retraction`、`topo:six-label-gallery`、`topo:diameter-six-labels`。非空Iとanchor a∈Iを選び、外側座標を $r_a=\min(1,\sqrt{w_a^2+\sum_{\ell\notin I}w_\ell^2})$ へまとめる。Euclidean非伸長性に加え、各source squareが一つのtarget cellへ写ることから、内在距離に対する非伸長retractionを得る。したがって $d_I=d_\square|_{\mathcal C_I}$。両端のsupportの和へ縮約できるので、最短路には六label以下で十分。Gallery上限は $3\binom{\min(d,6)}3$ である。

六次以上の直径 $2\sqrt5$ の上界は、共通labelを持つ場合の二square展開と、disjointな三元supportの場合の3L+1Dの四shuffleで証明する。後者の下界は、二組の三labelの個数に応じた9頂点型の値を120個の三角形へaffineに延長するcalibration。四galleryの共有辺・全展開座標、全120三角形の勾配二乗を有理数演算で再実行した。`verification/verify_cubical_six_label_geometry.py` がその再現コードであり、retractionの解析的証明やKE推定の検証ではない。新規性の網羅的確認は未了。

`ke:closed-corner-global-target` は既存closed-cornerのtarget距離を全 $\mathcal C_d$ のものへ置換する。Source側の全曲面ambient下界は `ke:global-ambient-lower` の別の証明で与える。`topo:protected-thin-bypass` は、一般の二square長さ空間で局所の飽和したprotected距離と全域(S),(F)が誤差零でも、細い外側帯によるshortcutが起こる例である。Actual KE族の反例ではない。有限の全被覆でも加法誤差だけでは不足することは、本ノート冒頭の `ke:full-cover-oscillating-bypass` が別に示す。

## 人工的基底計量の鋭い収束速度と幾何学的比較の核心
$p_T:B_d(T)\to\mathcal C_d$ に補助piecewise Euclidean metric $h$ を固定し、$|v|_\varepsilon^2=|dp_T(v)|_\square^2+\varepsilon^2|v|_h^2$ の内在距離を考える。graph correspondenceのdistortion $\mathcal D_\varepsilon$ は、$d=5$ で $\Theta(\varepsilon^2)$、$d\ge6$ で $\Theta(\varepsilon)$ と鋭く決まる（主原稿に読み込む base_topology.tex の topo:metric-collapse-sharp）。$d\ge6$ の下界は同一fiber内の正の $h$-距離に由来するが、**GH距離の下界ではない**。

実際の基底長さ計量 $d_t$ に対する十分条件（topo:finite-portal-criterion）は、(N) global no-shortcut誤差 $\alpha_t$、(S) square segment liftの乗法誤差 $\sigma_t$・加法誤差 $\lambda_t$、(F) 同じfiberの接続費用 $\kappa_t$。十分なsquare数 $N_d=3\binom{\min(d,6)}3$、直径 $D_d$ について
\[
\operatorname{dis}(p_T)\le\max\{\alpha_t,\ \sigma_tD_d+N_d\lambda_t+(N_d+1)\kappa_t\}.
\]
二枚のunit squareを一頂点で貼り、二枚を一枚に折る反例では(N),(S)が誤差零でも(F)が成立せず、$d_{\rm GH}\ge\sqrt2/2$（topo:portal-counterexample）。したがって局所模型だけでは大域収束は言えない。独立のLagrangian action metricの長さ完備化と枝・coreへの延長は本稿の全域実現定理の結論外である。P0では全空間のactual ambient距離に直接no-shortcut・portal評価を証明した。新規性は未確認。


## 六次Petersen分岐基底の対称性
$d=6$ で全ての頂点リンクをPetersenグラフとするラベル付き木系はちょうど六つであり、$S_6$ はこの集合に推移的に作用する。固定した一系の安定化群は位数 $6!/6=120$、指数6。従ってその一系の選択は座標置換の全 $S_6$ 対称性を保たない。KE候補 $\mathcal C_6$ は自然に $S_6$ 対称なので、Petersen分岐基底とのラベル付き比較を対称に行うには六つの木系全体を管理する必要がある。証明は base_topology.tex の topo:petersen-symmetry、全15 perfect matchingsと六one-factorizationsの有限列挙・安定化群位数は別に確認した。これは任意の別構成やラベル忘却後のシンプレクティックな対称性の不存在ではない。

## 検証状態


**曲面主稿改訂43の検証（2026-11-22）。** 同じ射影の体積測度極限を原稿へ統合し、固定compactの値比較・全質量と頂点逆像を別担当が点検した。Source-armからscalar障壁への依存について、complete-volume比較の固定t上有界性、三境界とorientationを保つbuffer、cut順序を対象限定で再読した。組版・変更頁表示はこの数学checkpointでは未実施で、最後の成功記録は改訂42の311頁・指定22頁である。既存整数証明書は保持し、今回は再実行していない。現行状態の正本は [検証状態](validation.json)。
