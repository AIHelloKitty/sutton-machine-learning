# 第一章

# **Contents**

[**Preface to the Second** **Edition**](#bookmark0)	**xiii**

[**Preface to the First** **Edition**](#bookmark3)	**xvii**

[**Summary of** **Notation**](#bookmark5)	**xix**

1 [**Introduction**](#bookmark7)	**1**

[Reinforcement Learning](#bookmark9)	1

[Examples](#bookmark14)	4

[Elements of Reinforcement Learning](#bookmark17)	6

[Limitations and Scope](#bookmark19)	7

[An Extended Example: Tic-Tac-Toe](#bookmark21)	8

[Summary](#bookmark27)	13

[Early History of Reinforcement Learning](#bookmark28)	13

[**I**	**Tabular** **Solution** **Methods**](#bookmark39)	**23**

2 [**Multi-armed**  **Bandits**](#bookmark41)	**25**

[A *k* -armed Bandit  Problem](#bookmark43)	25

[Action-value Methods](#bookmark46)	27

[The 10-armed Testbed](#bookmark49)	28

[Incremental Implementation](#bookmark53)	30

[Tracking a Nonstationary Problem](#bookmark58)	32

[Optimistic Initial Values](#bookmark63)	34

[Upper-Confidence-Bound Action Selection](#bookmark68)	35

[Gradient Bandit Algorithms](#bookmark71)	37

[Associative Search (Contextual Bandits)](#bookmark78)	41

[Summary](#bookmark80)	42

vii

3 [**Finite** **Markov** **Decision** **Processes**](#bookmark86)	**47**

[The Agent-Environment Interface](#bookmark88)	47

[Goals and Rewards](#bookmark104)	53

[Returns and Episodes](#bookmark106)	54

[Unified Notation for Episodic and Continuing Tasks](#bookmark118)	57

[Policies and Value Functions](#bookmark120)	58

[Optimal Policies and Optimal Value Functions](#bookmark134)	62

[Optimality and Approximation](#bookmark144)	67

[Summary](#bookmark145)	68

4 [**Dynamic** **Programming**](#bookmark149)	**73**

[Policy Evaluation (Prediction)](#bookmark153)	74

[Policy Improvement](#bookmark160)	76

[Policy Iteration](#bookmark168)	80

[Value Iteration](#bookmark174)	82

[Asynchronous Dynamic Programming](#bookmark181)	85

[Generalized Policy Iteration](#bookmark183)	86

[Efficiency of Dynamic Programming](#bookmark185)	87

[Summary](#bookmark187)	88

5 [**Monte Carlo** **Methods**](#bookmark191)	**91**

[Monte Carlo Prediction](#bookmark194)	92

[Monte Carlo Estimation of Action Values](#bookmark201)	96

[Monte Carlo Control](#bookmark203)	97

[Monte Carlo Control without Exploring Starts](#bookmark208)	100

[Off-policy Prediction via Importance Sampling](#bookmark212)	103

[Incremental Implementation](#bookmark224)	108

[Off-policy Monte Carlo Control](#bookmark230)	110

[*Discounting-aware Importance Sampling](#bookmark236)	112

[*Per-decision Importance Sampling](#bookmark239)	113

[Summary](#bookmark243)	115

6 [**Temporal-Difference** **Learning**](#bookmark247)	**119**

[TD Prediction](#bookmark249)	119

[Advantages of TD Prediction Methods](#bookmark262)	124

[Optimality of TD(0)](#bookmark267)	126

[Sarsa: On-policy TD Control](#bookmark273)	129

[Q-learning: Off-policy TD Control](#bookmark276)	131

[Expected Sarsa](#bookmark279)	133

[Maximization Bias and Double Learning](#bookmark285)	134

[Games, Afterstates, and Other Special Cases](#bookmark289)	136

[Summary](#bookmark291)	138

7 [*n***-step** **Bootstrapping**](#bookmark295)	**141**

[*n*-step TD Prediction](#bookmark297)	142

[*n*-step Sarsa](#bookmark308)	145

[*n*-step Off-policy Learning by Importance Sampling](#bookmark318)	148

[*Per-decision Off-policy Methods with Control Variates](#bookmark323)	150

[Off-policy Learning Without Importance Sampling:](#bookmark329)

[The *n*-step Tree Backup  Algorithm](#bookmark329)	152

[*A Unifying Algorithm: *n*-step *Q*(*σ*)](#bookmark334)	154

[Summary](#bookmark339)	157

8 [**Planning and Learning with** **Tabular** **Methods**](#bookmark341)	**159**

[Models and Planning](#bookmark343)	159

[Dyna: Integrated Planning, Acting, and Learning](#bookmark347)	161

[When the Model Is Wrong](#bookmark357)	166

[Prioritized Sweeping](#bookmark362)	168

[Expected vs. Sample Updates](#bookmark368)	172

[Trajectory Sampling](#bookmark374)	174

[Real-time Dynamic Programming](#bookmark379)	177

[Planning at Decision Time](#bookmark382)	180

[Heuristic Search](#bookmark384)	181

[Rollout Algorithms](#bookmark389)	183

[Monte Carlo Tree Search](#bookmark392)	185

[Summary of the Chapter](#bookmark395)	188

[Summary of Part I: Dimensions](#bookmark397)	189

###### [**II**	**Approximate Solution** **Methods**](#bookmark401)	**195**

9 [**On-policy Prediction with** **Approximation**](#bookmark405)	**197**

[Value-function Approximation](#bookmark407)	198

![img](file:///C:\Users\Hao\AppData\Local\Temp\ksohtml\wpsDE1A.tmp.png)[The Prediction Objective (VE)](#bookmark409)	199

[Stochastic-gradient and Semi-gradient Methods](#bookmark416)	200

[Linear Methods](#bookmark430)	204

[Feature Construction for Linear Methods](#bookmark442)	210

[Polynomials](#bookmark444)	210

[Fourier Basis](#bookmark447)	211

[Coarse Coding](#bookmark454)	215

[Tile Coding](#bookmark460)	217

[Radial Basis Functions](#bookmark469)	221

[Selecting Step-Size Parameters Manually](#bookmark471)	222

[Nonlinear Function Approximation: Artificial Neural Networks](#bookmark473)	223

[Least-Squares TD](#bookmark480)	228

[Memory-based Function Approximation](#bookmark486)	230

[Kernel-based Function Approximation](#bookmark489)	232

[Looking Deeper at On-policy Learning: Interest and Emphasis](#bookmark493)	234

[Summary](#bookmark497)	236

10 [**On-policy Control with** **Approximation**](#bookmark503)	**243**

[Episodic Semi-gradient Control](#bookmark505)	243

[Semi-gradient *n*-step Sarsa](#bookmark516)	247

[Average Reward: A New Problem Setting for Continuing Tasks](#bookmark521)	249

[Deprecating the Discounted Setting](#bookmark535)	253

[Differential Semi-gradient *n*-step Sarsa](#bookmark537)	255

[Summary](#bookmark539)	256

11 [***Off-policy Methods with** **Approximation**](#bookmark541)	**259**

[Semi-gradient Methods](#bookmark544)	260

[Examples of Off-policy Divergence](#bookmark549)	262

[The Deadly Triad](#bookmark558)	266

[Linear Value-function Geometry](#bookmark560)	268

[Gradient Descent in the Bellman Error](#bookmark571)	271

[The Bellman Error is Not Learnable](#bookmark580)	276

[Gradient-TD Methods](#bookmark587)	280

[Emphatic-TD Methods](#bookmark596)	283

[Reducing Variance](#bookmark600)	285

[Summary](#bookmark602)	286

12 [**Eligibility** **Traces**](#bookmark605)	**289**

[The *λ*-return](#bookmark608)	290

[TD(*λ*)](#bookmark622)	294

[*n*-step Truncated *λ*-return Methods](#bookmark631)	297

[Redoing Updates: The Online *λ*-return Algorithm](#bookmark637)	299

[True Online TD(*λ*)](#bookmark640)	301

[Dutch Traces in Monte Carlo Learning](#bookmark645)	303

[Sarsa(*λ*)](#bookmark649)	305

[Variable *λ* and *γ*](#bookmark660)	309

[Off-policy Eligibility Traces with Control Variates](#bookmark668)	311

[Watkins's Q(*λ*) to Tree-Backup(*λ*)](#bookmark678)	314

[Stable Off-policy Methods with Traces](#bookmark683)	316

[Implementation Issues](#bookmark687)	318

[Conclusions](#bookmark688)	319

13 [**Policy Gradient** **Methods**](#bookmark693)	**323**

[Policy Approximation and its Advantages](#bookmark698)	324

[The Policy Gradient Theorem](#bookmark703)	326

[REINFORCE: Monte Carlo Policy Gradient](#bookmark708)	328

[REINFORCE with Baseline](#bookmark713)	331

[Actor-Critic Methods](#bookmark719)	333

[Policy Gradient for Continuing Problems](#bookmark722)	335

[Policy Parameterization for Continuous Actions](#bookmark730)	337

[Summary](#bookmark735)	339

###### [**III**	**Looking** **Deeper**](#bookmark736)	**341**

14 [**Psychology**](#bookmark738)	**343**

[Prediction and Control](#bookmark741)	344

[Classical Conditioning](#bookmark743)	345

[Blocking and Higher-order Conditioning](#bookmark747)	347

[The Rescorla-Wagner Model](#bookmark751)	348

[The TD Model](#bookmark759)	351

[TD Model Simulations](#bookmark762)	352

[Instrumental Conditioning](#bookmark774)	359

[Delayed Reinforcement](#bookmark779)	363

[Cognitive Maps](#bookmark782)	365

[Habitual and Goal-directed Behavior](#bookmark784)	366

[Summary](#bookmark789)	370

15 [**Neuroscience**](#bookmark795)	**379**

[Neuroscience Basics](#bookmark797)	380

[Reward Signals, Reinforcement Signals, Values, and Prediction Errors](#bookmark799). . 382

[The Reward Prediction Error Hypothesis](#bookmark803)	383

[Dopamine](#bookmark807)	385

[Experimental Support for the Reward Prediction Error Hypothesis](#bookmark812)	389

[TD Error/Dopamine Correspondence](#bookmark815)	392

[Neural Actor-Critic](#bookmark818)	397

[Actor and Critic Learning Rules](#bookmark822)	400

[Hedonistic Neurons](#bookmark830)	404

[Collective Reinforcement Learning](#bookmark833)	406

[Model-based Methods in the Brain](#bookmark837)	409

[Addiction](#bookmark840)	411

[Summary](#bookmark842)	412

16 [**Applications and Case** **Studies**](#bookmark849)	**423**

[TD-Gammon](#bookmark851)	423

[Samuel's Checkers Player](#bookmark860)	428

[Watson's Daily-Double Wagering](#bookmark865)	431

[Optimizing Memory Control](#bookmark871)	434

[Human-level Video Game Play](#bookmark877)	438

[Mastering the Game of Go](#bookmark882)	443

[AlphaGo](#bookmark884)	446

[AlphaGo Zero](#bookmark888)	449

[Personalized Web Services](#bookmark891)	452

[Thermal Soaring](#bookmark894)	455

17 [**Frontiers**](#bookmark900)	**461**

[General Value Functions and Auxiliary Tasks](#bookmark902)	461

[Temporal Abstraction via Options](#bookmark905)	463

[Observations and State](#bookmark912)	466

[Designing Reward Signals](#bookmark919)	470

[Remaining Issues](#bookmark924)	473

[Reinforcement Learning and the Future of Artificial Intelligence](#bookmark929)	476

