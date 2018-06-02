## 词向量
#### 生成词向量的方式可分为：基于统计的方法和基于语言模型(language model)的方法。    
##### 基于统计方法 ：   
>       共现矩阵 ：通过统计一个事先指定大小的窗口内的word共现次数， 以word周边的共现词的次数做为当前word的vector。具体来说，我
>               们通过从大量的语料文本中构建一个共现矩阵来定义word representation。 	
>       SVD（奇异值分解） ：既然基于co-occurrence矩阵得到的离散词向量存在着高维和稀疏性的问SVD得到了word的稠密（dense）矩阵，
>               该矩阵具有很多良好的性质：语义相近的词在向量空间相近，甚至可以一定程度反映word间的线性关系。 
##### 语言模型(language model) ：
>       CBOW（Continuous Bag-of-Word）：CBOW模型是预测上下文已知的情况下，当前词出现的概率。   