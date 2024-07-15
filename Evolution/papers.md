## Search-based approaches

#### - Pareto Optimal Search Based Refactoring at the Design Level
[paper](https://dl.acm.org/doi/pdf/10.1145/1276958.1277176)

Summary:
- While manually determining useful refactorings can be chal- lenging, search based techniques can automatically discover useful refactorings. Current search based refactoring approaches require metrics to be combined in a complex fash- ion, and produce a single sequence of refactorings.
- In this paper:
we show how Pareto optimality allows users to pick from different optimal sequences of refactorings, according to their preferences; we show that Pareto optimality applies equally to sub-sequences of refactorings, allowing users to pick refactoring sequences based on the resources available to implement those refactorings; we show how Pareto op- timality can be used to compare different fitness functions, and to combine results from different fitness functions.
- **Fitness Function**:  
  A + B; A * B; tuple<A,B>;
  (CBO(C) ∗ SDMPC(C) or CBO(C) + SDMPC(C))

Two categories of search based refactoring and transformation:
- direct：
In the direct approach, the program is directly optimized. That is, the possible variants of the program form the search space of the problem. Using this approach the transforma- tion/refactoring steps are applied directly to the program, denoting moves from the current program to a near neigh- bour in the search space. 

Local search.

- indirect:
In the indirect approach, the program is indirectly opti- mized, via the optimization of the sequence of transforma- tions to apply to the program. In this approach the program is optimized by a sequence of transformations and it is the set of possible sequences of transformations that form the search space.

Fitness is computed by applying the sequence of transformations to the program in question and measuring the improvement in the metrics of interest. In this way, the goal remains the refactoring/transformation of the program, but the optimization is performed on the transformation sequence and fitness is computed indirectly, by applying the transformation sequence to the program.

It's possible to apply global search.

#### - A hierarchical model for object-oriented design quality assessment.
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=979986)

- **Fitness Function**:
Weighting on 11 metrics. Not clear how to select each weight, but seems like based on heuristics...
e.g.,
Understandability = -0.33 * Abstraction + 0.33 * Encapsulation - 0.33 * Coupling + 0.33 * Cohesion - 0.33 * Polymorphism - 0.33 * Complexity - 0.33
* Design Size

#### - Search-based software maintenance
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1602376)

Summary:
The high cost of software maintenance could poten- tially be greatly reduced by the automatic refactoring of object-oriented programs to increase their understandabil- ity, adaptability and extensibility. This paper describes a novel approach in providing automated refactoring support for software maintenance; the formulation of the task as a search problem in the space of alternative designs. Such a search is guided by a quality evaluation function that must accurately reflect refactoring goals. We have constructed a search-based software maintenance tool and report here the results of experimental refactoring of two Java programs, which yielded improvements in terms of the quality func- tions used. We also discuss the comparative merits of the three quality functions employed and the actual effect on program design that resulted from their use.

Search Techniques:
- First-Ascent Hill Climbing (HC1) A local search algo- rithm where the search moves to the first neighbouring solution of a higher quality discovered.
- Steepest-Ascent Hill Climbing (HC2) A local search al- gorithm where the search moves to the neighbouring solution of highest quality.
- Low-Temperature Simulated Annealing (SA) A meta- heuristic search technique described below.

Each metric value for design A is divided by the corresponding value for design B to give the metric change quotient.

Fitness Functions same as above [A hierarchical...]

#### - Metrics Are Fitness Functions Too
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1357891)

#### - The Weights Can Be Harmful: Pareto Search versus Weighted Search in Multi-objective Search-based Software Engineering
[paper](https://dl.acm.org/doi/pdf/10.1145/3514233)

#### - Behind the Intents: An In-depth Empirical Study on Software Refactoring in Modern Code Review
[paper](https://dl.acm.org/doi/pdf/10.1145/3379597.3387475)

#### - Improving Readability of Scratch Programs with Search-based Refactoring
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9610643)

#### - Intelligent Change Operators for Multi-Objective Refactoring
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9678519)

