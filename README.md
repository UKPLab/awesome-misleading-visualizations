# Awesome misleading visualizations

<img src='https://img.shields.io/badge/Last update-09/2025-green'>

A curated collection of papers, datasets, and resources on the topic of misleading visualizations and their interaction with AI research 📊🤖

This field is growing fast, and we’ll keep this repo updated with the latest work 🔥.
If you find it useful, don’t forget to leave a star ⭐ to stay in the loop!

💡 We also welcome contributions from the community. Feel free to open a PR and help make this collection even better.

Contact person: [Jonathan Tonglet](mailto:jonathan.tonglet@tu-darmstadt.de) 

[UKP Lab](https://www.ukp.tu-darmstadt.de/) | [TU Darmstadt](https://www.tu-darmstadt.de/)

Don't hesitate to send us an e-mail or report an issue, if something is broken (and it shouldn't be) or if you have further questions. 

## Table of Contents
- [QA with misleading visualizations](#qa-with-misleading-visualizations)
  - [QA papers](#qa-papers)
  - [QA datasets](#qa-datasets)
- [Misleading visualization detection and correction](#misleading-visualization-detection-and-correction)
  - [Detection papers](#detection-papers)
    - [Rule-based linters](#rule-based-linters)
    - [AI models](#ai-models)
  - [Detection datasets](#detection-datasets)
- [Analyses and taxonomies](#analyses-and-taxonomies)
- [Automated fact-checking with visualizations](#automated-fact-checking-with-visualizations)


## QA with misleading visualizations

The deceptive power of misleading visualizations has traditionally been studied through human subject experiments. More recently, researchers have begun testing AI models with similar setups to measure their vulnerability to misleading charts, and to design methods that make them more robust.

### QA papers

- [__An Empirical Evaluation of the GPT-4 Multimodal Language Model on Visualization Literacy Tasks__](https://dl.acm.org/doi/10.1109/TVCG.2024.3456155)

  _Alexander Bendeck, John Stasko_. September 2024. <img src='https://img.shields.io/badge/TVCG-2024-green'>
  <a href='https://osf.io/f39j6/files/osfstorage'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Advancing Multimodal Large Language Models in Chart Question Answering with Visualization-Referenced Instruction Tuning__](https://dl.acm.org/doi/10.1109/TVCG.2024.3456159)

  _Xingchen Zeng, Haichuan Lin, Yilin Ye, Wei Zeng_. January 2025. <img src='https://img.shields.io/badge/TVCG-2024-green'>
  <a href='https://github.com/zengxingchen/ChartQA-MLLM'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Protecting multimodal large language models against misleading visualizations__](https://arxiv.org/abs/2502.20503)

  _Jonathan Tonglet, Tinne Tuytelaars, Marie-Francine Moens, Iryna Gurevych_. February 2025. <img src='https://img.shields.io/badge/arXiv-2025-green'>
  <a href='https://github.com/UKPLab/arxiv2025-misleading-visualizations'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Unmasking Deceptive Visuals: Benchmarking Multimodal Large Language Models on Misleading Chart Question Answering__](https://arxiv.org/abs/2503.18172)

  _Zixin Chen, Sicheng Song, Kashun Shum, Yanna Lin, Rui Sheng, Huamin Qu_. March 2025. <img src='https://img.shields.io/badge/EMNLP-2025-green'>

- [__Benchmarking Visual Language Models on Standardized Visualization Literacy Tests__](https://onlinelibrary.wiley.com/doi/10.1111/cgf.70137?af=R)

  _Saugat Pandey, Alvitta Ottley_. March 2025. <img src='https://img.shields.io/badge/EuroVis-2025-green'>
  <a href='https://github.com/washuvis/VisLit-VLM-Eval'><img src='https://img.shields.io/badge/code-blue'></a>

- [__CHARTOM: A Visual Theory-of-Mind Benchmark for LLMs on Misleading Charts__](https://arxiv.org/abs/2408.14419v3)

  _Shubham Bharti, Shiyun Cheng, Jihyun Rho, Jianrui Zhang, Mu Cai, Yong Jae Lee, Martina Rau, Xiaojin Zhu_. June 2025. <img src='https://img.shields.io/badge/arXiv-2025-green'>

- [__The Perils of Chart Deception: How Misleading Visualizations Affect Vision-Language Models__](https://arxiv.org/abs/2508.09716)

  _Ridwan Mahbub, Mohammed Saidul Islam, Md Tahmid Rahman Laskar, Mizanur Rahman, Mir Tafseer Nayeem, Enamul Hoque_. August 2025. <img src='https://img.shields.io/badge/VIS-2025-green'>
 <a href='https://github.com/vis-nlp/visDeception'><img src='https://img.shields.io/badge/code-blue'></a>



### QA datasets

| Year | Title | Venue | Type | Paper | Dataset | 
| --- | --- |  --- |  --- | --- | --- | 
| 2015 | **Pandey et al.** | CHI | Likert-scale, MCQ | [Link](https://dl.acm.org/doi/10.1145/2702123.2702608) | - |
| 2020 | **Lauer et O'Brien** | SIGDOC |  Likert-scale | [Link](https://dl.acm.org/doi/10.1145/3380851.3416762) |  [Link](https://github.com/UKPLab/arxiv2025-misleading-visualizations) |
| 2023 | **CALVI** | CHI | MCQ |  [Link](https://dl.acm.org/doi/10.1145/3544548.3581406) | [Link](https://github.com/UKPLab/arxiv2025-misleading-visualizations/tree/main)| 
| 2025 | **CHARTOM** | arXiv | MCQ, free-text, rank | [Link](https://arxiv.org/abs/2408.14419v3) | Contact authors | 
| 2025 | **Real-world** |arXiv | MCQ | [Link](https://arxiv.org/abs/2502.20503) | [Link](https://github.com/UKPLab/arxiv2025-misleading-visualizations)| 
| 2025 | **Misleading ChartQA** | EMNLP | MCQ | [Link](https://arxiv.org/abs/2503.18172) | [Link](https://github.com/CinderD/MisleadingChartQA) | 
| 2025 | **Mahbub et al.** | VIS | Likert-scale | [Link](https://arxiv.org/abs/2508.09716) | [Link](https://github.com/vis-nlp/visDeception) |

## Misleading visualization detection and correction

Other works introduce datasets and detection techniques aimed at identifying whether a visualization is misleading, and identifying the specific issues it contains.

### Detection papers

#### Rule-based linters

- [__Surfacing Visualization Mirages__](https://dl.acm.org/doi/10.1145/3313831.3376420)

  _Andrew McNutt, Gordon Kindlmann, Michael Correll_. April 2020. <img src='https://img.shields.io/badge/CHI-2020-green'>

- [__VisuaLint: Sketchy In Situ Annotations of Chart Construction Errors__](https://onlinelibrary.wiley.com/doi/10.1111/cgf.13975)

  _Aspen K. Hopkins, Michael Correll, Arvind Satyanarayan_. July 2020. <img src='https://img.shields.io/badge/EuroVIS-2020-green'>

- [__VizLinter: A Linter and Fixer Framework for Data Visualization__](https://dl.acm.org/doi/10.1109/TVCG.2021.3114804)

  _Qing Chen, Fuling Sun, Xinyue Xu, Zui Chen, Jiazhe Wang, Nan Cao_. January 2022. <img src='https://img.shields.io/badge/TVCG-2021-green'>

- [__Annotating Line Charts for Addressing Deception__](https://dl.acm.org/doi/abs/10.1145/3491102.3502138)

  _Arlen Fan, Yuxin Ma, Michelle Mancenido, Ross Maciejewski_. April 2022. <img src='https://img.shields.io/badge/CHI-2022-green'>

- [__ChartChecker: A User-Centred Approach to Support the Understanding of Misleading Charts__](https://dl.acm.org/doi/10.1145/3715336.3735784)

  _Tom Biselli, Katrin Hartwig, Niklas Kneissl, Louis Pouliot, Christian Reuter_. July 2025. <img src='https://img.shields.io/badge/DIS-2025-green'>

#### AI models

- [__Can GPT-4 Models Detect Misleading Visualizations?__](https://ieeexplore.ieee.org/abstract/document/10771149)

  _Jason Alexander, Priyal Nanda, Kai-Cheng Yang, Ali Sarvghad_. October 2024. <img src='https://img.shields.io/badge/VIS-2024-green'>


- [__How Good (Or Bad) Are LLMs at Detecting Misleading Visualizations?__](https://dl.acm.org/doi/abs/10.1109/TVCG.2024.3456333)

  _Leo Yu-Ho Lo, Huamin Qu_. January 2025. <img src='https://img.shields.io/badge/TVCG-2024-green'>

- [__Automated Pipeline for Detecting and Analyzing Misleading Visual Elements__](https://ieeexplore.ieee.org/abstract/document/11021031)

  _Min Hyeong Kim, Yumin Song, Yungun Kim, Aeri Cho, Soohyun Lee, Hyeon Jeon_. April 2025. <img src='https://img.shields.io/badge/PacificVis-2025-green'>
  <a href='https://osf.io/dn6gs/'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Boosting Data Literacy: The Role of AI in Teaching Detection of Deceptive Charts__](https://link.springer.com/chapter/10.1007/978-3-031-98414-3_7)

  _Konrad J. Maciborski, Karolina Wysocka, Karolina Żelazowska-Byczkowska, Styliani Kleanthous, Adam Wierzbicki_. July 2025. <img src='https://img.shields.io/badge/LNAI-2025-green'>
  <a href='https://osf.io/at3gd/files/osfstorage?view_only=ae8e153d84c14af1ad4d174b767e5c7c'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Automated Visualization Makeovers with LLMs__](https://arxiv.org/abs/2508.05637)

  _Siddharth Gangwar, David A. Selby, Sebastian J. Vollmer_. July 2025. <img src='https://img.shields.io/badge/arXiv-2025-green'>
  <a href='https://osf.io/4tb87'><img src='https://img.shields.io/badge/code-blue'></a>  

- [__MisVisFix: An Interactive Dashboard for Detecting, Explaining, and Correcting Misleading Visualizations using Large Language Models__](https://arxiv.org/abs/2508.04679v1)

  _Amit Kumar Das, Klaus Mueller_. August 2025. <img src='https://img.shields.io/badge/VIS-2025-green'>
  <a href='https://github.com/vhcailab/MisVisFix'><img src='https://img.shields.io/badge/code-blue'></a>

- [__Is this chart lying to me? Automating the detection of misleading visualizations__](https://arxiv.org/abs/2508.21675)

  _Jonathan Tonglet, Jan Zimny, Tinne Tuytelaars, Iryna Gurevych_. August 2025. <img src='https://img.shields.io/badge/arXiv-2025-green'>
  <a href='https://github.com/UKPLab/arxiv2025-misviz'><img src='https://img.shields.io/badge/code-blue'></a>

- [__True (VIS) Lies: A Preliminary Analysis of How Generative AI is Capable of Recognizing Visualization Lies and their Rhetoric__](https://visxgenai.github.io/)
 
  _Graziano Blasilli, Marco Angelini_. November 2025. <img src='https://img.shields.io/badge/VISxGenAI-2025-green'>

### Detection datasets

| Year | Title | Venue | Type |  Paper | Dataset | 
| --- | --- |  --- |  --- |   --- | --- | 
| 2024 | **MISCHA-QA** | - | Synthetic |  - |  [Link](https://huggingface.co/datasets/chart-misinformation-detection/MISCHA-QA) |
| 2025 | **DCDM**  | LNAI | Synthetic |  [Link](https://link.springer.com/chapter/10.1007/978-3-031-98414-3_7) |  [Link](https://osf.io/at3gd/files/osfstorage?view_only=ae8e153d84c14af1ad4d174b767e5c7c) |
| 2025 | **Misvisfix** | VIS |  Real-world |  [Link](https://arxiv.org/abs/2508.04679v1) |  [Link](https://github.com/vhcailab/MisVisFix) |
| 2025 | **Misviz** | arXiv  | Real-world | [Link](https://arxiv.org/abs/2508.21675) | [Link](https://github.com/UKPLab/arxiv2025-misviz) | 
| 2025 | **Misviz-synth** | arXiv  | Synthetic | [Link](https://arxiv.org/abs/2508.21675) | [Link](https://github.com/UKPLab/arxiv2025-misviz) | 

## Analyses and taxonomies

The following studies provide taxonomies of misleading visualizations and analyze their impact on web users.

- [__Misinformed by Visualization: What Do We Learn From Misinformative Visualizations?__](https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.14559)

  _Leo Yu-Ho Lo, Ayush Gupta, Kento Shigyo, Aoyu Wu, Enrico Bertini, Huamin Qu_. August 2022. <img src='https://img.shields.io/badge/EuroVis-2022-green'>

- [__Misleading Beyond Visual Tricks: How People Actually Lie with Charts__](https://dl.acm.org/doi/10.1145/3544548.3580910)

  _Maxim Lisnic, Cole Polychronis, Alexander Lex, Marina Kogan_. April 2023. <img src='https://img.shields.io/badge/CHI-2023-green'>

- [__"Yeah, this graph doesn't show that": Analysis of Online Engagement with Misleading Data Visualizations__](https://dl.acm.org/doi/10.1145/3613904.3642448)

  _Maxim Lisnic, Alexander Lex, Marina Kogan_. May 2024. <img src='https://img.shields.io/badge/CHI-2024-green'>

- [__“I Came Across a Junk”: Understanding Design Flaws of Data Visualization from the Public’s Perspective__](https://dl.acm.org/doi/10.1109/TVCG.2024.3456341)

  _Xingyu Lan, Yu Liu_. January 2025. <img src='https://img.shields.io/badge/TVCG-2024-green'>

## Automated fact-checking with visualizations

Some works have explored scenarios where the visualizations are not deceiving. Instead, they are used as reliable evidence to detect false claims with automated fact-checking systems.

- [__Reading and Reasoning over Chart Images for Evidence-based Automated Fact-Checking__](https://aclanthology.org/2023.findings-eacl.30/)

  _Mubashara Akhtar, Oana Cocarascu, Elena Simperl_. May 2023. <img src='https://img.shields.io/badge/EACL Findings-2023-green'>
  <a href='https://github.com/mubasharaak/ChartFC_chartBERT'><img src='https://img.shields.io/badge/code-blue'></a>

- [__ChartCheck: Explainable Fact-Checking over Real-World Chart Images__](https://aclanthology.org/2024.findings-acl.828/)

  _Mubashara Akhtar, Nikesh Subedi, Vivek Gupta, Sahar Tahmasebi, Oana Cocarascu, Elena Simperl_. AUgust 2024. <img src='https://img.shields.io/badge/ACL Findings-2024-green'>
  <a href='https://aclanthology.org/2024.findings-acl.828/'><img src='https://img.shields.io/badge/code-blue'></a>

- [__ClimateViz: A Benchmark for Statistical Reasoning and Fact Verification on Scientific Charts__](https://arxiv.org/abs/2506.08700)

  _Ruiran Su, Jiasheng Si, Zhijiang Guo, Janet B. Pierrehumbert_. June 2025. <img src='https://img.shields.io/badge/EMNLP-2025-green'>
  <a href='https://github.com/Albasu120491/ClimateViz'><img src='https://img.shields.io/badge/code-blue'></a>






