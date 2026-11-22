# 現行研究方針：一般型曲面のLagrangian torus fibration
更新：2026-11-23 / v3.40（複素次元2専用、曲面主稿改訂52・五次整数接着第25稿）

## 価値最大化を目標とする公表計画

数学的重要性、新規性、理解の深化、応用可能性、正確性、読者による検証、実現可能性を総合して研究全体の価値を最大化する。現在の主軸は、actual負KE形式上の同じLagrangian射影による全域GH実現と、固定SNC補空間の距離・実球体積漸近である。従来の五篇の順序、論文数、特定の証明経路、未解決atlasの完成をそれ自体の目標にしない。有効な一般存在定理、条件付き結果、反例・障害と再現資産は保持する。

三研究の公表計画の正本を本節に置き、各repoの研究方針には担当する実行項目を記す。証明は担当repo、正確な依存関係は `research/ke-dependencies.md`、短い到達点と優先順位はresearch-hubを正本とする。

| 公表単位と優先度 | 中心となる価値 | 公表準備の達成基準 |
| --- | --- | --- |
| 第一優先：本repoの曲面主稿 | 固定次数 \(d\ge5\) のactual負KE形式、同じ射影、全曲面ambient距離・全fiber合併・確率体積極限を扱うP0、および五次・六次の同じ射影による全域作用atlas/GH・確率体積極限 | 精密な主定理を前へ置き、source・core・scalar下界・portal上界・遅い対角選択の証明鎖と外部入力を追える。一次資料との比較を具体化する。 |
| 第一優先：Part IVの局所解析 | 全深部tripleのtensor安定性、complete simplex、閉corner、固定end | 必要な境界入力と定数依存を抽出し、局所定理と一般位置全平面退化への適用を分ける。曲面へ供給する最小の入力表を作り、証明は一度だけ掲載する。 |
| 並行する第一優先：Part I | 一般SNC補空間の有界加法誤差を持つ錐写像と実球体積の精密漸近 | Rochon–Zhangからの入力、LeuzingerおよびChambert-Loir–Tschinkelとの対象・observableの差を示す。実球裾係数の内在性・基点依存と仮定の役割を証明する。 |
| 独立して維持：Part II・III・V、一般weights・追加保持集合・整数接着 | 標識付きTorelli、条件付きconifold、大域距離枠組、作用適合構成 | 無条件部分と未検証入力を分けて公表価値を判断する。これらの完成を上記の成果の公表条件にしない。 |

### 実行順序と判定基準

1. **中心定理と最小解析核を確定する。** 曲面主稿のP0を前へ移し、解析入力・六段階の証明経路・cutの順序を一箇所にまとめる。Part IVではfull-triple証明を再点検し、固定faceの密度下界と各固定parameterの滑らかなradial閉包から導ける局所定理を実際の仮定の範囲内で抽出する。固定compact・誤差・cutを先に選び、全ての小さい複素parameterの閾値を取り、最後に遅い対角選択を行う。
2. **新規性と独立な価値を明確にする。** Mikhalkin、Fernández de Bobadilla–Pełka、Zhang、Ruan、Evans–Mauriとの比較を、全域性・実際のKE形式・同じ射影・距離の範囲で整理する。Part Iでは実球裾係数の内在性、基点比較、compact基点集合上の一様性を検討し、非可積分なcusp誤差の明示例で仮定の役割を示す。未発見を新規性の証明としない。
3. **五次・六次の同時実現を中心結果へ組み込む。** 五次のcompatibleな有限データと六次の標準等重みについて、finite-t periods、source wall、全moment面積、全open overlaps、同じ射影のGHと確率体積極限を一本の証明鎖にする。六次の内部二端cuts、balanced separator、中央freezeとanchor後選択の役割を保持する。新証明と接続の対象限定独立点検、組版・表示と引用整合を確認済みである。任意先指定の大きい保持集合に残る障害は削除しない。
4. **引用入力と公表上の比較範囲を確定する。** Source正規形・有限W1予算・Schwarz半径の指定点検を保持し、Part IVのcomplete simplexでは存在/実Hessian完備のみをZhang Theorem 2.1経由のCheng–Yau入力とする。一意性・tubeと格子商・scaling・規格化は直接証明した。CY1982原典Theorem 4.4の本文取得は未了として明記する。局所境界入力から指定canonical simplexへの全深度比一様O(1/m)小誤差と、固定depth coordinates/reference k_Lでの率の最適性を比較する。全phaseや定量評価自体に新規性を置かず、Zhangの固定normalized compact、Ruanのtorus平均に関する定量的結果を区別する。FBPの明示GH近似と全fiber補助Kähler GHも引用し、actual KE・全域射影・同じ写像のambient距離・作用atlasの同時達成に公表上の比較を集中する。Actual compact族やfacet shift補正後の最適率、一般weights、CP/PBE/TC、任意中間尺度・有効t速度・高次元化は別課題とする。
5. **公表可能性を実際に確認する。** 変更証明と依存関係を別担当で点検し、LuaLaTeXの組版・相互参照と変更箇所の表示を確認する。日本語原稿で内容を固めてから英語化を判断する。原稿内の証明、今回の内部点検、計算、形式検証、外部査読、投稿・公表は別の状態として報告する。

項目1の主定理・証明入口とPart IVの局所定理抽出、項目2のPart Iの内在的裾係数・基点一様性・非可積分cusp例を本文へ反映した。項目3では有限endpoint条件をactual primitiveから求め、全momentの正targetと薄い初期source葉を構成し、同じ射影の全域atlas/GHまで証明を統合した。新証明のsource wall・Dini・成分別Moser・全葉接着を逆向きに独立点検し、三面に共通する平行移動付き整数アフィン接続式と、解析選択後のthin代表を許す根拠を本文へ統合した。FBP Remark 5.9、EM Remarks 2.11–2.12、Ruanの実際の仮定との比較も明確にした。さらに同じ射影上の確率体積極限を固定成分の体積保存から導き、公表範囲を計量と測度の双方へ明確化した。固定end解析の最小入力とnormal frameのwinding公式をPart IV v1.12へ統合した。Part I v1.9では積の実距離Laplace変換の複素対数germと正規化距離分布の復元を証明し、追加証明・一次比較・変更頁を点検した。総説v1.13はこれら三研究の現行結果と適用範囲を同期する。次は未確認の中心証明と一次文献比較を依存表から特定し、主張の新規性と公表単位を確定する。既に点検した鎖の一律な反復は行わない。六次の標準等重み同時実現は中心成果に含め、一般weights・先指定の大きい保持集合への拡張を独立課題とする。全主稿・全外部入力の包括的再監査、外部査読、新規性の網羅的確認は未完。誤りや既知結果との重複が見つかれば依存先を修正し、定理の範囲や公表単位を再評価する。

通常コミットとmainへの反映を承諾を求めず行い、長時間の作業では15〜30分を目安に切りのよい成果を保存する。他の作業者の変更を保持し、force pushとGitHub Actionsの追加・起動は行わない。各repoの原稿・ノート・方針・READMEの保存後、実際の確認範囲に基づいてhubを更新する。本節は研究固有の計画であり、共通の一般原則と保存許可は本書後半および `AGENTS.md` に置く。


**現行の到達点（改訂52・公表準備）。** 各固定次数d≥5のactual負KE–Lagrangian射影による全域GH実現と、同じ射影へ運ぶ確率KE体積の極限に証明がある。五次のcompatibleな有限データに加え、六次では等重みw_i,j=2/5とsource配分(1,1,1,1;2)を用い、初期source葉を選んだ同じπ_tに全域作用atlas・GH実現・確率体積極限を持たせる（`ke:sextic-simultaneous-realization`）。六つの標準Petersen系のいずれも選べる。f_tの押出しは成分頂点、π_tの押出しはcore頂点の等重み原子測度へ弱収束する。全cubical距離と有限な測度の台、確率体積と未正規化のrescaled体積を区別する。任意先指定の大きいsource近傍、任意の異なるweights・focus不変量、atlasのparameter極限や極限計量のHessian性は結論しない。指定証明の独立内部点検と、全主稿再監査・外部査読・形式証明・包括的新規性確認を区別する。


**六次の有限条件から同時実現へ（改訂44）。** `ke:petersen-actual-neck-periods` はactual finite-t primitiveとwindingから、標準zero-external targetsのsource配分(1,1,1,1;2)、external切片ρ_i,k=ρ_j,k、内部切片ρ_i,j=ρ_j,iを導く。Row sum 4πからρ_i,j=4π/5、w_i,j=2/5が一意に定まる。`ke:petersen-two-end-cuts` の内部累積位置条件を、`ke:petersen-balanced-separator` と `ke:petersen-thin-source-block` の中間面積指定・Diniによる薄いblock・中央parameter-freezeで満たす。Full source annuliをその後で固定し、`ke:petersen-full-moment` が全moment targetsと両anchorの全open germsを実現する。`ke:sextic-simultaneous-realization` は同じdomain・primitive・moment・cutsと固定marked Tを使い、三面共通の平行移動付き整数アフィン接続からatlasを、相対値比較から同じπ_tのGHと確率体積極限を得る。各証明と接続は作成担当以外の読み手も対象を区切って点検した。任意に先固定した大きい内部source blockの位置障害は残り、その場合に同じ存在を主張しない。

