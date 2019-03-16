# Sentiment-analysis  
1. 数据处理  
包括标记,合并,分词,去除停用词,去除特殊符号等标准化处理.  
2.训练词向量,生成索引矩阵  
wordVectors为训练的词向量,idsMatrix.npy为生成的单词索引矩阵,把每篇文档转化成数组,每个位置行代表每篇文档,每列代表每个单词,每个元素代表此文档中这个单词在词向量数组中索引位置.  
3.搭建LSTM网络,参数设置  
包括学习率,batch_size,max_sequence,lstm_units等,并按照batch_size大小对训练和测试数据进行处理作为网络输入.  
最终输出的预测结果为对语料的分类,这里为积极消极两种情况,迭代200000后准确率基本达到最高,在测试集中可达到80%以上.  
4.可视化   
训练过程由tensorbord可视化如下图   
https://github.com/dotah88/Sentiment-analysis/blob/master/tensor_image/45cb2c86-2308-4058-8d62-e5a49135eae1.png  

