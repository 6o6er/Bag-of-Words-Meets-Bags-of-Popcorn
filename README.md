# Bag-of-Words-Meets-Bags-of-Popcorn
kaggle上的情感分析，自己并不会自然语言处理，照着别人的写的，一边抄一边理解。。Orz

记录一下自己的学习过程：

刚拿到题目的时候完全没思路，之前还从未处理过自然语言处理的东西。在网上查了下需要的技术，很多博客提到了TF-IDF和Word2Vec、Doc2Vec.
	
TF-IDF之前了解过，他的方法也比较简单，具体的思路和吴军老师的《数学之美》当中介绍的例子很相似。就是评估每个词语的重要程度。介绍“原子能应用”这个词语的时候提到的。有兴趣的可以去查查

根据我查到的资料，直接用TF-IDF处理这个题的语料库，然后在做各种基础模型（LR\贝叶斯等）效果其实也很好，但听说Word2Vec是更晚出来的技术。于是打算直接学Word2Vec

Word2Vec的理论其实不复杂。他相当于是把n元模型优化成了神经网络模型。中间的隐藏层有多少神经元，最后的词向量就是多少维的。但是至今没看懂的是用哈夫曼进行的优化加速。

学习（抄）的源码来自：https://github.com/tjflexic/kaggle-word2vec-movie-reviews

题目链接：https://www.kaggle.com/c/word2vec-nlp-tutorial/data

目前代码并没写完。暂时有工作上的事，先上传一部分。