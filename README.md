# bert_family_classification
支持Roberta、albert、bert以及转化为tf版本的ernie等bert大家族所有预训练模型的加载、完成cls、ner、mrc三种经典任务（部分predict代码需要自行调整，train没有大问题）。

支持分段设置学习率，提高模型表现。

支持继续在domain数据中继续进行pertrain（albert除外）

支持冻结不同encoder层以优化模型效果（albert除外）

支持提取不同encoder层的输出并在此基础上修改网络结构

提供自定义loss和callback函数，便于使用者在此基础上调整

支持对于不均衡样本二、多分类的focal loss函数

支持tensorboard调用（需要修改tensorboard部分源码，方法参考https://www.jianshu.com/p/9da54361d289），实现训练可视化
************************************************************************************************************************

/stripts目录下保存在服务器进行训练的命令

/data中每个数字子目录保存每次对模型或者数据进行调整之后的训练数据，便于模型调优

/data/1/下放有cls、ner、mrc三个任务数据格式的说明和对应的example

/models中每个数字子目录保存每次进行调优后的模型

/sub中每个数字子目录保存每次调优后的predict提交csv文件

************************************************************************************************************************

roberta系列预训练模型:https://github.com/brightmart/roberta_zh

albert系列预训练模型:https://github.com/bojone/albert_zh

tf版ERNIE预训练模型:https://github.com/ArthurRizar/tensorflow_ernie

************************************************************************************************************************
感谢各位大佬的贡献~
欢迎fork，项目会继续更新
客官若是满意的话，请star支持一下吧( ￣▽￣)σ
