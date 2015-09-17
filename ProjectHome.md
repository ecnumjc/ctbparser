# 简介 #

ctbparser是一个用C++语言实现的开源的中文处理工具包（GBK编码），用于分词、词性标注、依存句法分析，采用的是[中文宾州树库(Chinese Tree Bank, CTB)](http://www.cis.upenn.edu/~chinese/ctb.html)标准。

# 优点 #

  1. 用户可以自行编辑词条以改善分词，词性标注效果。
  1. 可以处理繁体中文。
  1. 分词、词性标注、句法分析采用[条件随机场模型](http://en.wikipedia.org/wiki/Conditional_random_field)，而非传统的HHMM模型。该模型具有较好的新词识别能力。

# 评测 #

操作系统：64位CentOS 5，CPU: Intel(R) Xeon(R) E5405, 2.00GHz

测试语料：CTB6标准测试集

内存占用：270M

速度：30句/秒

分词F-score：95.3%

词性标注精度：94.27%

句法分析精度(LAS)：81%

# 参考文献 #

Mark A. Paskin, "Cubic-time Parsing and Learning Algorithms for Grammatical Bigram Models", technique report, 2001

Xian Qian, Qi Zhang, Xuangjing Huang and Lide Wu. "2D Trie for fast parsing", COLING 2010