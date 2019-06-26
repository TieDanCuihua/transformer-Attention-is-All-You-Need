# transformer-Attention-is-All-You-Need

Google的《Attention is all you need》学习记录与总结。此模型在WMT 2014英语-德语翻译任务上达到28.4 BLEU。
比起学习知识，我认为检索知识才是最耗时间的。找到好的资料，往往能事半功倍。我这里列出了我学习这篇论文时发现的好资料。

源代码参考了https://github.com/Kyubyong/transformer。 代码写的很好，本想自己按照自己的思想修改一下，却发现越修改越糟糕.....
这里有一篇代码的解读，https://blog.csdn.net/u012526436/article/details/86519381， 能帮助大家更好的理解论文、理解原理。
当时我看到了tf.linalg.LinearOperatorLowerTriangular时，一直没想明白干啥用的，后来查到了代码解读，才恍然大悟。

论文地址：https://arxiv.org/pdf/1706.03762.pdf
这里有一篇论文的中文翻译版:https://www.yiyibooks.cn/yiyibooks/Attention_Is_All_You_Need/index.html ， 不过建议读英文原版。

这篇论文的主要思想是放弃Rnn，全程只有attention来解决问题。

RNN，包括LSTM等，在处理一句话时，都是一个字一个字的处理数据。我们每个人刚认字时，也都是一个字一个字的读文章的，但现在，我们高中毕业，大学毕业后，恐怕不会还是一个字一个字的读文章了，不是一目十行，也得一目半行吧，而且大家都知道，在读文章时，很多时候打乱一句话中各个字的顺序，并不会影响人们的理解，
所以，我深刻的怀疑这篇论文的灵感就是来源于人们从小到大读文章的习惯。(纯属自己瞎想)



