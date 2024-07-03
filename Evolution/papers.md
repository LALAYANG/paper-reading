## Search-based approaches

#### Sapienz: Multi-objective Automated Testing for Android Applications

[paper](https://dl.acm.org/doi/pdf/10.1145/2931037.2931054)  

Summary:
- We introduce Sapienz, the first approach offering multi- objective automated Android app exploratory testing that seeks to maximise code coverage and fault revelation, while minimising the length of fault-revealing test sequences.
- Our goal is to produce an entirely automated approach that max- imises fault revelation with short test sequences. The key insight in our approach is that minimising test sequence length and maximising other objectives can be combined in a Pareto-optimal multi-objective search-based approach to Android testing. 
- Three objectives: code coverage, sequence length and the number of crashes found.

#### Analysing the fitness landscape of search-based software testing problems
[paper](https://link.springer.com/content/pdf/10.1007/s10515-016-0197-7.pdf)

#### Graph-Based Seed Object Synthesis for Search-Based Unit Testing
[paper](https://dl.acm.org/doi/pdf/10.1145/3468264.3468619)

#### Search-Based Energy Testing of Android
[paper](https://dl.acm.org/doi/pdf/10.1109/ICSE.2019.00115)

================================================================

#### Pareto Optimal Search Based Refactoring at the Design Level
[paper](https://dl.acm.org/doi/pdf/10.1145/1276958.1277176)

**Two categories of search based refactoring and transformation:**
- direct：
In the direct approach, the program is directly optimized. That is, the possible variants of the program form the search space of the problem. Using this approach the transforma- tion/refactoring steps are applied directly to the program, denoting moves from the current program to a near neigh- bour in the search space. 

Local search.

- indirect:
In the indirect approach, the program is indirectly opti- mized, via the optimization of the sequence of transforma- tions to apply to the program. In this approach the program is optimized by a sequence of transformations and it is the set of possible sequences of transformations that form the search space.

Fitness is computed by applying the sequence of transformations to the program in question and measuring the improvement in the metrics of interest. In this way, the goal remains the refactoring/transformation of the program, but the optimization is performed on the transformation sequence and fitness is computed indirectly, by applying the transformation sequence to the program.

It's possible to apply global search.

- A + B; A * B; tuple<A,B>

#### The Weights Can Be Harmful: Pareto Search versus Weighted Search in Multi-objective Search-based Software Engineering
[paper](https://dl.acm.org/doi/pdf/10.1145/3514233)

#### Behind the Intents: An In-depth Empirical Study on Software Refactoring in Modern Code Review
[paper](https://dl.acm.org/doi/pdf/10.1145/3379597.3387475)

#### Improving Readability of Scratch Programs with Search-based Refactoring
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9610643)

#### Intelligent Change Operators for Multi-Objective Refactoring
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9678519)

#### Explainable Search-Based Refactoring
[paper](https://deepblue.lib.umich.edu/bitstream/handle/2027.42/170141/TSE_Explainability__Copy_%20%281%29.pdf?sequence=1)

#### How Does Refactoring Impact Security When Improving Quality? A Security Aware Refactoring
[paper](https://deepblue.lib.umich.edu/bitstream/handle/2027.42/155871/RefactoringSecurityQMOOD__ICSE____Copy_.pdf)

#### Many-Objective Software Remodularization Using NSGA-III
[paper](https://dl.acm.org/doi/pdf/10.1145/2729974)

#### Search-based software maintenance
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1602376)

## Readability

#### A Metric for Software Readability
[paper](https://web.eecs.umich.edu/~weimerw/p/weimer-issta2008-readability.pdf)

#### A Simpler Model of Software Readability
[paper](https://dl.acm.org/doi/pdf/10.1145/1985441.1985454)

#### On the Naturalness of Software
[paper](https://dl.acm.org/doi/pdf/10.5555/2337223.2337322)

#### Automatically Assessing Code Understandability: How Far Are We?
[paper](https://www.cs.wm.edu/~denys/pubs/ASE'17-Readability.pdf)

#### No More Manual Tests? Evaluating and Improving ChatGPT for Unit Test Generation.
[paper](https://arxiv.org/pdf/2305.04207)


## Metrics

#### CodeBLEU: a Method for Automatic Evaluation of Code Synthesis 
[paper](https://arxiv.org/pdf/2009.10297)

#### Cognitive Complexity
[technical report](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://www.sonarsource.com/docs/CognitiveComplexity.pdf&ved=2ahUKEwjD3uLctIuHAxWRv4kEHb80DS0QFnoECDkQAQ&usg=AOvVaw0CP7Ad2hDUAXwwKJhH0McN)
[two-pages paper](https://dl.acm.org/doi/pdf/10.1145/3194164.3194186)

#### A Complexity Measure
[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1702388)




## Statistical Analysis

#### A Practical Guide for Using Statistical Tests to Assess Randomized Algorithms in Software Engineering
[paper](https://dl.acm.org/doi/pdf/10.1145/1985793.1985795)
