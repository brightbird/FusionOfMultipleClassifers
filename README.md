# 摘要
近年来，随着O2O的迅速发展，外卖领域产生了大量的文本评论。在大数据时代，这些包含用户主观情感倾向的文本蕴含着大量有用的信息，人工分析长篇文本的情感倾向效率极低，所以，利用计算机对文本进行情感分析具有巨大的应用价值。本文针对外卖领域文本评论，分析了基于词典、k-近邻、朴素贝叶斯、最大熵模型、支持向量机的情感极性分析算法。在基于词典的情感分析算法上，本文构建了一个外卖领域的情感词典。在基于k-近邻算法上，本文提出了Multiple-K的新型决策机制，有效消除K值大小对分类结果的影响。在情感分析算法上，本文采用多分类器融合的投票机制，来决定单个句子的情感极性。实验结果表明，这种方法是有效，准确率能提升3到4个百分点。

# 关键词
多分类器融合；情感分析；K-近邻；贝叶斯；最大熵；支持向量机；情感词典

# 引言
文本信息可大致分为两类：事实和观点。事实是关于实体、事件及实体与事件的属性的客观表达描述。情感是对事物的积极或消极的情绪表达。随着互联网的飞速发展，特别是微博、微信、论坛等的兴起，人们越来越多地通过网络发表自己的评论看法。在大数据时代，这些包含用户主观情感倾向的文本蕴含着大量有用的信息，人工分析长篇文本的情感倾向效率极低，所以，利用计算机对文本进行情感分析具有巨大的应用价值。 

情感分析的研究已比较成熟，在粒度上，情感分析可以有三种划分：词语粒度、句子粒度和篇章粒度。 而每个粒度下，又有其相应的子任务。 

篇章粒度。篇章粒度上的情感分析主要考虑整个篇章的情感极性。Lee et al. 将传统机器学习方法应用于电影评论的情感分析，最后得到从篇章中提取出unigrams后SVM的分类效果最好。 这三种机器学习方法都是有监督的方法。而Peter D. Turney提出了一种无监督的方法进行篇章情感极性的自动分类。 篇章粒度有几个子任务，都有相应的研究尝试解决。比如，主客观分类 、review helpfulness 、垃圾观点侦测 。

句子粒度。句子粒度的情感分析首先是判断句子是否主观或客观，然后将主观语句进行极性分类。Weibe et al. 提出主观性分析在句子中的有效性及其在自然语言处理的应用。 熊德兰等人提出了基于HowNet的语义距离和语法距离相结合的句子褒贬倾向性计算方法利用夹角余弦法对语义倾向进行了改进。 句子粒度的子任务有：观点检索 、观点问答 、观点摘要 。

词语粒度。词语粒度的情感分析主要是提取出评价对象，评价观点，实体，属性，特征及其情感倾向。   

本文尝试对外卖领域的文本，进行句子粒度的情感分析。构建了适应外卖领域的情感词典，并提出K-NN、Naïve Bayes、MaxEnt、SVM的多分类器融合和规则辅助的情感分析方法。

[more...](/paper/多分类器融合的情感分析方法研究.docx)