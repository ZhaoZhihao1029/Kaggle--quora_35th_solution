# Kaggle--quora_35th_solution
https://www.kaggle.com/c/quora-insincere-questions-classification

比赛背景：检测有毒内容以改善在线对话，开发识别和标记非真诚问题的模型。

主要工作：技术工具采用python + pytorch。

+ 预处理包括对130.6w训练集和5.6w测试集进行标点和特殊符号的清洗，替换部分错词，使用nltk切词并统计词频，进行zero-padding至固定文本长度；
    
+ 使用平均词向量代替单一词向量；
    
+ 分别使用lstm + gru + capsule和lstm + gru + attention网络结构及cyclical学习率（CLR）训练4个模型，并对预测结果进行blending。
    