研究資料v3.40・依存表v3.29、主稿改訂52。Part IV v1.15の `simplex:prop:boundary-floor-sharpness` を短く引用し、固定depth coordinates・比較模型k_Lに関する局所仮定クラスでのO(1/m)の最適性を明記した。Actual compact射影的族の誤差下界やfacet shift補正後の最適性は主張しない。Zhangの固定normalized compactと全phase、Ruanの固定縮小polytope上の定量的なtorus平均比較を一次本文で確認し、指定canonical simplexへの全深度比一様な小誤差を局所解析の比較点とした。FBPの明示GH近似・補助Kähler計量とactual射影の比較、cubical/flat simplicial計量の非homothety、既存のsource・輸送・core・atlasの指定点検を保持する。現行組版と実表示の実施範囲は検証JSONに記す。

同じ確率KE体積から独立に選んだ有限標本の距離行列は，異なるラベル間距離が2のd点等重み空間の標本行列へ分布収束する（`ke:random-ke-distance-matrix`）。二点距離は(1/d)δ_0+(1−1/d)δ_2で，平均は2(d−1)/d。これは既存GH・測度収束からの系で，追加解析入力を要しない。全cubical空間のGH極限と標本距離が観測する測度台を区別する。

既存のGH distortion \(\epsilon_t\) と同じ射影の確率体積輸送 \(W_1((f_t)_*\nu_t,\nu_0)\) だけから、独立なk点の正規化距離行列の分布について \(W_1^{(\infty)}(\mathcal L_{t,k},\mathcal L_{0,k})\le\epsilon_t+kW_1((f_t)_*\nu_t,\nu_0)\) を証明した（`ke:random-ke-distance-transport`）。固定compactの予算では右辺を \(\epsilon_t+k[\eta_K+D_d(\delta_K+e_K)]\) と評価でき、二点距離が{0,2}の\(\rho\)-近傍外に出る確率も同じ輸送費用を\(\rho\)で割って抑えられる。k重結合の費用は\(\ell^\infty\)行列normで測り、固定されたkと族を対象とする。Moving tensorの追加入力も有効t速度も与えない。

`ke:source-uniform-deep-volume-tail` により、固定source tubeの深部体積V_t(S)は全ての小さいtに一様にC/S以下。さらに固定0<θ<1/4のS0≤S≤θLではcθ/S≤V_t(S)≤Cθ/Sと最良次数であり、S≥L/2+A_bではc_b L^{-2}exp(−(2S−L))≤V_t(S)≤C_b L^{-2}exp(−(2S−L))と中央指数領域まで二側比較する。既存capped体積上下界のみを積分し、新しいmoving tensor仮定は不要。全neck・全曲面の体積裾、距離径や有効GH速度を導くものではない。

**Capped前因子はactual KE体積についても鋭い。** Part IV v1.16 の `coarse:prop:capped-prefactor-sharp` が同じbarrierの指数2の最大性を証明し、曲面主稿 `ke:source-capped-actual-prefactor-sharp` はさらに `ke:source-central-density` を用いて、実際のω_t²≥cΩ_t,d^(β)がt一様に全X_tで成立する必要十分条件はβ≤2と証明する。β>2では固定単純sourceの中央点p_tでω_t²/Ω^(β)≈L_t^(2−β)→0。これは既定のα_iとcanonical densityを固定したときの結論であり、別の障壁構成やGH速度の普遍的限界ではない。

## 現在の成果と優先順位

**P0の全域GH実現には、現在の原稿に証明がある。** 任意の固定次数 \(d\ge5\) と下記の一般性条件を満たす全平面退化について、actual負KE形式の大域Lagrangian torus fibrationと、同じ写像 \(f_t=p_T\pi_t\) の全曲面ambient距離に関する一様distortionの消失を構成した。主定理は `ke:global-realization`、統合証明は `ke:global-metric-realization`。必要な証明箇所と局所・全域の接続を複数担当で内部点検しているが、形式証明、全主稿・全外部入力の包括的再監査、外部査読、新規性の網羅的確認は行っていない。

現在の優先課題は、公表に向けた依存証明と一次文献の包括的再点検、新規性の確認、主稿の構成整理である。一般存在・actual KE計量実現・作用適合atlasの量化を照合し、五次のcompatibleな有限データと六次の標準等重みについて、初期source葉を選ぶ同じ射影のatlas/GH/測度を証明した。Sourceの全moment退出は三境界Schwarzと直接経路により $O(1)$ に改善した。Componentの接続費用は $C(1+\log(N_j+1))$。残余基底の定数を先に固定し、それを吸収するcut $N_j$ を選ぶことで、全fiber合併とportalの予算も $H_{j,t}=C(1+\log(N_j+1))$ とできる。同じmomentのcorner参照点を用いることで下界の乗法係数も固定族の定数に整理した。上下両側のdistortionは `ke:eq:global-realization-explicit-cut-budget` のcutを明示した式で評価できる。これは残余定数やscalar補助cutの増大率、最適収束速度を評価した結果ではない。SourceのGaussian評価は独立な補助結果として保持する。従来の大域fibration構成・特異fiber・作用適合atlasの有効な成果は保持する。五次整数接着の全分類は未完の独立課題であり、公表準備と必要な検証を優先しながら維持する。三次元の存在問題は別repoを正本とする。自律的な研究・保存の手順は [AGENTS.md](AGENTS.md) と [Cloud Codexの再開手順](research/cloud-codex.md) に置く。

### 三研究を一体で進める編集方針

研究上の依存監査・方針・文献比較は三repoを通して行い、証明の正本と公表単位は次の分担で保つ。分担の理由は、固定した非コンパクト空間の無限遠幾何、退化パラメータに一様な局所解析、actual形式上の大域fibrationという異なる対象と量化を明確にするためである。既存の有効な証明と独立論文は保持する。

