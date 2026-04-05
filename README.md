# Awesome Multivector Retrieval
[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

An extensive and commented list of resources on late-interaction multivector retrieval.

## Contents
- [Awesome Multivector Retrieval](#awesome-multivector-retrieval)
	- [Contents](#contents)
	- [Models](#models)
	- [Retrieval](#retrieval)
	- [Software Libraries](#software-libraries)

## Models

- *COIL: Revisit Exact Lexical Match in Information Retrieval with Contextualized Inverted List*<br>
	Luyu Gao, Zhuyun Dai, Jamie Callan<br>
	NAACL, 2021<br>
	📄 [paper](https://doi.org/10.18653/v1/2021.naacl-main.241)

- *uniCOIL: A Neural Lexical Model for Passage Retrieval*<br>
	Sean C. Lin, Jheng-Hong Yang, Jimmy Lin<br>
	ACL, 2021<br>
	📄 [paper](https://doi.org/10.18653/v1/2021.acl-short.47)

- *ColBERT: Efficient and Effective Passage Search via Contextualized Late Interaction over BERT*<br>
	Omar Khattab, Matei Zaharia<br>
	SIGIR, 2020<br>
	📄 [paper](https://doi.org/10.1145/3397271.3401075) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

- *ColBERTv2: Effective and Efficient Retrieval via Lightweight Late Interaction*<br>
	Keshav Santhanam, Omar Khattab, Jon Saad-Falcon, Christopher Potts, Matei Zaharia<br>
	NAACL, 2022<br>
	📄 [paper](https://doi.org/10.18653/v1/2022.naacl-main.272) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

- *Introducing Neural Bag of Whole-Words with ColBERTer: Contextualized Late Interactions using Enhanced Reduction*<br>
	Sebastian Hofstatter, Omar Khattab, Sophia Althammer, Mete Sertkan, Allan Hanbury<br>
	CIKM, 2022<br>
	📄 [paper](https://doi.org/10.1145/3511808.3557367)

- *Joint Optimization of Multi-Vector Representation with Product Quantization*<br>
	Yufan Fang, Jing Zhan, Yiqun Liu, Jiafeng Mao, Min Zhang, Shaoping Ma<br>
	NLPCC, 2022<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-17120-8_49)

- *CITADEL: Conditional Token Interaction via Dynamic Lexical Routing for Efficient and Effective Multi-Vector Retrieval*<br>
	Minghan Li, Sean C. Lin, Barlas Oguz, Arnab Ghoshal, Jimmy Lin, Yashar Mehdad, Wen-tau Yih, Xilun Chen<br>
	ACL, 2023<br>
	📄 [paper](https://doi.org/10.18653/v1/2023.acl-long.663)

- *Rethinking the Role of Token Retrieval in Multi-Vector Retrieval*<br>
	Juhee Lee, Zhuyun Dai, Sai Meher Krishna Duddu, Tao Lei, Iftekhar Naim, Ming-Wei Chang, Vincent Y. Zhao<br>
	NeurIPS, 2023<br>
	📄 paper

- *SLIM: Sparsified Late Interaction for Multi-Vector Retrieval with Inverted Indexes*<br>
	Ming Li, Sean C. Lin, Xuchen Ma, Jimmy Lin<br>
	SIGIR, 2023<br>
	📄 [paper](https://doi.org/10.1145/3580305.3599258)

- *SPLATE: Sparse Late Interaction Retrieval*<br>
	Thibault Formal, Stephane Clinchant, Herve Dejean, Carlos Lassance<br>
	SIGIR, 2024<br>
	📄 [paper](https://doi.org/10.1145/3626772.3657968)

- *Muvera: Multi-Vector Retrieval via Fixed Dimensional Encodings*<br>
	Laxman Dhulipala, Mohammad Hadian, Rahul Jayaram, Jae Lee, Vahab Mirrokni<br>
	NeurIPS, 2025<br>
	📄 paper

- *ColPali: Efficient Document Retrieval with Vision Language Models*<br>
	Manuel Faysse, Hugues Sibille, Tony Wu, Bilel Omrani, Gautier Viaud, Celine Hudelot, Pierre Colombo<br>
	ICLR, 2025<br>
	📄 [paper](https://doi.org/10.48550/arXiv.2407.01449)

- *Video-ColBERT: Contextualized Late Interaction for Text-to-Video Retrieval*<br>
	Arun V. Reddy, Alexander Martin, Eugene Yang, Andrew Yates, Kate Sanders, Kenton Murray, Reno Kriz, Celso M. de Melo, Benjamin Van Durme, Rama Chellappa<br>
	CVPR, 2025<br>
	📄 [paper](https://doi.org/10.48550/arXiv.2503.19009)

- *Hypencoder: Hypernetworks for Information Retrieval*<br>
	Julian Killingback, Hansi Zeng, Hamed Zamani<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3729983)

- *ColMate: Contrastive Late Interaction and Masked Text for Multimodal Document Retrieval*<br>
	Ahmed Masry, Megh Thakkar, Patrice Bechard, Sathwik Tejaswi Madhusudhan, Rabiul Awal, Shambhavi Mishra, Serena Do, Shachi Dave, Piyush Khaitan, Livio Baldini Soares<br>
	EMNLP, 2025<br>
	📄 [paper](https://doi.org/10.18653/v1/2025.emnlp-industry.145)

- *SimpleDoc: Multi-Modal Document Understanding with Dual-Cue Page Retrieval and Iterative Refinement*<br>
	Chelsi Jain, Yiran Wu, Yifan Zeng, Jiale Liu, Shengyu Dai, Zhenwen Shao, Qingyun Wu, Huazheng Wang<br>
	EMNLP, 2025<br>
	📄 [paper](https://doi.org/10.18653/v1/2025.emnlp-main.1443)

## Retrieval

- *Baleen: Robust Multi-Hop Reasoning at Scale via Condensed Retrieval*<br>
	Omar Khattab, Christopher Potts, Matei Zaharia<br>
	NeurIPS, 2021<br>
	📄 [paper](https://proceedings.neurips.cc/paper/2021/hash/e8b1cbd05f6e6a358a81dee52493dd06-Abstract.html)

- *PLAID: An Efficient Engine for Late Interaction Retrieval*<br>
	Keshav Santhanam, Omar Khattab, Christopher Potts, Matei Zaharia<br>
	CIKM, 2022<br>
	📄 [paper](https://doi.org/10.1145/3511808.3557325) | 🛠️ [code](https://github.com/stanford-futuredata/ColBERT)

- *DESSERT: An Efficient Algorithm for Vector Set Search with Vector Set Queries*<br>
	Jovan Engels, Benjamin Coleman, Vivek Lakshman, Anshumali Shrivastava<br>
	NeurIPS, 2023<br>
	📄 paper

- *UDAPDR: Unsupervised Domain Adaptation via LLM Prompting and Distillation of Rerankers*<br>
	Jon Saad-Falcon, Omar Khattab, Keshav Santhanam, Radu Florian, Martin Franz, Salim Roukos, Avirup Sil, Md. Arafat Sultan, Christopher Potts<br>
	EMNLP, 2023<br>
	📄 [paper](https://doi.org/10.18653/v1/2023.emnlp-main.693)

- *Efficient Multi-Vector Dense Retrieval with Bit Vectors*<br>
	Franco Maria Nardini, Cosimo Rulli, Rossano Venturini<br>
	ECIR, 2024<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-56060-6_1)

- *A Reproducibility Study of PLAID*<br>
	Sean MacAvaney, Nicola Tonellotto<br>
	SIGIR, 2024<br>
	📄 [paper](https://doi.org/10.1145/3626772.3657856)

- *IGP: Efficient Multi-Vector Retrieval via Proximity Graph Index*<br>
	Ziyang Bian, Man Lung Yiu, Buzhou Tang<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3730004)

- *WARP: An Efficient Engine for Multi-Vector Retrieval*<br>
	Joel L. Scheerer, Matei Zaharia, Christopher Potts, Gustavo Alonso, Omar Khattab<br>
	SIGIR, 2025<br>
	📄 [paper](https://doi.org/10.1145/3726302.3729904)

- *Efficient Constant-Space Multi-vector Retrieval*<br>
	Sean MacAvaney, Antonio Mallia, Nicola Tonellotto<br>
	ECIR, 2025<br>
	📄 [paper](https://doi.org/10.1007/978-3-031-88714-7_22)

- *BiMax: Bidirectional MaxSim Score for Document-Level Alignment*<br>
	Xiaotian Wang, Takehito Utsuro, Masaaki Nagata<br>
	EMNLP, 2025<br>
	📄 [paper](https://aclanthology.org/2025.findings-emnlp.704/)

- *LILaC: Late Interacting in Layered Component Graph for Open-domain Multimodal Multihop Retrieval*<br>
	Joohyung Yun, Doyup Lee, Wook-Shin Han<br>
	EMNLP, 2025<br>
	📄 [paper](https://doi.org/10.18653/v1/2025.emnlp-main.1037)

- *Multivector Reranking in the Era of Strong First-Stage Retrievers*<br>
	Silvio Martinico, Franco Maria Nardini, Cosimo Rulli, Rossano Venturini<br>
	arXiv, 2026<br>
	📄 [paper](https://arxiv.org/abs/2601.05200)

## Software Libraries

- [ColBERT](https://github.com/stanford-futuredata/ColBERT) <br>
	*Reference implementation for ColBERT and ColBERTv2 late-interaction multivector retrieval.*

- [RAGatouille](https://github.com/AnswerDotAI/RAGatouille) <br>
	*Python toolkit to train and serve ColBERT-based late-interaction retrievers.*

- [PyLate](https://github.com/lightonai/pylate) <br>
	*Library for late-interaction retrieval pipelines and efficient multivector search integration.*

- [kANNolo](https://github.com/TusKANNy/kannolo) <br>
	*Rust and Python library for approximate nearest-neighbor search over dense, sparse, and multivector embeddings.*

- [Vectorium](https://github.com/TusKANNy/vectorium) <br>
	*Embedding storage and compression backbone for dense, sparse, and multivector retrieval workloads.*

- [FastPlaid](https://github.com/lightonai/fast-plaid) <br>
	*High-performance engine for ColBERT-style late-interaction retrieval.*

- [NextPlaid](https://github.com/lightonai/next-plaid) <br>
	*Local-first, memory-mapped multivector retrieval database with API support.*

- [Mixpeek](https://mixpeek.com/) <br>
	*Production infrastructure tailored for multimodal late-interaction retrieval systems.*

- [Vespa](https://vespa.ai/) <br>
	*Production search engine with support for token-level interaction ranking and vector retrieval pipelines.*

- [Qdrant](https://qdrant.tech/) <br>
	*Vector database that supports multivector representations and hybrid retrieval deployments.*

- [Weaviate](https://weaviate.io/) <br>
	*Vector search engine for dense and hybrid retrieval, often used as infrastructure for late-interaction stacks.*

- [Milvus](https://milvus.io/) <br>
	*Vector database with support for advanced similarity operators used in late-interaction retrieval pipelines.*

- [OpenSearch](https://opensearch.org/) <br>
	*Open-source search engine with vector and hybrid retrieval support, including late-interaction reranking pipelines.*