#### - Explainable Search-Based Refactoring
[paper](https://deepblue.lib.umich.edu/bitstream/handle/2027.42/170141/TSE_Explainability__Copy_%20%281%29.pdf?sequence=1)

#### - How Does Refactoring Impact Security When Improving Quality? A Security Aware Refactoring
[paper](https://deepblue.lib.umich.edu/bitstream/handle/2027.42/155871/RefactoringSecurityQMOOD__ICSE____Copy_.pdf)

#### - Many-Objective Software Remodularization Using NSGA-III
[paper](https://dl.acm.org/doi/pdf/10.1145/2729974)

#### - Sapienz: Multi-objective Automated Testing for Android Applications
[paper](https://dl.acm.org/doi/pdf/10.1145/2931037.2931054)  

#### - Search-Based Software Engineering: Trends, Techniques and Applications
[paper](https://dl.acm.org/doi/pdf/10.1145/2379776.2379787)
11.9. Multiobjective Optimization

#### - The weighted sum method for multi-objective optimization: new insights
[paper](https://link.springer.com/content/pdf/10.1007/s00158-009-0460-7.pdf)

#### - Balance
[paper](https://mir.cs.illinois.edu/marinov/publications/XiaETAL23FASER.pdf)

#### - Operator-Based and Random Mutant Selection: Better Together
[paper](http://lingming.cs.illinois.edu/publications/ase2013.pdf)

#### - Faster Mutation Testing Inspired by Test Prioritization and Reduction
[paper](http://lingming.cs.illinois.edu/publications/issta2013a.pdf)

Summary:
- We introduce Sapienz, the first approach offering multi- objective automated Android app exploratory testing that seeks to maximise code coverage and fault revelation, while minimising the length of fault-revealing test sequences.
- Our goal is to produce an entirely automated approach that max- imises fault revelation with short test sequences. The key insight in our approach is that minimising test sequence length and maximising other objectives can be combined in a Pareto-optimal multi-objective search-based approach to Android testing. 
- Three objectives: code coverage, sequence length and the number of crashes found.

#### - Analysing the fitness landscape of search-based software testing problems
[paper](https://link.springer.com/content/pdf/10.1007/s10515-016-0197-7.pdf)

#### - Graph-Based Seed Object Synthesis for Search-Based Unit Testing
[paper](https://dl.acm.org/doi/pdf/10.1145/3468264.3468619)

#### - Search-Based Energy Testing of Android
[paper](https://dl.acm.org/doi/pdf/10.1109/ICSE.2019.00115)

#### - DeGPT: Optimizing Decompiler Output with LLM
[paper](https://www.ndss-symposium.org/wp-content/uploads/2024-401-paper.pdf)

#### - Pareto Efficient Multi-Objective Test Case Selection
[paper](http://web4.cs.ucl.ac.uk/staff/S.Yoo/papers/Yoo2007dq.pdf)

## Readability

#### - A Metric for Software Readability
[paper](https://web.eecs.umich.edu/~weimerw/p/weimer-issta2008-readability.pdf)

#### - A Simpler Model of Software Readability
[paper](https://dl.acm.org/doi/pdf/10.1145/1985441.1985454)

#### - On the Naturalness of Software
[paper](https://dl.acm.org/doi/pdf/10.5555/2337223.2337322)

#### - Automatically Assessing Code Understandability: How Far Are We?
[paper](https://www.cs.wm.edu/~denys/pubs/ASE'17-Readability.pdf)

#### - No More Manual Tests? Evaluating and Improving ChatGPT for Unit Test Generation.
[paper](https://arxiv.org/pdf/2305.04207)

#### - Search-based Automatic Repair for Fairness and Accuracy in Decision-making Software
[paper](https://discovery.ucl.ac.uk/id/eprint/10185565/1/s10664-023-10419-3.pdf)

#### - Learning a Metric for Code Readability
[paper](https://web.eecs.umich.edu/~weimerw/p/weimer-tse2010-readability-preprint.pdf)

#### WaDec: Decompile WebAssembly Using Large Language Model
[paper](https://arxiv.org/pdf/2406.11346)
- Code readability is fundamentally determined by two main factors: Syntactic Completeness and Code Bloat.
- Code Bloat. One of the most intuitive indicators of code readability is the change in the number of lines of code. We assume that the readability of the source code is relatively high, and recovering the source code is a primary goal of decompilation. Therefore, introducing code bloat, the rate of expansion in the number of code lines, as a metric is a wise choice.
- Syntactic Completeness & Function Completeness. Syntactic completeness is a foundational metric for the legitimacy of code syntax and is widely adopted in the field. This metric measures the proportion of syntactically complete code relative to the total codebase, with the help of tree-sitter, which can determine whether a piece of code or a function has errors. Additionally, syntactic completeness underpins compilability; code that is not syntactically complete is inherently uncompileable. Function completeness refers to whether the decompiled code includes all the functions from the source code.

#### R2I: A Relative Readability Metric for Decompiled Code


#### An Empirical Study of the Relationships between Code Readability and Software Complexity.
[paper](https://arxiv.org/pdf/1909.01760)

#### Modeling Readability to Improve Unit Tests
[paper](https://web.eecs.umich.edu/~weimerw/p/p107-daka.pdf)

## Other Metrics

#### - CodeBLEU: a Method for Automatic Evaluation of Code Synthesis 
[paper](https://arxiv.org/pdf/2009.10297)

#### - Cognitive Complexity
[technical report](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://www.sonarsource.com/docs/CognitiveComplexity.pdf&ved=2ahUKEwjD3uLctIuHAxWRv4kEHb80DS0QFnoECDkQAQ&usg=AOvVaw0CP7Ad2hDUAXwwKJhH0McN)
[two-pages paper](https://dl.acm.org/doi/pdf/10.1145/3194164.3194186)

#### - A Complexity Measure
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1702388)




## Statistical Analysis

#### A Practical Guide for Using Statistical Tests to Assess Randomized Algorithms in Software Engineering
[paper](https://dl.acm.org/doi/pdf/10.1145/1985793.1985795)
