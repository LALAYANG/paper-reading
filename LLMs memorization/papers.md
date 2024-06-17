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
Summary:
- We compare the attention weights of neural models with the attention that humans pay when reasoning about source code examples.
- Task: method summarization - original method name prediction.
- Models: two neural models
- Two kinds of attention weights: regular attention (showing what tokens the model focuses on) and copy attention (showing what tokens the model considers to copy verbatim into the output)
- RQ1: Are the intrinsic attention weights of neural models correlated with human attention?
  1) Neural models and humans often agree about what tokens to copy verbatim from the input to the output, but less on what other tokens to attend to.
- RQ2: How does the distribution of attention across tokens differ between models and humans?
- RQ3: Do neural models and humans attend to the same kinds of tokens, e.g., identifiers, separators, operators, and keywords?
- RQ4: Do learned models and humans struggle with the same kinds of examples?
  


## Metrics
- No More Manual Tests? Evaluating and Improving ChatGPT for Unit Test Generation (manual user study)
- https://arxiv.org/pdf/2403.16898
- https://arxiv.org/pdf/2311.11690
