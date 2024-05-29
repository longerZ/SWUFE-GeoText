# SWUFE-GeoText

* [背景知识](# 背景知识)
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

<h2 id="10_must_reads">背景知识</h2> 
<h3 id="word_based_models">时空轨迹数据概述</h3>

* Alam M M, Torgo L, Bifet A. 2022. [A survey on spatio-temporal data analytics systems](https://dl.acm.org/doi/abs/10.1145/3507904). *ACM Computing Surveys*. ([citation]():54(10s): 1-38.)

* Peter E. Brown, Stephen A. Della Pietra, Vincent J. Della Pietra, and Robert L. Mercer. 1993. [The Mathematics of Statistical Machine Translation: Parameter Estimation](http://aclweb.org/anthology/J93-2003). *Computational Linguistics*. ([Citation](https://scholar.google.com/scholar?cites=2259057253133260714&as_sdt=2005&sciodt=0,5&hl=en): 5,218)
* Kishore Papineni, Salim Roukos, Todd Ward, and Wei-Jing Zhu. 2002. [BLEU: a Method for Automatic Evaluation of Machine Translation](http://aclweb.org/anthology/P02-1040). In *Proceedings of ACL 2002*. ([Citation](https://scholar.google.com/scholar?cites=9019091454858686906&as_sdt=2005&sciodt=0,5&hl=en): 10,700)
* Philipp Koehn, Franz J. Och, and Daniel Marcu. 2003. [Statistical Phrase-Based Translation](http://aclweb.org/anthology/N03-1017). In *Proceedings of NAACL 2003*. ([Citation](https://scholar.google.com/scholar?cites=11796378766060939113&as_sdt=2005&sciodt=0,5&hl=en): 3,713)
* Franz Josef Och. 2003. [Minimum Error Rate Training in Statistical Machine Translation](http://aclweb.org/anthology/P03-1021). In *Proceedings of ACL 2003*. ([Citation](https://scholar.google.com/scholar?cites=15358949031331886708&as_sdt=2005&sciodt=0,5&hl=en): 3,115)
* David Chiang. 2007. [Hierarchical Phrase-Based Translation](http://aclweb.org/anthology/J07-2003). *Computational Linguistics*. ([Citation](https://scholar.google.com.hk/scholar?cites=17074501474509484516&as_sdt=2005&sciodt=0,5&hl=en): 1,235)
* Ilya Sutskever, Oriol Vinyals, and Quoc V. Le. 2014. [Sequence to Sequence Learning
with Neural Networks](https://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf). In *Proceedings of NIPS 2014*. ([Citation](https://scholar.google.com/scholar?cites=13133880703797056141&as_sdt=2005&sciodt=0,5&hl=en): 9,432)
* Dzmitry Bahdanau, Kyunghyun Cho, and Yoshua Bengio. 2015. [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/pdf/1409.0473.pdf). In *Proceedings of ICLR 2015*. ([Citation](https://scholar.google.com/scholar?cites=9430221802571417838&as_sdt=2005&sciodt=0,5&hl=en): 10,479)
* Diederik P. Kingma, Jimmy Ba. 2015. [Adam: A Method for Stochastic Optimization](https://arxiv.org/pdf/1412.6980). In *Proceedings of ICLR 2015*. ([Citation](https://scholar.google.com/scholar?cites=16194105527543080940&as_sdt=2005&sciodt=0,5&hl=en): 37,480)
* Rico Sennrich, Barry Haddow, and Alexandra Birch. 2016. [Neural Machine Translation of Rare Words with Subword Units](https://arxiv.org/pdf/1508.07909.pdf). In *Proceedings of ACL 2016*. ([Citation](https://scholar.google.com/scholar?cites=1307964014330144942&as_sdt=2005&sciodt=0,5&hl=en): 1,679)
* Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, and Illia Polosukhin. 2017. [Attention is All You Need](https://papers.nips.cc/paper/7181-attention-is-all-you-need.pdf). In *Proceedings of NIPS 2017*. ([Citation](https://scholar.google.com/scholar?cites=2960712678066186980&as_sdt=2005&sciodt=0,5&hl=en): 6,112)
