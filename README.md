# Awesome Multivector Retrieval
[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

An extensive and commented list of resources on late-interaction multivector retrieval.

## Contents
- [Awesome Multivector Retrieval](#awesome-multivector-retrieval)
	- [Contents](#contents)
	- [Models](#models)
		- [Foundational Models](#foundational-models)
		- [Compression \& Token Pruning](#compression--token-pruning)
		- [Multimodal \& Vision](#multimodal--vision)
		- [General Models \& Training](#general-models--training)
	- [Retrieval](#retrieval)
		- [Indexing \& Search Algorithms](#indexing--search-algorithms)
		- [Scoring Kernels](#scoring-kernels)
	- [Software Libraries](#software-libraries)
		- [Training \& Inference Frameworks](#training--inference-frameworks)
		- [Retrieval Engines \& Indexes](#retrieval-engines--indexes)
		- [Scoring Kernels](#scoring-kernels-1)
	- [Model Checkpoints](#model-checkpoints)
		- [General-Purpose](#general-purpose)
		- [Specialized / Domain](#specialized--domain)
	- [Datasets and Encodings](#datasets-and-encodings)
	  - [`MS MARCO v1`](#ms-marco-v1)
	  - [`LoTTE-pooled`](#lotte-pooled)
	- [Multimedia Resources](#multimedia-resources)

## Models

### Foundational Models

- *ColBERT: Efficient and Effective Passage Search via Contextualized Late Interaction over BERT*<br>
	Omar Khattab, Matei Zaharia<br>
	SIGIR, 2020<br>
	📄 [paper](https://doi.org/10.1145/3397271.3401075) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

- *COIL: Revisit Exact Lexical Match in Information Retrieval with Contextualized Inverted List*<br>
	Luyu Gao, Zhuyun Dai, Jamie Callan<br>
	NAACL, 2021<br>
	📄 [paper](https://doi.org/10.18653/v1/2021.naacl-main.241)

- *ColBERTv2: Effective and Efficient Retrieval via Lightweight Late Interaction*<br>
	Keshav Santhanam, Omar Khattab, Jon Saad-Falcon, Christopher Potts, Matei Zaharia<br>
	NAACL, 2022<br>
	📄 [paper](https://doi.org/10.18653/v1/2022.naacl-main.272) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

### Compression & Token Pruning

- *Introducing Neural Bag of Whole-Words with ColBERTer: Contextualized Late Interactions using Enhanced Reduction*<br>
	Sebastian Hofstatter, Omar Khattab, Sophia Althammer, Mete Sertkan, Allan Hanbury<br>
	CIKM, 2022<br>
	📄 [paper](https://doi.org/10.1145/3511808.3557367) | 🛠️ [code](https://github.com/sebastian-hofstaetter/colberter)

- *Joint Optimization of Multi-Vector Representation with Product Quantization*<br>
	Yufan Fang, Jing Zhan, Yiqun Liu, Jiafeng Mao, Min Zhang, Shaoping Ma<br>
	NLPCC, 2022<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-17120-8_49)

- *CITADEL: Conditional Token Interaction via Dynamic Lexical Routing for Efficient and Effective Multi-Vector Retrieval*<br>
	Minghan Li, Sean C. Lin, Barlas Oguz, Arnab Ghoshal, Jimmy Lin, Yashar Mehdad, Wen-tau Yih, Xilun Chen<br>
	ACL, 2023<br>
	📄 [paper](https://doi.org/10.18653/v1/2023.acl-long.663)

- *Rethinking the Role of Token Retrieval in Multi-Vector Retrieval*<br>
	Jinhyuk Lee, Zhuyun Dai, Sai Meher Karthik Duddu, Tao Lei, Iftekhar Naim, Ming-Wei Chang, Vincent Y. Zhao<br>
	NeurIPS, 2023<br>
	📄 [paper](https://dl.acm.org/doi/10.5555/3666122.3666799)

- *SLIM: Sparsified Late Interaction for Multi-Vector Retrieval with Inverted Indexes*<br>
	Minghan Li, Sheng-Chieh Lin, Xueguang Ma, Jimmy Lin<br>
	SIGIR, 2023<br>
	📄 [paper](https://doi.org/10.1145/3539618.3591977)

- *SPLATE: Sparse Late Interaction Retrieval*<br>
	Thibault Formal, Stephane Clinchant, Herve Dejean, Carlos Lassance<br>
	SIGIR, 2024<br>
	📄 [paper](https://doi.org/10.1145/3626772.3657968)

- *Muvera: Multi-Vector Retrieval via Fixed Dimensional Encodings*<br>
	Laxman Dhulipala, Majid Hadian, Rajesh Jayaram, Jason Lee, Vahab Mirrokni<br>
	NeurIPS, 2024<br>
	📄 [paper](https://doi.org/10.52202/079017-3204)

- *Enhancing ColBERT: A Method for Reducing Space Complexity and Accelerating Retrieval Speed*<br>
	Hai Nguyen T., Huong Le T.<br>
	PACLIC, 2024<br>
	📄 [paper](https://aclanthology.org/2024.paclic-1.79/)

- *CRISP: Clustering Multi-Vector Representations for Denoising and Pruning*<br>
	João Veneroso, Rajesh Jayaram, Jinmeng Rao, Gustavo Hernández Ábrego, Majid Hadian, Daniel Cer<br>
	arXiv, 2025<br>
	📄 [paper](https://arxiv.org/abs/2505.11471)

- *Token Pruning Optimization for Efficient Multi-vector Dense Retrieval*<br>
	Shanxiu He, Mutasem Al-Darabsah, Suraj Nair, Jonathan May, Tarun Agarwal, Tao Yang, Choon Hui Teo<br>
	ECIR, 2025<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-88708-6_7)

- *Towards Lossless Token Pruning in Late-Interaction Retrieval Models*<br>
	Yuxuan Zong, Benjamin Piwowarski<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3730100)

- *Sculpting the Vector Space: Towards Efficient Multi-Vector Visual Document Retrieval via Prune-then-Merge Framework*<br>
	Yibo Yan, Mingdong Ou, Yi Cao, Xin Zou, Jiahao Huo, Shuliang Liu, James Kwok, Xuming Hu<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2602.19549)

- *Multi-Vector Index Compression in Any Modality*<br>
	Hanxiang Qin, Alexander Martin, Rohan Jha, Chunsheng Zuo, Reno Kriz, Benjamin Van Durme<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2602.21202) | 🛠️ [code](https://github.com/hanxiangqin/omni-col-press)

### Multimodal & Vision

- *ColPali: Efficient Document Retrieval with Vision Language Models*<br>
	Manuel Faysse, Hugues Sibille, Tony Wu, Bilel Omrani, Gautier Viaud, Celine Hudelot, Pierre Colombo<br>
	ICLR, 2025<br>
	📄 [paper](https://doi.org/10.48550/arXiv.2407.01449)

- *Video-ColBERT: Contextualized Late Interaction for Text-to-Video Retrieval*<br>
	Arun V. Reddy, Alexander Martin, Eugene Yang, Andrew Yates, Kate Sanders, Kenton Murray, Reno Kriz, Celso M. de Melo, Benjamin Van Durme, Rama Chellappa<br>
	CVPR, 2025<br>
	📄 [paper](https://doi.org/10.48550/arXiv.2503.19009)

- *ColMate: Contrastive Late Interaction and Masked Text for Multimodal Document Retrieval*<br>
	Ahmed Masry, Megh Thakkar, Patrice Bechard, Sathwik Tejaswi Madhusudhan, Rabiul Awal, Shambhavi Mishra, Akshay Kalkunte Suresh, Srivatsava Daruru, Enamul Hoque, Spandana Gella, Torsten Scholak, Sai Rajeswar<br>
	EMNLP, 2025<br>
	📄 [paper](https://doi.org/10.18653/v1/2025.emnlp-industry.145)

### General Models & Training

- *PyLate: Flexible Training and Retrieval for Late Interaction Models*<br>
	Antoine Chaffin, Raphaël Sourty<br>
	CIKM, 2025<br>
	📄 [paper](https://doi.org/10.1145/3746252.3761608) | 🛠️ [code](https://github.com/lightonai/pylate)

- *ColBERT-Zero: To Pre-train Or Not To Pre-train ColBERT models*<br>
	Antoine Chaffin, Luca Arnaboldi, Amélie Chatelain, Florent Krzakala<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2602.16609)

- *Your Embedding Model is SMARTer Than You Think*<br>
	Jianrui Zhang, Hyun Jung Lee, Sukanta Ganguly, Tae-Eui Kam, Donghyun Kim, Yong Jae Lee<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2605.24938) | 🛠️ [code](https://github.com/HanSolo9682/SMART)

## Retrieval

### Indexing & Search Algorithms

- *Baleen: Robust Multi-Hop Reasoning at Scale via Condensed Retrieval*<br>
	Omar Khattab, Christopher Potts, Matei Zaharia<br>
	NeurIPS, 2021<br>
	📄 [paper](https://proceedings.neurips.cc/paper/2021/hash/e8b1cbd05f6e6a358a81dee52493dd06-Abstract.html)

- *PLAID: An Efficient Engine for Late Interaction Retrieval*<br>
	Keshav Santhanam, Omar Khattab, Christopher Potts, Matei Zaharia<br>
	CIKM, 2022<br>
	📄 [paper](https://doi.org/10.1145/3511808.3557325) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

- *DESSERT: An Efficient Algorithm for Vector Set Search with Vector Set Queries*<br>
	Joshua Engels, Benjamin Coleman, Vihan Lakshman, Anshumali Shrivastava<br>
	NeurIPS, 2023<br>
	📄 [paper](https://dl.acm.org/doi/10.5555/3666122.3669096)

- *Efficient Multi-Vector Dense Retrieval with Bit Vectors*<br>
	Franco Maria Nardini, Cosimo Rulli, Rossano Venturini<br>
	ECIR, 2024<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-56060-6_1) | 🛠️ [code](https://github.com/CosimoRulli/emvb)

- *A Reproducibility Study of PLAID*<br>
	Sean MacAvaney, Nicola Tonellotto<br>
	SIGIR, 2024<br>
	📄 [paper](https://doi.org/10.1145/3626772.3657856)

- *IGP: Efficient Multi-Vector Retrieval via Proximity Graph Index*<br>
	Ziyang Bian, Man Lung Yiu, Buzhou Tang<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3730004) | 🛠️ [code](https://github.com/DBGroup-SUSTech/multi-vector-retrieval)

- *WARP: An Efficient Engine for Multi-Vector Retrieval*<br>
	Joel L. Scheerer, Matei Zaharia, Christopher Potts, Gustavo Alonso, Omar Khattab<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3729904) | 🛠️ [code](https://github.com/jlscheerer/xtr-warp)

- *Efficient Constant-Space Multi-vector Retrieval*<br>
	Sean MacAvaney, Antonio Mallia, Nicola Tonellotto<br>
	ECIR, 2025<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-88714-7_22)

- *Multivector Reranking in the Era of Strong First-Stage Retrievers*<br>
	Silvio Martinico, Franco Maria Nardini, Cosimo Rulli, Rossano Venturini<br>
	ECIR, 2026<br>
	📄 [paper](https://doi.org/10.1007/978-3-032-21324-2_4) | 🛠️ [code](https://github.com/TusKANNy/papers_reproducibility/tree/main/ecir2026) | 🛠️ [code](https://github.com/TusKANNy/kannolo)

- *Efficient Multivector Retrieval with Token-Aware Clustering and Hierarchical Indexing*<br>
	Silvio Martinico, Franco Maria Nardini, Cosimo Rulli, Rossano Venturini<br>
	SIGIR, 2026<br>
	📄 [paper](https://arxiv.org/abs/2604.28142) | 🛠️ [code](https://github.com/TusKANNy/tachiom)

- *No More K-means: Single-Stage Sparse Coding for Efficient Multi-Vector Retrieval*<br>
	Lixuan Guo, Yifei Wang, Tiansheng Wen, Aosong Feng, Stefanie Jegelka, Chenyu You<br>
	ICML, 2026<br>
	📄 [paper](https://arxiv.org/abs/2605.30120)

- *SMVE: Sparse Multi-Vector Retrieval*<br>
	Martin Spisak, Marek Galovic<br>
	ECIR, 2026<br>
	📄 [blog](https://www.topk.io/blog/20260311-smve-multi-vector-retrieval)

- *ColBERTSaR: Sparsified ColBERT Index via Product Quantization*<br>
	Eugene Yang, Andrew Yates, Dawn Lawrie, James Mayfield, Saron Samuel, Rohan Jha<br>
	SIGIR, 2026<br>
	📄 [paper](https://arxiv.org/abs/2606.05568) | 🛠️ [code](https://github.com/hltcoe/ColBERTSaR)

### Scoring Kernels

- *FLASH-MAXSIM: IO-Aware Fused Kernels for Late-Interaction Scoring*<br>
	Roi Pony, Adi Raz Goldfarb, Idan Friedman, Daniel Ezer, Udi Barzelay<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2605.29517) | 🛠️ [code](https://github.com/roipony/flash-maxsim)

## Software Libraries

### Training & Inference Frameworks

- [ColBERT](https://github.com/stanford-futuredata/ColBERT) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Reference implementation for ColBERT and ColBERTv2, and includes PLAID support for efficient late-interaction retrieval.*

- [RAGatouille](https://github.com/AnswerDotAI/RAGatouille) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Python toolkit to train and serve ColBERT-based late-interaction retrievers.*

- [PyLate](https://github.com/lightonai/pylate) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Python library for training, fine-tuning, inference, and retrieval with ColBERT-style late-interaction models on single and multi-GPU setups.*

- [PyLate-rs](https://github.com/lightonai/pylate-rs) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*High-performance Rust inference engine for PyLate models, with Python bindings and optimized integration with FastPlaid for retrieval pipelines.*

### Retrieval Engines & Indexes

- [FastPlaid](https://github.com/lightonai/fast-plaid) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*GPU-optimized engine for ColBERT/PLAID-style late-interaction retrieval.*

- [kANNolo](https://github.com/TusKANNy/kannolo) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*ANN library for dense, sparse, and multivector retrieval.*

- [Vectorium](https://github.com/TusKANNy/vectorium) <img src="images/rust-logo.png" height="22" alt="Rust"/><br>
	*Rust library for compact storage/access of dense, sparse, and multivector embeddings.*

- [Firn](https://github.com/gordonmurray/firnflow) <img src="images/rust-logo.png" height="22" alt="Rust"/><br>
	*Rust search engine for single-vector and late-interaction multivector namespaces, backed by LanceDB on object storage with RAM/NVMe result caching.*

- [NextPlaid](https://github.com/lightonai/next-plaid) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*CPU-oriented local-first multivector retrieval engine with memory-mapped storage.*

- [EMVB](https://github.com/CosimoRulli/emvb) <img src="images/cpp-logo.svg" height="20" alt="C++"/><br>
	*Reference implementation for Efficient Multi-Vector Dense Retrieval with Bit Vectors.*

- [IGP](https://github.com/DBGroup-SUSTech/multi-vector-retrieval) <img src="images/cpp-logo.svg" height="20" alt="C++"/><br>
	*Official C++ implementation for IGP: proximity-graph indexing for multi-vector retrieval (with Python scripts for experiments).*

- [WARP](https://github.com/jlscheerer/xtr-warp) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Official implementation for WARP, an efficient multi-vector retrieval engine.*

- [ColGrep](https://github.com/lightonai/next-plaid/tree/main/colgrep) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*High-performance code search CLI tool powered by LateOn-Code and NextPlaid, enabling semantic + hybrid (regex + semantic) code retrieval locally with incremental indexing.*

- [TACHIOM](https://github.com/TusKANNy/tachiom) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Fast and scalable multivector retrieval system with Token-Aware Clustering (TAC) and hierarchical Product Quantization for efficient late-interaction search.*

- [TopK](https://github.com/topk-io/topk) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Managed retrieval engine with support for late-interaction search over billions of documents, online index updates, filtering, and more.*

### Scoring Kernels

- [Flash-MaxSim](https://github.com/roipony/flash-maxsim) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*IO-aware Triton kernel for MaxSim scoring in ColBERT/ColPali pipelines: tile-by-tile on-chip computation with zero intermediate memory and INT8 quantization support.*

- [maxsim](https://github.com/ErikKaum/maxsim) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Ahead-of-time compiled MaxSim kernel with CUDA and Metal backends (NVIDIA + Apple Silicon), distributed as a HuggingFace kernels package.*

- [late-interaction-kernels](https://github.com/hcompai/late-interaction-kernels) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*Fused Triton kernels for MaxSim scoring with CUDA, Metal, and CPU backends, native PyLate/colpali-engine integration, and PLAID-style compressed-index support.*

- [maxsim-cpu](https://github.com/mixedbread-ai/maxsim-cpu) <img src="images/rust-logo.png" height="22" alt="Rust"/> <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*CPU-only MaxSim kernel written in Rust (libxsmm on x86, Apple Accelerate on ARM) with Python bindings.*

## Model Checkpoints

### General-Purpose

- [colbert-ir/colbertv2.0](https://huggingface.co/colbert-ir/colbertv2.0)<br>
	*Official ColBERTv2 checkpoint (MS MARCO-trained) from the ColBERT authors, widely used as the canonical baseline model.*

- [lightonai/LateOn](https://huggingface.co/lightonai/LateOn)<br>
	*State-of-the-art ColBERT model (149M, ModernBERT-based) achieving 57.22 NDCG@10 on BEIR with fully open training data and strong generalization under decontamination.*

- [ColBERT-Zero](https://huggingface.co/lightonai/ColBERT-Zero)<br>
	*Large-scale fully pre-trained ColBERT checkpoint trained on public data and released with the ColBERT-Zero paper.*

- [GTE-ModernColBERT-v1](https://huggingface.co/lightonai/GTE-ModernColBERT-v1)<br>
	*PyLate late-interaction checkpoint based on ModernBERT with 128-dimensional token embeddings and strong long-context retrieval behavior.*

- [Iso-ModernColBERT](https://huggingface.co/topk-io/Iso-ModernColBERT)<br>
	*Isotropically corrected version of GTE-ModernColBERT-v1 built for efficient inference and scalable retrieval.*

- [colberter-128-32-msmarco](https://huggingface.co/sebastian-hofstaetter/colberter-128-32-msmarco) / [uni-colberter-128-1-msmarco](https://huggingface.co/sebastian-hofstaetter/uni-colberter-128-1-msmarco)<br>
	*ColBERTer checkpoints trained on MS MARCO (128-dim, with 32 and 1 unique whole-word vectors per document respectively).*

### Specialized / Domain

- [lightonai/LateOn-Code](https://huggingface.co/lightonai/LateOn-Code)<br>
	*Specialized ColBERT model (149M parameters) fine-tuned for code retrieval, achieving SOTA on MTEB Code benchmark.*

- [lightonai/LateOn-Code-edge](https://huggingface.co/lightonai/LateOn-Code-edge)<br>
	*Lightweight code retrieval model (17M parameters) for edge devices, matching larger models while running efficiently on CPU.*

- [Reason-ModernColBERT](https://huggingface.co/lightonai/Reason-ModernColBERT)<br>
	*Reasoning-focused late-interaction checkpoint fine-tuned on reasonir-hq, with strong BRIGHT benchmark performance for reasoning-intensive retrieval.*

## Datasets and Encodings

### `MS MARCO v1`
- **Documents**: `8,841,823`
- **Queries** [`dev.small`]: `6,980`
- **Reference Metric**: `MRR@10`

| Encoding | Link | Vector dim | Avg vectors per doc | Avg vectors per query | MRR@10 |
|---|---|---:|---:|---:|---:|
| `colbertv2` | [link](https://huggingface.co/datasets/tuskanny/ms_marco_colbertv2/tree/main) | 128 | 67 | 32 | 0.397 |


### `LoTTE-pooled`
- **Documents**: `2,428,854`
- **Queries** [`dev/search`]: `2,931`
- **Reference Metric**: `Success@5`

| Encoding | Link | Vector dim | Avg vectors per doc | Avg vectors per query  | Success@5 |
|---|---|---:|---:|---:|---:|
| `colbertv2` | [link](https://huggingface.co/datasets/tuskanny/lotte_pooled_colbertv2/tree/main) | 128 | 109 | 32 | `N/A` |


## Multimedia Resources

- Omar Khattab on Late Interaction in 2030. [Link](https://www.youtube.com/watch?v=Z2TmdcylyEc)
- Multi-Vector Search with Amélie Chatelain and Antoine Chaffin - Weaviate Podcast #134. [Link](https://www.youtube.com/watch?v=44GC3E-WbHU)
