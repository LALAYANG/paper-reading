## LLMs memorization

- **Traces of Memorisation in Large Language Models for Code**. ICSE2024. [pdf](https://arxiv.org/pdf/2312.11658) [code] 
```
@inproceedings{al2024traces,
  title={Traces of memorisation in large language models for code},
  author={Al-Kaswan, Ali and Izadi, Maliheh and Van Deursen, Arie},
  booktitle={Proceedings of the IEEE/ACM 46th International Conference on Software Engineering},
  pages={1--12},
  year={2024}
}
```

- **Unveiling Memorization in Code Models**. ICSE2024. [pdf](https://dl.acm.org/doi/pdf/10.1145/3597503.3639074) [code] 
```
@inproceedings{yang2024unveiling,
  title={Unveiling memorization in code models},
  author={Yang, Zhou and Zhao, Zhipeng and Wang, Chenyu and Shi, Jieke and Kim, Dongsun and Han, Donggyun and Lo, David},
  booktitle={Proceedings of the IEEE/ACM 46th International Conference on Software Engineering},
  pages={1--13},
  year={2024}
}
```

- **Neural Code Completion Tools Can Memorize Hard-coded Credentials**. FSE2024. [pdf](https://arxiv.org/pdf/2309.07639) [code]  (full version to be added)
```
bib
```

## LLMs Contamination

- **Investigating Data Contamination for Pre-training Language Models**. [pdf](https://arxiv.org/pdf/2401.06059v1) [code]  (full version to be added)
```
bib
```

## Automated Generation of Benchmarks


- **PPM: Automated Generation of Diverse Programming Problems for Benchmarking Code Generation Models**. FSE2024. [pdf](https://arxiv.org/pdf/2401.15545) [code](https://github.com/SeekingDream/PPM) 
```
@article{chen2024ppm,
  title={PPM: Automated Generation of Diverse Programming Problems for Benchmarking Code Generation Models},
  author={Chen, Simin and Feng, Xiaoning and Han, Xiaohong and Liu, Cong and Yang, Wei},
  journal={arXiv preprint arXiv:2401.15545},
  year={2024}
}
```

- **Top Leaderboard Ranking = Top Coding Proficiency, Always? EvoEval: Evolving Coding Benchmarks via LLM**. [pdf](https://arxiv.org/pdf/2403.19114) [code](https://github.com/evo-eval/evoeval)
```
@article{evoeval,
  author    = {Xia, Chunqiu Steven and Deng, Yinlin and Zhang, Lingming},
  title     = {Top Leaderboard Ranking = Top Coding Proficiency, Always? EvoEval: Evolving Coding Benchmarks via LLM},
  year      = {2024},
  journal   = {arXiv preprint},
}
```
- **CRUXEval: A Benchmark for Code Reasoning, Understanding and Execution**. ICML2024. [pdf](https://arxiv.org/pdf/2401.03065) [code](https://github.com/facebookresearch/cruxeval) 
```
@article{gu2024cruxeval,
  title={Cruxeval: A benchmark for code reasoning, understanding and execution},
  author={Gu, Alex and Rozi{\`e}re, Baptiste and Leather, Hugh and Solar-Lezama, Armando and Synnaeve, Gabriel and Wang, Sida I},
  journal={arXiv preprint arXiv:2401.03065},
  year={2024}
}
```
## Understanding how models reason about code

- **Thinking Like a Developer? Comparing the Attention of Humans with Neural Models of Code**. ASE 2021. [pdf](https://software-lab.org/publications/ase2021.pdf)
```
@inproceedings{paltenghi2021thinking,
  title={Thinking like a developer? comparing the attention of humans with neural models of code},
  author={Paltenghi, Matteo and Pradel, Michael},
  booktitle={2021 36th IEEE/ACM International Conference on Automated Software Engineering (ASE)},
  pages={867--879},
  year={2021},
  organization={IEEE}
}
```

```
Summary:
- We compare the attention weights of neural models with the attention that humans pay when reasoning about source code examples.
- Task: method summarization - original method name prediction.
- Models: two neural models
- Two kinds of attention weights: regular attention (showing what tokens the model focuses on) and copy attention (showing what tokens the model considers to copy verbatim into the output)

Insight 1: Neural models and humans often agree about what tokens to copy verbatim from the input to the output, but less on what other tokens to attend to. The relatively high correlation for copy attention gives an empirical justification to the copy attention mechanisms used by many neural models.
Insight 2: No attention mechanism, among those studied, closely mimics the way humans distributes their attention on the tokens of the method body.
Insight 3: The transformer model seems to be overspecialized in attending only a small subset of tokens, as compared to the convolutional model.
Insight 4: Sometimes the humans do not fully explore the entire method, but base their answers on a subset of the tokens in the methods, typically the beginning (esp. variable declarations) and end (esp. returns and assertions).
Insight 5: High attention paid by the copy attention to identifiers confirms their effectiveness in focusing primarily on tokens that might be copied verbatim into the method name.
Insight 6: Strings, keywords, and operators are often overlooked by the models, whereas the humans give more attention to them.
Insight 7: Block-level separators, such as curly braces, are attended mostly by the models, whereas the humans get this information implicitly from the indentation of the formatted code.
Insight 8: Regular attention of transformers specializes in the recognition of separators that proceed and follow method invocations. This confirms and extends an analogous specialization of multi-head attention observed also in natural language processing [10]. We here confirm that transformers are attentive to separators also when applied to code-related tasks. We hypothesize that recognizing separators is important for the model to understand the role of individual tokens, e.g., that a specific token represents the name of a called method. An interesting future work could be to further explore the root causes of this phenomenon.
Insight 11: Beside getters and setters, neural models often struggle to predict more challenging kinds of methods, such as checkers and test methods, whereas the humans are successful across a wider range of methods.
Insight 12: Longer methods are harder to summarize, both for models and humans.
```

- **Do Large Language Models Pay Similar Attention Like Human Programmers When Generating Code?** FSE 2024.
(Do LLMs attend to similar parts of a task description like human programmers in code generation? )
```
To What Extent Is Model Attention Aligned With Human Attention? 
There is a consistent misalignment between LLM attention and programmer attention in all settings, indicating that LLMs do not reason programming tasks like human programmers.
Can Attention Explain Errors of Code Generation Models? (5.2)
Missing attention to critical conditions. 
Missing Attention to Important Descriptive Words of an Operation or a Data Object. 
Missing Attention to Operation Descriptions.
Missing Attention to Data Types.
Incorrect Mapping Between NL Words and Code Elements.
```

- **When Dataflow Analysis Meets Large Language Models**. [pdf](https://arxiv.org/pdf/2402.10754)
<!--Interesting cases in appendix
- When a branch condition contains a library function, LLMDFA may offer a wrong interpretation of its semantics. to polish operators with lib function calls in branch condition-->

```
An LLM-powered dataflow analysis framework that analyzes arbitrary code snippets without requiring a compilation infrastructure and automatically synthesizes downstream applica- tions.

Inspiration:
can LLMs understand dataflow?
```

- **GraphCodeBERT: Pre-training Code Representations with Data Flow.** ICLR2021.
```
Instead of taking syntactic-level structure of code like abstract syntax tree (AST), we leverage semantic-level information of code, i.e. data flow, for pre- training. Data flow is a graph, in which nodes represent variables and edges represent the relation of “where-the-value-comes-from” between variables.
Def-Use chains
```

## Metrics
- No More Manual Tests? Evaluating and Improving ChatGPT for Unit Test Generation (manual user study)
- https://arxiv.org/pdf/2403.16898
- https://arxiv.org/pdf/2311.11690
