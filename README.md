# Kaggle--quora_35th_solution
https://www.kaggle.com/c/quora-insincere-questions-classification

### 比赛背景：
+ 检测有毒内容以改善在线对话，开发识别和标记非真诚问题的模型。

### 技术工具：
+ 采用 python + pytorch

### 数据集：
+ 1306122 训练集和 56370 测试集

### 主要工作：

+ 预处理包括对数据集进行标点和特殊符号的清洗，替换部分错词，使用 nltk 切词并统计词频，进行 zero-padding 至固定文本长度；
    
+ 使用平均词向量代替单一词向量；
    
+ 分别使用 lstm + gru + capsule 和 lstm + gru + attention 网络结构及 cyclical 学习率（CLR）训练4个模型，并对预测结果进行 blending 。
    
