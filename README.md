# -文本相似度流程：
	


主要过程： text ——> 分类 ——> 匹配 -> 结果
分类：
  分类的目的主要是减少计算复杂度，如果知道文本属于哪一类，能大大减少后续匹配的时间。
  数据 -> 预处理 -> 文本表示 -> 分类器
  预处理：需要去掉无用字符，去掉停用词等。
  文本表示：将文本转换为向量形式，包括特征提取等过程。
  分类器： 将处理好的数据输进去，进行分类。模型预定使用谷歌的bert模型，听说这个模型表现最好。

文本匹配：
	文本匹配有2个方向，一个是语义匹配比如中国-北京，欧洲-意大利。另外一个就是字符距离匹配，简单来说类似论文查重。模型将会输出数据库中最相似的文章或者句子。

现任务：
	暂时先采用新闻数据作为测试数据库，进行文本分类模型建立。
数据来源：THUCNews中文文本数据集
	
