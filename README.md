# SWUFE-GeoText

* [背景知识](#background)
  * 时空轨迹数据概述
  * 常见时空轨迹数据
  * 时空轨迹数据的表示与定义
* 时空轨迹语义理解学习框架
  * 深度序列学习
  * 概率深度学习
  * 时空图学习
  * 基于底座模型的学习
* 时空轨迹语义理解核心任务
  * 时空要素表示学习
  * 基于时空语义理解的轨迹相似学习
    * 轨迹聚类
    * 轨迹分类
    * 轨迹连接
    * 异常轨迹识别
  * 基于时空语义理解的轨迹预测学习
    * 人群移动性预测
    * 城市感知预测
    * 时空数据补全
  * 时空知识图谱
* 生成式智能时代的挑战与机遇
  * 面向时空语义理解的高质量数据合成及集成研究
  * 全量式时空语义理解大模型训练机制研究
  * 多模态在时空轨迹应用
  * 时空大模型赋能实际应用

<h2 id="background">背景知识</h2> 
<h3 id="word_based_models">时空轨迹数据概述</h3>

* Alam M M, Torgo L, Bifet A. 2022. [A survey on spatio-temporal data analytics systems](https://dl.acm.org/doi/abs/10.1145/3507904). *ACM Computing Surveys*. ([citation]():54(10s): 1-38)
* Erwig, Martin, et al. 1999. [Spatio-temporal data types: An approach to modeling and querying moving objects in databases](https://link.springer.com/article/10.1023/A:1009805532638). *GeoInformatica*.  ([citation]: 3.3: 269-296)
* Pelekis, Nikos, et al. 2004. [Literature review of spatio-temporal database models](https://www.cambridge.org/core/journals/knowledge-engineering-review/article/abs/literature-review-of-spatiotemporal-database-models/38175D21635346C9002C3C2DEDF9232D). *The Knowledge Engineering Review*. ([citation]: 19.3 (2004): 235-274)
* Zhang, Junbo, et al. 2016. [DNN-based prediction model for spatio-temporal data](https://dl.acm.org/doi/abs/10.1145/2996913.2997016). *Proceedings of the 24th ACM SIGSPATIAL international conference on advances in geographic information systems*.

<h3 id="word_based_models">常见时空轨迹数据</h3>

* Atluri, Gowtham, Anuj Karpatne, and Vipin Kumar. 2018. [Spatio-temporal data mining: A survey of problems and methods](https://dl.acm.org/doi/abs/10.1145/3161602). *ACM Computing Surveys (CSUR)*. ([citation]: 51.4 (2018): 1-41)
* Evans, Michael R., et al. 2019. [Enabling spatial big data via CyberGIS: Challenges and opportunities](https://link.springer.com/chapter/10.1007/978-94-024-1531-5_8). *CyberGIS for geospatial discovery and innovation*. ([citation]: (2019): 143-170)

<h2 id="background">时空轨迹语义理解学习框架</h2> 

* Chen W, Liang Y, Zhu Y, et al. 2024. [Deep Learning for Trajectory Data Management and Mining: A Survey and Beyond](https://arxiv.org/abs/2403.14151). *arXiv preprint*. ([citation]: arXiv:2403.14151)

<h3 id="word_based_models">深度序列学习</h3>

* Chen X, Duan Y, Houthooft R, et al. 2016. [Infogan: Interpretable representation learning by information maximizing generative adversarial nets](https://proceedings.neurips.cc/paper_files/paper/2016/hash/7c9d0b1f96aebd7b5eca8c3edaa19ebb-Abstract.html). *Advances in neural information processing systems*. ([citation]: 29)
* Radford A, Metz L, Chintala S. 2015. [Unsupervised representation learning with deep convolutional generative adversarial networks](https://arxiv.org/abs/1511.06434). *arXiv preprint*. ([citation]: arXiv:1511.06434)
* Martin Arjovsky, Soumith Chintala, Léon Bottou. 2017. [Wasserstein GAN](https://arxiv.org/abs/1701.07875). *arXiv preprint*. ([citation]: arXiv:1701.07875 [stat.ML])
* Li C, Xu T, Zhu J, et al. 2017. [Triple generative adversarial nets](https://proceedings.neurips.cc/paper/2017/hash/86e78499eeb33fb9cac16b7555b50767-Abstract.html). *Advances in neural information processing systems*. ([citation]: 30)

<h3 id="word_based_models">概率深度学习</h3>

* Kingma D P, Welling M. 2013. [Auto-encoding variational bayes](https://arxiv.org/abs/1312.6114). *arXiv preprint*. ([citation]: arXiv:1312.6114)
* Ramchandran S, Tikhonov G, Lönnroth O, et al. 2024. [Learning conditional variational autoencoders with missing covariates](https://www.sciencedirect.com/science/article/pii/S0031320323008105). *Pattern Recognition*. ([citation] 147: 110113)
* FactorVAE
* β-VAE
* Sohl-Dickstein J, Weiss E, Maheswaranathan N, et al. 2015. [Deep unsupervised learning using nonequilibrium thermodynamics](https://proceedings.mlr.press/v37/sohl-dickstein15.html). *International conference on machine learning*. ([citation]: PMLR, 2015: 2256-2265)
* Ho J, Jain A, Abbeel P. 2020. [Denoising diffusion probabilistic models](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html). *Advances in neural information processing systems*. ([citation]: 2020, 33: 6840-6851)
* Song Y, Sohl-Dickstein J, Kingma D P, et al. 2020. [Score-based generative modeling through stochastic differential equations](https://arxiv.org/abs/2011.13456). *arXiv preprint*. ([citation]: arXiv:2011.13456)
* Lin L, Li Z, Li R, et al. 2023. [Diffusion models for time-series applications: a survey](https://link.springer.com/article/10.1631/FITEE.2300310). *Frontiers of Information Technology & Electronic Engineering*. ([citation]: 2023: 1-23)
* Lim H, Kim M, Park S, et al. 2023. [Regular time-series generation using sgm](https://arxiv.org/abs/2301.08518). *arXiv preprint*. ([citation]: arXiv:2301.08518, 2023)
* Li Y, Lu X, Wang Y, et al. 2022. [Generative time series forecasting with diffusion, denoise, and disentanglement](). *Advances in Neural Information Processing Systems*. ([citation]: 35: 23009-23022)
* Zhu Y, Yu J J, Zhao X, et al. 2024. [Controltraj: Controllable trajectory generation with topology-constrained diffusion model](https://arxiv.org/abs/2404.15380). *arXiv preprint*. ([citation]:arXiv:2404.15380, 2024)
* Zhu Y, Ye Y, Zhang S, et al. 2024. [Difftraj: Generating gps trajectory with diffusion probabilistic model](https://proceedings.neurips.cc/paper_files/paper/2023/hash/cd9b4a28fb9eebe0430c3312a4898a41-Abstract-Conference.html). Advances in *Neural Information Processing Systems*. ([citation]: 36)
* Wei T, Lin Y, Guo S, et al. 2024. [Diff-RNTraj: A Structure-aware Diffusion Model for Road Network-constrained Trajectory Generation](https://arxiv.org/abs/2402.07369). *arXiv preprint*. ([citation]: arXiv:2402.07369)
* Larsen A B L, Sønderby S K, Larochelle H, et al. 2016. [Autoencoding beyond pixels using a learned similarity metric](https://proceedings.mlr.press/v48/larsen16). *International conference on machine learning*. ([citation]: PMLR, 2016: 1558-1566)
* AVB
* Makhzani A, Shlens J, Jaitly N, et al. 2015. [Adversarial autoencoders](https://arxiv.org/abs/1511.05644). *arXiv preprint* ([citation]: arXiv:1511.05644)





