| 正本 | 担当する内容 | 本研究との接続 |
| --- | --- | --- |
| [multiscale-kaehler-einstein](https://github.com/uedakazushi/multiscale-kaehler-einstein) | 固定SNC・配置補空間の漸近錐、残余period/Torelli、条件付きconifold局在（Part I–III） | 固定成分 $U_i=\mathbb P^2\setminus(d-1\text{ 本の直線})$ の幾何と極限空間の局所模型。シリーズ総説は同repo。 |
| [kaehler-einstein-degeneration](https://github.com/uedakazushi/kaehler-einstein-degeneration) | 退化族のcapped density・全深部triple・固定base/end解析（Part IV）、CP/PBE付きの大域距離枠組（Part V） | 定理・仮定・規格化を固定してK1–K4へ入力する。 |
| 本repo | Actual KE–Lagrangian構成、共通moment接着、scalar下界・portal上界、同じ射影の全域GH実現 | 利用側から入力を監査し、詳しい接続を `research/ke-dependencies.md` に一元化する。 |

固定補空間のblow-downを退化族のmoving領域へ無条件に移さず、固定compact・誤差・cutを先に選び最後に $t$ の閾値を取る。三研究の「証明あり」「条件付き」「未完成」「今回点検した範囲」を揃える。Surfaceの直接経路はCP/PBE/TCやH_loc/H_anc自体を検証するものではない。Part IIの複素・双曲periodと本稿の第二作用、P0と同時atlasも区別する。依存する結果の訂正は正本から利用側へ反映し、保存後にhubの要約を更新する。全論文の統合は目的とせず、公表単位の再検討は論理的なまとまりと重複量に基づいて行う。

### 固定成分と選択した中間尺度

Part I v1.9の `thm:contract` と `cor:based-ball-approximation` は、固定成分 $U_i$ 上でproperな1-Lipschitz全射 $\mathcal S_i:U_i\to C_{2,d-1}$ を選び、一度 $\mathcal S_i,K_i$ を固定すれば、距離 $R^{-1}d_{\mathrm{KE},i}$ の中心 $o$・半径 $A$ の閉球と、錐の中心 $R^{-1}\mathcal S_i(o)$・同半径の閉球のGH距離が $3K_i/(2R)$ 以下になることを示す。ここで球にはambient距離を制限し、定数は $o,A$ に一様である。指定compactを零へ送る選択では $K_i$ はそのcompactに依存してよい。固定成分のco-Gram・全射性、LDP、Busemann・tailの対象限定監査を三研究で同期したが、この $K_i$ はcut $N_j$ と退化parameter $t$ を動かす一様定数を供給しない。

`prop:cone-limits` と `cor:moving-limit-classification` は、incidence copiesを保つlink coneと正の面座標のstarを用い、全moving-basepoint limitsを分類し、任意のscaling sequenceに対する実現も与える。`lem:star-ball-isometry` の条件は $m_\alpha>2A$ であり、閉star全体のambient距離を積とみなさない。`lem:cone-link-metric` と `prop:link` は、非連結linkの成分間距離を無限大として、truncated angular metricから全長さ距離を回復する。得られるのは等長型であり、named cell labels、normal-depthの重み、genuine geodesic-ray boundaryの同定ではない。Moving側は共同点検結果を同期し、link側は曲面側担当も独立に点検した。これらは固定空間の定理であり、退化族の一様性、任意の中間尺度、同じ $\pi_t$ でのatlasとP0の同時実現を与えない。

Part I v1.9の測度論では、ordinary volume-IRFAから任意の $\min_iT_i\to\infty$ に対する全residual space上の固定stripの全変動収束を得る。Metric-IRFAと収束するcentered offsets・residual基点を加えると、ambient閉球の押出し測度の全変動収束とpointed measured GH収束も成立し、smooth volume-IRFAは不要である。Chern–Weilと面質量は、滑らかな基準曲率に対する有界primitive・有限体積・cutoffによる直接Stokesで規格化を確認した。全faceの整合した体積漸近からactual conditional measuresの一様subcritical momentsを導き、Abel–Mellin recursionに独立なweighted error dominatorを追加仮定しない。同じmoment上界でvertex tightnessを評価するため、metric-IRFAと全faceのordinary volume-IRFAでexact tail/joint/Laplaceも成立し、exponential volume条件は追加仮定しない。Component別cutoffを含むmixed transformsの係数はface incidenceを検出するが、面質量の数値だけからの回収ではない。具体的なラベル・適用範囲と担当ごとの点検範囲は依存表へ置く。これらは固定成分の測度データの結果であり、P0の新しい解析入力や退化族の一様評価を与えない。

主定理の仮定依存表では、LDPの $\mu/\mu(X)$ と、face translation・面質量に用いる非正規化 $\mu=dV_g$ を区別する。後者はfull collarの $\mu_F=\chi_F\mu$ を $\Pi_T=(t_I-T,\pi_F)$ で押し出す。球のpmGHにはcentered offsetsと残余基点の収束を加え、tailには非空境界と固定基点を要求する。Ordinary volume-IRFAからのAbel係数と、追加の残余 $L^1$ joint polyhomogeneityを要するmeromorphic continuationは別の結論である。主稿 `ex:Abel-not-meromorphic` の $1/t$ の誤差例を有効な障害として保持する。

Part II v2.1では完全標識とKähler orientationを保つ復元と、factor/cusp labelsを保ち向きだけを忘れるgeneric Torelliを区別する。後者は全curve factorsを使い、全体複素共役までの結論である。これらの標識は裸のmetric limitから自動的に得られない。測度側の先行比較ではChambert-Loir–TschinkelのIgusa積分・residue measuresを参照し、面測度とMellin主要係数を結ぶ一般原理を独自成果として数えない。一次比較の範囲と正本は依存表に置く。

固定成分 $U_i=\mathbb P^2\setminus(d-1\text{ 本の直線})$ のPart Iの漸近錐 $C_{2,d-1}$ は、cubical target $\mathcal C_d$ の成分頂点 $e_i$ のmetric tangent coneとlabel付きで一致する。`topo:component-cone-germ` に半径 $r<1/2$ の閉球の厳密な等長を証明した。さらに既存P0の同じ全射の歪み $\epsilon_t$ を用い、$1\ll a_t\ll R_t$ かつ $R_t\epsilon_t=o(a_t)$ なら、成分頂点上の任意の基点から $(X_t,a_t^{-1}d_{g_t})$ がこの錐へpointed GH収束する（`ke:intermediate-component-cone`）。$a_t=R_t\sqrt{\epsilon_t+R_t^{-1}}$ と選べる。同系はさらに、$\eta_t=\sup_{y\in A_t}d_\square(f_t(y),e_i)\to0$ と $R_t(\epsilon_t+\eta_t)=o(a_t)$ の下で、任意の $y_t\in A_t$ へ基点を移しても一様に成立する。同じP0の一成分のcoreと変更collarには $\eta_t\le C(1+\log(N_{j(t)}+1))/R_t$ を使える。局所錐・中間尺度・基点移動の証明を独立内部点検したが、既存P0全体の再認証、任意の中間尺度や極限交換の証明ではない。

### 全移動基点の中間尺度と固定段階の量化

主稿 `topo:cubical-local-models` と `topo:cubical-moving-blowups` は、有限cubical targetの全局所模型と全移動基点の拡大極限を分類する。成分頂点では $C_{2,d-1}$、supportが二元の辺（$e_i+e_j$ も含む）では $\mathbb R\times\mathcal Y_{d-2}$、三座標が全て1の頂点では全角 $3\pi/2$ の錐、それ以外では $\mathbb R^2$ となる。$\mathcal Y_m$ は原点で貼った $m$ 本の半直線。局所閉球は全targetのambient距離に関して等長であり、移動基点の極限ではこれらの空間の任意の有限基点を許す。

`ke:distortion-to-pointed-balls` は、全射の全域歪みが $\delta$ 以下なら、任意の中心・同じ半径の閉球の基点付きGH距離を $3\delta/2$ 以下で比較する。これを同じP0の写像に適用し、`ke:intermediate-moving-classification` は $a_t\to\infty$、$a_t/R_t\to0$、$R_t\epsilon_t/a_t\to0$ の下でactual曲面の全移動基点の部分列極限を上の四型に分類する。任意の許容尺度と退化列で各型を実現できる。全域歪みの速度は未評価なので、この誤差条件を除いた任意の中間尺度、tensor収束、極限交換へは拡張しない。有限幾何とGH移送の証明は複数担当で独立に内部点検した。

`ke:source-inclusive-fixed-shell` は、sourceを含む固定残余compactで同一の正則体積frameを保ち、固定endのmoment $\pm4\pi/(-\log r^2)$ とshell横断費用を証明する。先にcompactと $r$、最後に全ての小さい複素 $t$ を選ぶ。Songの固定smooth locus収束とRochon–Zhangのcusp展開の一次資料を確認した。異なる正規形のprimitiveの一致やresidual period消滅は追加しない。`ke:global-clipped-cogram-lower` は固定parameterの有限評価へ定式化を改め、誤差消失は統合定理の最後の対角選択でのみ用いる。上下界・Part IV入力の指定証明鎖に循環やprotected距離のambient距離への無条件な置換は認めなかった。全主稿・全外部結果の包括的再監査ではない。

### P0で得た定理の範囲

任意の**固定した**次数 \(d\ge5\) に対し、主稿 `deg:family` の明示族、および同じ一般性条件を満たす全平面退化
\[
 X_t=\{\prod_{i=1}^{d}L_i+tF_d=0\}\subset\mathbb P^3
\]
を対象とする。平面は一般位置、\(F_d\) は全三重点で非零、各二重線で相異なる単純零点を持ち、十分小さい非零parameterで \(X_t\) は滑らかとする。\(\operatorname{Ric}(\omega_t)=-\omega_t\)、\([\omega_t]=2\pi(d-4)H\)、\(R_t=\log(-\log|t|^2)\) と固定する。次数・族一様の定数やspecial Lagrangian性を追加要求しない。

許容される一つの標識付き木系 \(T\) を選び、実際の \(\omega_t\) に関して全regular fibersがLagrangian \(T^2\) である連結fiberの大域全射 \(\pi_t:X_t\to B_d(T)\) を構成する。Sourceのpinched torus、branchの \(S^1\times(S^1\vee S^1)\)、core skeletonを含む本研究の相対構成に接続する。特異fiberは各smooth stratumがisotropicという意味で扱う。Markingの位相的な型を保ちながらnodeの位置や必要な構成パラメータは \(t\) とともに選び直せる。あらゆる既存の任意選択に対する収束は要求しない。

`topo:KE-cubical-comparison` の \(p_T:B_d(T)\to\mathcal C_d\) に対し、\(f_t=p_T\circ\pi_t\) が
\[
 \varepsilon_t:=\sup_{x,y\in X_t}
 \left|R_t^{-1}d_{g_t}(x,y)-d_\square(f_t(x),f_t(y))\right|
 \longrightarrow0
\]
を満たすことを証明した。ここで \(d_{g_t}\) は**曲面全体の全経路を許すambient距離**、\(d_\square\) は \(\mathcal C_d\) 全体のunit-square長さ距離である。全射性からGH距離は \(\varepsilon_t/2\) 以下となる。全ての \(f_t\)-fiber、従って正則・特異を含む全 \(\pi_t\)-fiberの正規化ambient直径が一様にゼロとなる。\(d\ge6\) で \(p_T\) が潰す内部木についても、一つの木上の複数の \(\pi_t\)-fibersの**合併全体**を評価した（`ke:collapsed-tree-full-fiber-collapse`）。

証明は十分遅い固定段階の対角選択を用い、各固定次数・固定族について一つの許容された標識付き木系を選ぶ。最適収束速度、任意に先指定した木系・作用・critical valuesへの一様な適合、次数一様の評価、全次数のmatroidal atlas、special Lagrangian性は結論に含めない。五次だけの結果ではない。新たな誤りが見つかった場合は、依存する主張・方針・hubを含めて訂正する。

### Normal momentを保つ相対変更と五次の同時実現

`ke:moment-relative-replacement` と `ke:relative-replacement-gh` は、同じ保持cornerの全葉、sourceのcompact nodal neighborhoods、同じcanonical normal moment・anchor cuts、同じcomponent core領域を保つ相対変更に対し、基底値の差を
\[
\sup_x d_\square(f_{j,t}(x),\widehat f_{j,t}(x))
\le C\eta_{j,t},\qquad \eta_{j,t}=C(1+\log(N_j+1))/R_t
\]
で抑える。変更後のmarked Reeb productとcore coneの実際の商データ、全overlapのwhole-fiber一致は入力である。閉商を先に構成し、同じcorner inset・neck profile・小さいcore panelsでparameter化する。Reduced方向の変更をC1まで小さくする必要はなく、任意の指定変更を実現する定理ではない。これらの条件下ではGHの距離比較を引き継げる。五次では `ng8:quintic-full-moment` が初期source葉を選ぶことで所定targetの全moment実現と全open overlapsを与え、`ke:quintic-simultaneous-realization` がこの相対変更の条件を検証して同じ射影のatlas/GHを構成する。六次では `ke:petersen-full-moment` と `ke:sextic-simultaneous-realization` が等重み・初期source葉選択の下で同じ条件を満たす。先指定された追加保持集合への適用はstrict cutsを改めて確認する。

`ng8:fixed-fiber-relative-dh` は、各固定tのfree compact bandで、作用不変primitiveとaffineな境界作用からStokesによりtotal reduced areaのaffine性を得る。Reference constantsのt依存を許し、actual KE形式のt=0へのsmooth extensionを仮定しない。一方、重み(1,−1)の標準模型を \(I_1+I_2\le c\)、\(\mu=I_1-I_2\) で切ると、周期2π規約で \(\operatorname{Area}(P_\mu)=\pi(c-|\mu|)\) となる（`ng8:source-dh-wall`）。Source横断の全intervalへfree-bandのaffine性を流用できないことを示す局所模型であり、actual P0全体の面積公式ではない。相対Moserには端germsとmarked identificationsに加え、保持集合の補集合ごとの正の有限配分が必要である。補集合が分かれる場合、総量と個別marginだけでは足りない。


`ng8:componentwise-critical-area` は可動成分ごとの質量保存を正の有限配分行列と同値にし、`ng8:strict-area-cuts` がstrict Hall cutで判定する。`ng8:p0-small-area-flexibility` は、固定stage・固定tの小さいmoment intervalで、sourceのfull compact pinched torusを含む飽和annuliを保持した微小面積変更を実現する。`ke:actual-anchor-fan-criterion` と `ke:anchor-stokes-budget` は同じactual coreのanchor periodsからchartを構成する十分条件を与える。詳しい有限条件・規格化・障害と証明の所在は研究ノート「相対critical-areaの有限条件とactual source」「Actual coreの有限anchor period条件」を参照する。

`ke:raw-moment-error-insufficient` では、固定stageで \(\mu_t=-L_t^{-\alpha}\)、\(\nu_t=-L_t^{-\beta}\)、\(0<\alpha<\beta<1\) と取ると、\(|\mu_t-\nu_t|\to0\) でもlongitude差は \(\beta-\alpha\) へ向かう。近似matchingを用いる場合はnormal momentの絶対誤差でなく、profileを通した基底値差を制御する。

### 一般存在・KE実現・作用atlasの量化

一般存在 `main:global` は指定した Kähler 形式と任意の許容された embedded marked pants treesを扱う。次数分割では `part:global` の所定の型のmarked Morse葉層の相対isotopy classを指定する。SNC相対定理 `snc:main` は正のweighted Kähler表示、各成分の交点数二以上を仮定し、同じclassの代表とnormal holonomyを構成中に選ぶ。P0は固定した族から一つの木系を選び、全ての十分小さい複素parameterで同じ基底型を使う。各射影の連続性と、parameter方向に連続又は滑らかな族の存在は区別する。

五次では `ke:quintic-simultaneous-realization` が、有限整合式を満たすweights・四角形系・source配分から、初期source葉を選び同じ $\pi_t$ の全域作用atlasとGHを構成する。等重みの対称六系により対象族の存在が従う。六次では `ke:petersen-full-moment` と `ke:sextic-simultaneous-realization` により、等重み・初期source葉選択の下で同じ射影のatlas/GH/測度を証明した。任意に先指定したsource近傍の保持や任意のfocus不変量への適合は含まない。

七次以上では `ke:global-core-nonmatroidal` により、同じP0の基底の各core近傍にもmatroidal chartが存在しない。Core linkの第一Betti数C(d−2,2)≥10と三価matroidal linkの上限8からの直接系である。これは固定した基底のcore germの位相障害であり、cubical合成写像やcore surgeryを許す全fibrationsの分類へは拡張しない。

先行研究の比較では、Fernández de Bobadilla–PełkaのTheorem6.14(b)のfibrationは部分領域上だが、同(c)はproperなら全nearbyfiberの構成Kähler計量のGH収束を与える。本稿はactual負KE計量と同じ全域射影のdistortionを扱う。Zhangの境界fibrationの特異fiberは確認したpreprintのtheta graph×S¹であり、本稿のfigure-eight×S¹とは同相でない。図・定理・版を研究ノートと参考文献に記す。これらは対象限定の一次比較であり、網羅的新規性確認ではない。

### 証明の状態と外部KE仮定との区別

現行主稿は、`ke:slow-cut-closed-corner-gh` を $m\ge m_*,\ R\ge R_*,\ \log(m+1)+4\log R\le R/8$ の有限条件で述べ、固定cut後のparameter選択を明記した。全target端点のportal選択、$\mu=0,\pm\delta$ の境界・中央torus、全fiber合併、有限galleryの費用を独立点検した。`topo:finite-endpoint-comparison` は厳密な線分liftやfiber内経路を仮定せず上界を与える。Raw/actual momentの区別とtailの共通bufferも明記した。共通anchorによる保持neckの正確な区間、同一moment参照点と固定族係数による上下両側のcut budgetを保持する。FBPの構成計量によるGH定理とFHJの孤立楕円特異点のcusp閉鎖を一次資料で比較し、一般のMoser移送だけではactual距離比較を得ないことをIntroductionに記した。内部点検・組版・表示確認は末尾に区別する。

Actual全域構成、sourceの全点評価、同じ基底値に対する全域上下界を主稿に保持する。Componentの対数接続費用、anchor interval外のneck尾部の深度、残余基底→cut→parameterの非循環な選択も保持する。Coreのcompact-relative Morse–Smale化と閉isotropic filtrationも明示し、primitive・nontrapping・collar補間・全fiber trim・閉quotientを重点監査した。追加証明は別担当と独立に内部点検済み。数学的点検、形式証明、組版、有限計算、GitHub保存は区別する。

本研究は、正則normal frameのscalar Schwarz障壁とglobal clipped-depth mapでno-shortcut下界を、同一moment接続と有限portal galleryで上界を直接証明する。**関連KE研究の \((\mathrm{CP})_d\)、\((\mathrm{PBE})_d\)、\((\mathrm{TC})_5\) を証明したという主張ではない。** これらを対象族で検証する課題は関連研究側に残り、本稿の全域実現定理では仮定として使わない。`topo:ke-map-compatibility` による既存GH近似との条件付き比較は、有効な補助結果として保持する。

### 全域quotientとEuler予算

`glue:closed-whole-fiber-quotient` は有限閉piecesの全fiber飽和から閉同値関係を直接作り、Hausdorff性を後段の基底同定に依存させない。`ke:global-base-parameterization` は有限閉貼合せとquotientの普遍性から同じfiber partitionの基底同相を構成する。`topo:cubical-composite-connected` により $f_t=p_T\pi_t$ の全fibersも連結である。ただし内部木上のfiber合併は三次元部分を含み得るため、$f_t$ 自体をLagrangian torus fibrationとは呼ばない。

`inv:euler-pushforward` は $\pi_*\mathbf1$ の非零部分を $d\binom d2$ 個の相異なるnodal valuesと $d$ 個のcore valuesへ局在させる。Finite strata上の局所productとcompact-support Euler特性の加法性により、全Euler数は $d\binom{d-3}{2}+d\binom d2=d(d^2-4d+6)$。`inv:cubical-fiber-euler` は同じcubical点へ写るnodesを重複度付きで数える。五次・六次の面ごとのnode配分は具体的recipesに限り、一般存在・P0の追加条件にはしない。これらは既知の閉写像・Euler加法性の本構成への適用であり、一般原理の新規性を主張しない。

### Sourceとnodal patchの適用範囲

`ke:source-focus-transversality` はmoment依存の残余関数に対する写像の非退化条件を与える。同じ葉の分割でも残余関数を三乗すると写像は退化するため、foliationの型と指定momentum mapの判定を分ける。`ke:focus-neighborhood-period` と `ke:focus-whole-neighborhood-transport` は、normal cycleと一つの残余period、通常のTaylor不変量とprimitiveの追加定数項を区別する。実際に構成したcompact pinched torusと飽和近傍全体を運び、任意の先指定模型とのmatchingは要求しない。

`glue:area-normalized-blowup` は例外面積 $e$ によるradial Kähler構成を与える。CGの相対比較を固定した飽和affine-convex patchに局所化し、その外を恒等とする。Patchを固定後に容量を小さくし、全compact nodal neighborhoodsを取り、normal conjugacyのcollarをそれらから離して、最後に退化parameterを選ぶ。既知原理の適用として一次資料と比較し、全域quotientと特異fiberのEuler予算へ接続する。

### 証明の構成と公表前に点検する箇所

K2の全交わりの飽和と共通葉、K3のlink→adapted primitive→相対葉族→補間後trim→全域被覆の指定証明鎖を独立に点検し、対象内に追加仮定や訂正を要するギャップは見つからなかった。条件と証明箇所は [研究ノート](research/notes.md) の「K2/K3の全fiber接着で用いる条件」にまとめる。今後はこの接着の再確認を繰り返すより、残る外部入力と一次比較、主定理のscopeの包括的点検を優先する。

K1–K3はactual全域fibrationを、K4は同じ写像の全曲面distortionと全fiber合併の収縮を与える。K5の統合定理は `ke:global-metric-realization` に置く。K0のcore構成とK5の全域組立ては、今回の指定範囲の独立点検を終えた。今後は同じ鎖の一律な反復を避け、Part IVの最小入力表からの使用域照合と、actual KE形式・全域の同じ射影・作用atlasの先行結果比較を残る公表課題として絞る。六次の有限period・全moment面積構成と同時実現も公表対象に含め、任意先指定germsへの拡張は独立課題とする。詳細な入力・参照commit・定理ラベルは [KE依存関係](research/ke-dependencies.md)、有効な障害と着想は [研究ノート](research/notes.md) が正本。

| 課題 | 最初に行うこと | この課題の達成条件・現在の状態 |
| --- | --- | --- |
| K0：入力の監査 | 固定coupling chartsの葉period障害に加え、正則bandの第二作用判定、canonical frameの残余period差、固定形式の非直線critical action反例を本文に整理した。一重focus近傍の残余period・全近傍移送・transversalityと、面積規格化したnodal surgeryの支持を明示した。有限閉quotient、合成写像の全fiber連結性、Euler関数の有限支持とcoarse fiber公式を明示した。Introduction・主定理の量化を照合し、五次・六次の同時atlas/GH/測度定理、任意指定germsの残る条件と七次以上のcore障害を明示した。次は残る依存証明と先行比較を逆向きに点検する。Core・atlas接続の既存監査は保持し、一般存在・P0・作用atlasを区別する。 | 共通anchor・同一momentによる基底値比較、有限cutのcorner比較、全target端点のportal、全fiber合併とgalleryを重点点検済み。Capped・full-triple/Savin・complete volume比較・Song/RZ、source特異reduction、K2全intersection、core primitive・nontrapping・relative collar・whole-fiber trim・閉isotropic filtrationの既存点検を保持する。全既存証明・全入力の包括的再監査と外部査読は未了。 |
| K1：actual neckの短円とbuffer | `ke:fixed-stage-source-neck`、`ke:neck-corner-diagonal-matching` の残余compact→normal cutoff→moment区間→parameter閾値の選択を用いる。 | 固定source-free基底の二側比較、source中心を含む短円、共通source/像、source-inclusive neckを証明。十分遅い残余exhaustionでは全flow・全円orbitを含むtripleとの共通開領域も確保した。任意に指定した縮小速度や曲面全体の被覆への一様性は主張しない。 |
| K2：複数endの同時整合 | `ke:neck-corner-saturated-union` の部分fibrationを全域構成への入力として使う。 | 三armの座標接続、normal period一致、相対Hamiltonian補正、共通moment区間とreduced graphにより、closed cornerと切詰めたneckの**全交わり**でfiber partition・向き付きnormal cycle・内部source/saddle markingを一致させた。Endの第二cycleは共通torus同定で移送して選ぶ。Source・saddleを含むactual部分fibrationを得た。独立に選んだ第二periodの一致は自動ではない。Core接着と全曲面被覆はK3で別途証明した。 |
| K3：component coreの相対接着 | `ke:actual-global-fibration` と四つの追加節を距離評価の入力とする。 | **固定段階の全域構成を証明。** 正residue periodの厳密同定、閉moment link、固定stageでの全特異層近傍の被覆とcompact complement、actual generator C1・adapted primitive/nontrapping、saddleを動かす相対葉族、全fiber単位のtrimを経て、全 $X_t$ をactual Lagrangian fibrationで覆った。各componentのcore・変更collar・neck尾部のambient接続費用は $C(1+\log(N_j+1))$、遅い対角選択で正規化径が消える。全曲面distortionは含まない。 |
| K4：全曲面の距離比較 | `ke:sharp-global-one-active` → `ke:global-depth-lipschitz` → `ke:global-depth-base-comparison` → `ke:global-ambient-lower` と、`ke:global-ambient-upper` の接続を点検する。 | 原稿に全域上下界の証明あり。中央sourceの全点径 $O(1)$、全moment退出 $O(1)$、保持cornerの基底値整合、全内部木の共通momentを用いる。`ke:collapsed-tree-full-fiber-collapse` は潰される全fiber合併を評価する。新証明と接続を複数担当で内部点検済み。 |
| K5：統合主定理と公表準備 | `ke:global-metric-realization` の全固定 $d\ge5$ の主張から、一次文献比較・新規性確認・本文の説明順を整える。 | 同じ $f_t=p_T\pi_t$ のdistortion消失を統合。全域上界は $C_d\{b_j^{-1}+(1+\log R_t+\log(N_j+1))/R_t\}$ に整理した。下界も固定族の係数へ整理した。Scalar補助cutと残余定数の増大率、定性的な閾値は未評価であり、最適rateは未解決。組版・表示確認の状態は末尾を参照。全主稿再監査・外部査読・形式証明は未実施。 |

K1–K2の正本は `ke_neck_corner_exhaustion.tex`。残余compactの定数を先に固定し、それを支配するnormal cutoffと共通moment区間を選び、最後にparameter閾値を取る。`ke:normal-flow-naturality` とmoment依存のreduced葉により共通開collarを構成する。さらにcorner cut $m_t=6b_j$、neckの葉でのtrim $B=7b_j$、広いnormal-first patchを用い、first-exit評価で全intersectionを共通plateauへ閉じ込める。逆normal flowの自然性からmomentを同定した後に深いnormal下界を使う（`ke:neck-corner-saturated-union`）。

この部分fibrationはsourceのpinched torusとsaddle fiberを含み、各closed cornerの内在・protected GH評価を持つ。`ke:actual-global-fibration` は保持されたcorner葉とsource近傍を保って全域へ接着する。中央全点径にはGaussian tail・Bishop–Gromov比較による証明と、短いgate退出・source-arm tensor比較による直接証明がある。全intervalのsource接続と基底値の整合を用い、全曲面のshortcut下界と木上のfiber合併・portal上界を別々に証明した。局所protected距離をそのまま全曲面距離に読み替えてはいない。

Source全体のEuler場 $W_+=x\partial_x+y\partial_y$ のactual normを固定chart上で一様に抑えた（`ke:source-euler-bound`）。中央sourceの $|z|\ge e^{-a_t}$、$a_t=o(R_t)$ の部分は、固定residual shellへ $O(a_t+1)$ で接続でき、正規化ambient径が消える（`ke:source-sublog-residual-connectors`）。Euler経路だけでは軸に届かないが、`ke:source-central-diameter` は別のGaussian体積比較で $z=0$ と極小residual点も含む全点径を $O(1)$ に抑える。`ke:fixed-base-source-central-band` により、固定基底の全中央帯と閉pinched torus全体も収縮する。

### SNCの相対period条件と適用範囲

固定normal connection・coupling chartsと同じresiduesの下で、basic補正とcoreを保つexact cutoffによる接着は、各成分の $g_a$ 個の独立正則葉periodが零であることと同値である（`snc:fixed-holonomy`）。障害 $H^1(D;\mathbb R)/q^*H^1(\Gamma;\mathbb R)$ の次元、必要なholonomy調整のrankはいずれも $\sum_a g_a$ であり、全 $2g_a$ component periodsを消す必要はない（`snc:reeb-leaf-kernel`、`snc:minimal-holonomy-controls`）。Basic補正は全critical collarsの外に支持できる一方、非零障害のholonomy補正は一般に元のfull saddle collarsを変える。Unitary phasesだけを固定する場合の整数period自由は、固定connection/gaugeの命題の外である。有限endpointはactual collar座標によるcone座標 $r$ の式で連続性を確認した。IKMの既知の成分上の原理と本稿のSNC統合を区別し、TMZのexact deformationおよびBSVの存在定理から任意指定connectionの実現を結論しない。証明・一次資料は主稿 `relative_compactification.tex` と研究ノートを参照。

### 第二作用の接着とmatroidal chartの障害

`neck:regular-period-matching` は、可縮な正則action chartと既定base同定の下で、第二作用の整数shear・符号・定数を含む一致をsymplectic matchingの必要十分条件とする。Exact matchingには固定primitiveの定数差も零であることが必要であり、normal actionだけでは決まらない（`neck:normal-action-counterexample`）。既知のaction-angle theoremのspecializationであって、その一般原理の新規性は主張しない。Canonical frame差による残余periodの整数windingは `ke:transition-residual-period` で区別する。

`atl:critical-action-obstruction` は作用適合matroidal chartの存在にcritical actionの有理直線性が必要であることを示す。`atl:fixed-form-bent-branch` は同じactual形式・normal action・両端とtoric/saddle点germs・marked treeを固定し、非直線critical actionを作る。従ってdenominatorを任意に許しても、その非零二階微分を持つ点には局所chartがない。五次・六次の既存atlas構成は、共通のembedded marked class、実面積、整数framing、切片を別々に合わせる。`ng8:straight-neck` の補間には同じ $\operatorname{Diff}_0(P\operatorname{rel}\text{ collars})$-orbitを用い、抽象的な木の同型だけで済ませない。一般symplectic存在とP0の計量実現の範囲は変更しない。

## 原稿・ノートの正本と公表単位
- `papers/surface-lagrangian-torus-fibration.tex`：このrepoの主たる公表用本文。相対SNC構成、次数分割、分岐底、作用適合atlasとactual KE–fibrationの全域GH実現定理（現行改訂47）。統合証明は `papers/sections/paper/ke_global_metric_realization.tex`。組版・表示確認の実施状態は末尾と `research/validation.json` に記す。
- `papers/quintic-integer-gluing.tex`：五次整数アフィン接着、高分母支持グラフの独立論文（第25稿、201頁の記録）。指定SNC cores・K5 graph・標準cones・marked puncturesを保つ候補が対象。必要支持3型26標識は**実現数ではない**。G5_14の中央matching、一般分母剛性、三高Dの同時非負性が未解決。
- `papers/meridian-surgery.tex`：四pantsのmeridian局所置換と閉corner circuitsの障害（18頁の記録）。
- `papers/research-notes.tex`：各種補題・証明素材のTeXノート（現行65頁、変更した第1・4頁を表示確認）。
- `research/notes.md`：現在有効な数学上の着想、条件、文献比較、障害と再開手順。検証コードは `verification/`。
- 複素次元3のnormal-trivial curves、focus block、相対円板群と大域存在目標は [threefold-lagrangian-torus-fibration](https://github.com/uedakazushi/threefold-lagrangian-torus-fibration) の `main` が正本。詳細をこのrepoへ二重掲載しない。関連するKE研究はresearch-hubから参照する。

## 複素次元2：先行研究とsingular fibers
曲面の主定理 main:global は、Mikhalkin (Topology 43, 2004, Theorem 1) の全次元stratified topological torus fibration（Lagrangian性は各maximal cellで選ばれたfiberだけ）、Zhang (J. Math. Study 58, 2025, Theorem 1.1) の一般型と微分同相な四次元多様体のpants分解と境界上のtheta graph×S¹模型（図はarXiv:2102.10037v1で確認）、Evans–Mauri (Ann. Henri Lebesgue 4, 2021, §3.1) の四次元pantsの局所Lagrangian fibrationとは区別する。Smith (Turkish J. Math. 25, 2001) の制限はhomologically essential toriとtame singularitiesを追加仮定する。Leung–Symington (JSG 8, 2010, **Theorem 2.1**) により、閉almost toric fibrationを持つ四次元多様体の分類に一般型X_dは含まれない。Fernández de Bobadilla–Pełka (CPAM, 2026) の一般SNC退化の部分領域構成から全域のfibrationは自動的には従わない。一次資料と仮定はresearch/notes.mdの「複素次元2」節と主稿Introductionに整理。

全平面構成のsingular fiberは、(1) 分岐辺上の S¹×(S¹∨S¹)（Euler数0）、(2) 面内孤立nodeでの一重pinched T²（Euler数1、focus monodromy）、(3) d個のcore頂点の一般位置d−1直線補空間に対応するlogarithmic Weinstein skeleton（Euler数C(d−3,2)）。正則fiberはLagrangian T²。全平面分割の開分岐辺はC(d,2)(d−4)本（**fiberの個数ではない**）、孤立nodeはd C(d,2)個。五次では(cores, branch edges, nodes)=(5,10,50)、六次では(6,30,90)。通常のalmost toricにない分岐辺とcoreを許すことが本研究の特徴。一般次数の全体構成と、五次・六次に限る大域作用適合atlasは別の主張。先行研究との比較は現行原稿とノートに保持する。全証明の独立検証と包括的新規性の確定は未了である。

## KEのGH極限との関係
標準負KE尺度では成分内部の四次元完備KE幾何が残る。径の尺度 $R_t=\log(-\log|t|^2)$ では、本稿の `ke:global-metric-realization` が同じ $f_t=p_T\pi_t$ を用いるactual GH収束を直接証明する。五次は $p_T$ が同相、六次以上は基底内の木全体も収縮する。関連KE研究にある $(\mathrm{CP})_d+(\mathrm{PBE})_d$ を使う経路とは証明を区別し、これらの仮定自体を検証したとはしない。既存近似 $\Phi_t$ と $p_T\pi_t$ の一様比較から収束を移す `topo:ke-map-compatibility` も補助命題として保持する。Zhang (MRL, 2015)の局所collapse定理のQ-factorial・相対ample仮定は、source germ $xy=tz$ を持つ我々の族へそのまま適用できない。文献と適用計算は `research/notes.md`、公表用の比較は主稿 `intro:ke-collapse` を参照。

## 成分coreの存在とtarget距離の確定部分

`ke_component_core_geometry.tex` はRochon–ZhangのSNC cusp potentialを用いて、固定compactで厳密一致する正則化と、極限KE形式自体の正residue・有限型Weinstein coreを与える。全域への接着は、既存のactual linkの葉をLiouville flowで内向きに延ばす構成で実現した。これにより、compactification出力の葉を先指定したcollarへ点固定で移す相対germを追加入力とせずに済む。既存の局所core fillingの結果は保持する。

`ke_component_link_cover.tex` は $q_a=M_a+2\pi w_a=\pm\widehat\mu_N$ を整数windingとexact transportから同定し、$N_j\iota_j\gg1$ のmoment cutsを丸めて閉linkを作る。固定shellのmoment上界と同じMoser flowの逆像bufferにより、K2の部分fibrationが中央の全特異層の固定近傍を覆い、その補集合がcomponent compactsに入ることも証明する。`ke_core_invariant_primitive.tex` は生成場のC1 smallness、centered scalar平均によるexact補正、全overlapとcutoff shellの被覆、nontrappingを証明する。`ke_relative_reduced_foliations.tex` はfull critical leavesを保つ相対葉族を構成する。

`ke_actual_core_gluing.tex` の `ke:actual-global-fibration` がこれらを統合し、全 $X_t$ 上のactual KE–Lagrangian fibrationを与える。全fiber単位のtrimと閉同値関係により連結fiber・Hausdorff基底を保ち、基底は同じ標識付き $B_d(T)$ となる。第二actionやcritical valuesの数値は先指定しない。各componentの変更領域とneck尾部の接続費用を $C(1+\log(N_j+1))$ と評価し、$R_t\ge jC(1+\log(N_j+1))$ によって正規化ambient径・選んだ接続費用を消す。異なるcomponent cores全部の合併径、任意のLiouville軌道長、core/fiberの内在径の評価とは区別する。

指定collarの相対fluxは `ke:component-flux-space` で有限次元化した。一般位置 $m=d-1$ 直線のcomponentについて障害空間の次元は $\binom{d-2}{2}$。これはCohen–Suciuの既知のboundary cohomologyの適用であり、新規性は主張しない。同じ形式に関して任意に小さい非延長germを実現する `ke:nonextendible-small-core-germ` と、contact rescalingが固定葉を保たない `ke:contact-rescaling-collar-scope` を、全域構成の不存在と混同しない。全K2交わりを含む恒等collar、補間後partitionに対する内側平行linkでのtrim、SNC構成にも共通の閉isotropic filtrationを本文に明示した。

`ke:core-depth-upper` と `ke:removed-corner-target-cap` は、実際に切り取った各component capの旧softmax像を $d_\square(P^{\rm old}(x),e_i)\le\sqrt2\log(CN_j)/R_t$ と評価する。閉link上の深度上界を固定strictly plurisubharmonic potentialの最大原理でcore全体へ延ばす。`ke:global-base-parameterization` は旧softmax値との $O((1+\log N_j)/R_t)$ 整合を全保持cornerで与える。保持領域自身の新しい内在距離の上界を要求せず、旧corner内の経路を全曲面の経路として用いて `ke:global-ambient-upper` へ接続する。全曲面の下界はscalar評価による別の証明である。

`base_topology.tex` の非伸長座標retractionにより、任意の座標部分複体 $\mathcal C_I$ の内在距離は全 $\mathcal C_d$ の距離の制限に一致する。特にclosed-cornerのGH評価は同じ誤差で全target距離を使えるが、source側の全曲面shortcutを制御したとはしない。最短路には六label以下で十分で、portal比較のgallery数は五次30、六次以上60にできる。

六次以上では $\operatorname{diam}\mathcal C_d=2\sqrt5$。最大対は互いに素な三元supportのall-ones頂点対に限る。四つの明示的galleryによる上界と、120三角形上のPL calibrationによる下界を本文で証明した。五次の既存値 $\sqrt{13}$ を使わず自己完結した証明である。直径近似対の明示的な線形安定性だけに五次の厳密値を使う。有限部分は `python3 verification/verify_cubical_six_label_geometry.py` で再検算できる。Actual KE曲面の $R_t^{-1}\operatorname{diam}(X_t,g_t)\to2\sqrt5$ は、六次以上では全域実現定理とこの有限幾何を合わせた帰結となる。

## 全深部三重点の actual 比較と閉cornerのGH極限
任意の固定次数 d≥5 の一般位置全平面退化で、三重点の全深度比・全角度に一様な actual KE 比較を証明した。正確な座標 ζ0ζ1ζ2=t、ell_i=−log|ζ_i|²、L=−log|t|²、R=log L とし、k_Lをlogarithmic simplex上のcomplete toric KE form、その実計量をg_L^sfとする。十分大きい固定m1と各qのCqについて、m≥m1、min ell_i≥mで
\[
\left|\log\frac{\omega_t^2}{k_L^2}\right|\le C/m,\qquad
\|g_t-g_L^{sf}\|_{C^q}\le C_q/m.
\]
定数は固定dと族に依存してよい。次数一様性は主張しない。証明の正本はKE主稿 `coarse:thm:full-triple-tensor`。

固定toric模型の存在・完備性にはZhang (2015), §2.1, Theorem 2.1 / Proposition 2.2を用いる（退化族のTheorem 2.4とQ-factorial仮定は使わない）。ψ_L=log L−Σlog ell_iに対してψ_L−(log3)/2≤φ_L≤ψ_L、V_L/3≤k_L²≤V_Lを内外にずらした障壁で証明する。Complete模型から三つの半平面へのYau Schwarz lemma、determinant比較、内部正則性により一様cusp geometryを得る。凸性からfacet shiftのlog-density差をO(1/min ell)とし、actual計量を内外のsimplex KE metricsでvolume比較する。Savinの小摂動定理でtensor・全高階誤差へ移る。Actual metric bufferや(TC)/(PBE)を前提としない。

Actual側の大域入力は `coarse:cor:degree-d-volume-lower`。Adjunction residueでcanonical densityを固定し、backgroundによるHermitian frame errorの吸収と各正のcap方向のminorから六型のdeterminant下界を証明する。Sourceでは元のplane coordinatesを保つexact xy=tzとrescalingにより二つのcap係数≥c_d/Lを使う。Compact minimum原理からactual volume下界を得る。この依存部分の証明と適用条件はKE側の原稿に明示されている。このcapped下界とfull-triple比較の必要な証明を重点点検し、固定境界面の下界だけで足りる箇所も明示した。監査範囲は依存表に記し、外部主稿全体の独立再監査は行っていない。

Lagrangian主稿 `ke:actual-closed-corner` の同じ averaging–Moser flow と同じactual Lagrangian torus bundleに対し、`ke:closed-corner-gh` と `ke:closed-corner-protected-gh` が全閉cornerのGH極限を与える。m=Rでsoftmax hexagonのMoser像をW_{t,J}、その射影をπ_{t,J}とすると、R^−2 g_tによる距離について
\[
\sup_{x,y\in W_{t,J}}
\left|d_t(x,y)-d_J(\pi_{t,J}(x),\pi_{t,J}(y))\right|
\le C\frac{\log R}{R}.
\]
これはW_{t,J}自身の内在距離と、外側保護領域V_t={min ell_i>R/2}内の全経路を許す距離の双方で成立する。標的のd_Jは三枚のunit squaresからなるC_J自身の内在距離として定義する。`topo:coordinate-retraction` により、これはfull C_dの距離の制限と等しい。この局所評価からの形式的な置換は行わず、全曲面ambient下界は `ke:global-ambient-lower` で別に証明した。全fiberのintrinsic/ambient diameterはO(1/R)、正規化後はO(1/R²)、raw cubical mapとの誤差はO(log R/R)。Squareの継目も同一のregular T²であり、既存大域fibrationのsource・branch・coreのsingular fibersとは同定しない。

距離の解析入力はKE主稿 `simplex:lem:rank-one-schwarz` の係数1評価と `simplex:prop:dominant-product` のsharp product比較。Clipped logarithmic projectionで模型simplex全体の経路の下界を示し、三枚以内のsquare galleryを内部へ移して上界を得る（`simplex:thm:closed-corner-model`）。ActualとのO(1/R)比較と同じMoser flowのC1評価で上記の結論へ移す。正本は `papers/sections/paper/ke_closed_corner_gh.tex`。Source・saddleを含むneckからcoreへの全域接着は `ke:actual-global-fibration` で証明した。全曲面を通るshortcutは `ke:global-depth-lipschitz` の全曲線評価と同じ基底値との比較で制御した。新規性の網羅的確認と外部査読・形式証明は未実施。

有限cut版 `ke:slow-cut-closed-corner-gh` では、固定族の定数 $m_*,R_*,C$ に対し、$m\ge m_*$、$R\ge R_*$、$\log(m+1)+4\log R\le R/8$ の下で誤差を $C[m^{-1}+(\log(m+1)+\log R)/R]$ と評価する。固定した $m$ の後に $t$ を小さくする順序を許す。固定 $m$ のままでは評価に $C/m$ が残り、GH収束にはさらに $m_t\to\infty$、$\log m_t=o(R_t)$ を使う。

## 開正方形上のactual KE–Lagrangian collapse
主稿の `papers/sections/paper/ke_open_cell_collapse.tex` に、任意の固定次数d≥5のactual KE計量に対する局所結果を置く。関連KE主稿 `simplex:cor:actual-dominant-product` は、三重点独立深度 a,b∈[L^η/2,2L^(1−η)]、0<η<1/2 上のproduct-cusp比較を全固定階でO(L^−η)と与える。Complete simplex模型の誤差O(((a+b)/L)²)とactual/model誤差O(1/min ell)を合わせた率であり、global capped volume下界、明示的な上下KE barriers、Savin (2007), Theorem 1.3に依存する。(TC)_dや(PBE)_dを追加仮定しない。

`ke:open-cell-moser-c1` は平均化のprimitiveとMoser場のC1 normをO(L^−η)とし、flowのpullback metricを制御する。`ke:open-cell-collapse` はKη=[η,1−η]²上のactual KE–Lagrangian T² fibrationを構成し、fiberのintrinsic/ambient diameter O(L^−η)、raw mapとの誤差O(1/R)を与える。Moser像領域に内在長さ距離を入れると、R^−2 g_tは平坦KηへGH収束し、projection distortionはO(L^−η+L^−η/R)=O(L^−η)。定数は固定ηに依存する。これらの証明と一次資料の適用条件を点検した。一般的新規性は未確認。

固定ηの開正方形と全閉cornerは、それぞれ上記の局所定理で扱う。Source・branch・coreを含む全域fibrationと同じ写像のambient距離比較は `ke:global-metric-realization` へ統合した。局所定理単独から全域distortionを推論してはいない。

## 共通normal circleに適合する二段階平均

主稿 `papers/sections/paper/ke_staged_neck_averaging.tex` が正本。自由な正則normal S¹を先に平均してη=A1ωとし、triple endで残る円を平均してκ=A2ηとする。単一primitive ω=dλとflow/domain bufferの下で、φ*ω=η、ψ*η=κ、Θ=φψについてΘ*λ=A2A1λ+dqとなる。第二flowはnormal circleと可換であるから、各actual torusはneckと同じactual action φρ1φ^−1を含む。μ∘ψ=A2μが厳密に成り立ち、全marked整数cycleのaction periodsを同じλから規格化できる（`ke:staged-neck-averaging`）。

`ke:short-circle-actual-buffer` は、作用不変領域全体でperiod-1 normal generatorがactual計量に関して|V|≤εを満たせば、Moser trajectoryのactual長をc_w ε以下に抑える。c_w=(π/2)||w||₂で、通常kernelならπ/(2√3)、centered kernelならπ/(4√3)。作用不変背景・tensor二側比較・exactnessはこの評価に不要で、forward/backward両flowに成立する。さらにcompact飽和集合Kのactual bufferが(2c_w+1/2)εを超えれば、飽和source OとそのMoser像の両方がKを含む（`ke:short-circle-image-buffer`）。単一primitiveがあれば同じKの近傍にactual Hamiltonian normal actionを得る。全neckの一様な短さ・buffer、C¹とintrinsic fiber径は引き続き別の入力である。

一段階構成、二段階構成、固定整数基底の変更は、共通domain/image bufferの下でHamiltonian isotopyにより比較できる（`ke:staged-hamiltonian-comparison`）。形式のpositive triangle上のpath homotopyとexact primitive transportを明示している。Exact endpoint mapであることだけからHamiltonian性を結論しない。旧bundleと同じfiber partitionとは主張しない。

`ke:staged-closed-corner-gh` は、三重点の標準T²の任意の固定primitive subgroupを第一段に選び、actual closed-corner bundleと同じO(log R/R)の内在・protected-ambient GH評価を与える。Fiberの元の尺度のintrinsic径はO(1/R)。三重点内の定量的bufferは既存のfull-triple比較で検証済みである。

関連KE主稿 `pair:prop:bundle-conic` / `pair:cor:global-primitive` / `pair:cor:actual-common-moment` により、source-freeな固定compact base上では一つの正則normal action、canonical primitive、円平均η_tの共通moment intervalが得られた。Fixed-end momentはperiod1の規約で±4π/(−log r²)を主項とし、r固定後t→0とする。これらからneck全体のnormal Moser flowの生存・bufferや各triple endとの同時一致は従わない。

`ke:staged-reduced-extension` は、marked simple-saddle foliationと適合するreduced end germsの延長を仮定して、regular T²とsaddle S¹×figure-eightを持つneckを接着する。共通normal actionだけでは、別に固定したneckの第二periodやfiberそのものの一致を意味しない。Reduced leaves、内部marking、critical actionの条件を具体的な構成で確認し、全域接着とGH実現へ用いた。任意の独立先指定periodへの適合は結論しない。

## 相対接着で必要なcollar条件
`ke:relative-fiber-preserving` は、torus飽和した開collar N上の元のphase toriが既にactual ω-Lagrangianなら、chain primitive β=Hω、H=K_1+A_1K_2によるMoser flowが各fiberを集合として保ち、p∘φ^−1=p on Nを満たすことを証明する。作用不変性は不要であり、centered chain primitiveでも同じ結論となる。各点を固定することとは異なる。点ごとの固定には、作用不変なcollarとcentered primitiveを用いる既存の `ke:relative-averaging` が使える。

`ke:relative-neck-matching` は、同じorbit partitionを持つactual Lagrangian neck fibrationが開overlap上に与えられれば、基底collarを同定して局所接着できるという条件付きの系である。共通葉と全intersectionの飽和は、許容射影と遅い対角選択を用いた `ke:neck-corner-saturated-union` で別途実証した。定数係数のmonomial座標変更はorbit partitionを保つが、非定数holomorphic unitを含む変更は一般に保たない。任意の別のprimitiveへの置換でもfiber保存が続くとは仮定しない。

## 小さいLagrangian fibersへの局所的な前進
曲面側の着手対象は複素次元2でのKE極限とLagrangian fibrationの適合性である。主稿の `papers/sections/paper/ke_fiber_compatibility.tex` に次の証明を置いた。

- `ke:short-torus-averaging`：自由な正則 $T^2$ 作用、torus不変Hermitian計量 $h$、$c h\le g_\omega\le C h$、torus上のperiod零を仮定する。作用の周期1生成場の長さの和を $e$ とすると、平均化のchain homotopyから長さ $O(e)$ のprimitiveを作り、一つのMoser flowで領域全体にLagrangian fibrationを構成する。変位は $Ce/(2c)$ 以下、ambient fiber diameterは $\sqrt C e(C/c+1/2)$ 以下。高階微分比較は使わない。
- `ke:triple-hexagon`：$\zeta_i\zeta_j\zeta_k=t$ の三つのsquareを一つのhexagonとして全phase torusで実現し、raw-depth mapとの誤差を $O((1+\log m_t)/R_t)$ に抑える。
- `ke:triple-moving-fibration`：全phaseを含む moving domain $\min\ell_a>m_t/2$ 上の一様tensor比較を追加仮定すれば、actual負KE形式に対する局所fibrationが得られ、そのambient fiber diameterは元の尺度でも $O(m_t^{-1})$。$m_t=R_t\to\infty$ とできる。負KE equationにより局所canonical trivialization上で形式がexactとなるのでperiod条件は満たされる。

これらは原稿に条件と証明を保持する局所結果である。Averaging–Moserの基本方法はRuan, arXiv:math/0309177v2, §3に先行し、一般的新規性は未確認。H-minimal/special Lagrangian性、大域接着、singular fibersの計量評価は結論しない。

**解析入力の区別：** 関連KE主稿の `coarse:prop:density-counterexample` により、負KE計量であってもbounded volume densityから一様tensor比較は導けない。五次coarse metric packageには独立な $(\mathrm{TC})_5$ が必要であり、その無条件な検証は未完成である。これは対象compact familyの反例ではない。全深部三重点のfull-orbit moving tensor比較は全固定d≥5で検証済みであり、閉cornerへの局所適用に追加仮定は不要である。Source等を含むexterior全体の一様tensor二側比較は別の未解決問題である。本稿の全域ambient距離比較は、それを仮定しないscalar/portal評価で証明した。

## 中心結果と証明の状態
- 曲面側の分岐基底 \(B_d(T)\) とKE候補 \(\mathcal C_d\) は、labelled cell-like homotopy equivalence \(p_T\) で結ばれる。\(d=5\) では同相、\(d\ge6\) では非同相（`papers/sections/paper/base_topology.tex` の `topo:KE-cubical-comparison`）。
- 人工的PL長さ距離\(d_\varepsilon\)によるgraph correspondenceの誤差は、\(d=5\) で \(\Theta(\varepsilon^2)\)、\(d\ge6\) で \(\Theta(\varepsilon)\)。GH収束は上から同じ次数で評価できるが、\(d\ge6\) にGH距離の同次数の下界を主張しない（`topo:metric-collapse-sharp`）。
- 幾何学的な基底計量で同じ収束を得るための十分条件は、(N) global no-shortcut、(S) square geodesic lifts、(F) small-fiber/portal connectors（`topo:finite-portal-criterion`）。二つのsquareを一頂点で貼った反例（`topo:portal-counterexample`）により、(F) は(N)+(S)からは従わない。これらは抽象的距離論である。本稿のP0では全空間のactual ambient距離を直接扱い、独立のactual action metricの構成・その長さ完備化までは結論していない。
- 六次同時Petersen分岐木系は6通り・\(S_6\)の一軌道で、各安定化群の位数は120。固定木系はfull \(S_6\)-equivariantではない。新規性は未確認。

## 優先する次の一手

1. **三研究を通した依存監査と一次文献比較。** 全域actual構成から局所解析入力・相対接着を逆向きにたどる。指定Kähler形式での一般存在、actual KEの同じ合成写像による計量実現、追加の作用atlas条件の区別を維持し、既知原理・本稿での適用・新規性未確認箇所を整理する。今回の量化点検を全証明の再監査と読み替えない。
2. **五次・六次同時実現の公表範囲を固定する。** `ke:quintic-simultaneous-realization` と `ke:sextic-simultaneous-realization` を入口に、選べるweights・source葉と先指定germsの違いを要約・Introductionへ整合させる。六次の等重み一意性は標準zero-external targetsの下での結論であり、全Petersen atlasに拡張しない。追加保持annuliの内部位置障害は `ke:petersen-two-end-cuts` と研究ノートを参照し、新しい条件を無言で加えない。
3. **主稿の構成と再現。** 統合定理を軸に本文の説明順・参照・要約を整え、有効な証明と独立成果を保持する。必要な組版・表示確認を行い、通常commitで研究repo、続いてhubを更新する。

五次整数接着の \(G_{5,14}\) 中央matching・\(\{4,1,0\}\) 配分・分母三条件、\(G_{5,16}\)、\(G_{5,17}\)、三高係数の同時非負性と一般分母剛性は独立した未解決課題として保持する。必要な26標識は実現数と読み替えない。

## 保存・再現と現在の検証状態

重点点検済みの範囲は、sourceのsingular reductionと固定marked tree、K2全intersection、中央sourceの全点径、全moment退出、基底の接着、sharp scalar障壁、同じ写像の全域上下界、統合主定理と必要なK2/K3の接続を対象とした。DMVの掲載版Theorem 1.2とYauのSchwarz lemmaを一次資料で確認し、Rochon–ZhangのSNC cusp入力、Evans–Mauri Lemma 2.16、および外部KE主稿のdominant-product・fixed-end momentの適用も照合した。全主稿の独立再監査とは区別する。

現行のTeX分割節と検証スクリプトは `papers/sections/` を直接参照し、旧ルートsymlinkに依存しない。静的な構成検査は `python3 verification/verify_repository_layout.py`、現行の五主検算・五独立監査は `python3 verification/run_current_checks.py`。旧JSONやmanifestの相対パス・記録時点のSHA-256は出典情報として保持し、パス正規化後の現行実行パスと区別する。
組版はrepo直下の `latexmk papers/surface-lagrangian-torus-fibration.tex`、整数接着は `latexmk papers/quintic-integer-gluing.tex`。LuaLaTeXとLuaTeX-ja／TikZ／日本語フォントが必要、PDFとSyncTeXはbuild/へ出力しGitで追跡しない。段階別の実行は `scripts/research_check.py` と [Cloud Codexの再開手順](research/cloud-codex.md) を参照する。元の計算コード、入力、証明書は保持する。

**曲面主稿改訂47の検証（2026-11-23）。** Part IVの固定座標・模型に関する局所安定性率の最適性を引用し、指定証明と入力を独立に点検した。Zhang・Ruanの指定一次箇所を実読し、導入の比較範囲は別担当も確認した。LuaLaTeX/latexmkで324頁に組版し、主要log六分類は全て0。1・18–20・323–324頁の6頁を150dpiで実表示し、追加段落・隣接する改頁・関連書誌に欠字・重なり・切断・数式/URLの溢れを認めない。PDF/source hashと確認担当は検証JSONに記す。既存FBP・simplex・source・輸送・core・atlasの指定点検は保持し、一律に再実施したとはしない。全324頁の逐頁検査、全証明・全外部入力の再監査、外部査読、形式証明、包括的新規性確認ではない。静的構成検査は通過し、既存整数証明書は今回再実行していない。

## 共通研究原則と保存許可（研究固有方針から独立）
数学的重要性・新規性・理解の深化・応用可能性・正確性・実現可能性を総合し方針を見直す。証明済み・仮定付き・未完成・予想・計算観察、既知成果と新規性、草稿の証明と今回の独立監査を区別する。重要な先行研究は一次資料の仮定と参照箇所を確認する。日本語LuaLaTeXで十分な証明を保ち、有効な着想・反例・障害は現行ノートへ整理する。再現資産を保持し、旧版ZIP/ログの集積を避ける。研究の区切りでは承諾なしで通常コミットを `main` へpushし、Cloud Codexの長時間作業は切りのよいところ、遅くとも前回成功pushから約15分を目安に現行の有効な成果と未解決箇所を保存する（詳細はAGENTS.md）。force push・GitHub Actions追加/起動をしない。Library旧資料を削除せず、GitHub管理後の定常二重保存は行わない。対象repo保存後にresearch-hubの到達点・核心・次の一手・依存と再開先を更新し、数学検証・組版・push・hub反映を区別する。

GitHub管理前の研究では、区切りごとに現行方針・ノート・論文・必要な再現資産と組版済みPDFをbundleとして承諾なくLibraryへ保存する。移行後は対象repoのmainを正本とし、Libraryはpush不能時の緊急保存または別途指定に用いる。現在有効な内容から再開できる構成を保ち、旧版の復元用アーカイブ、組版中間物、重複実装を現行一式へ蓄積しない。元資料独自の有用内容は移行・検証前に失わず、削除を指示されていない既存Library資料は保持する。
