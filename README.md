# sparkify-udacity

    
## 项目定义和动机（Motivations）：

用户流失是每个软件公司不愿意看到的事情，对于音乐公司也是如此。因此，根据用户以前的数据，预测可能的流失用户，在用户注销之前提供各种可能的挽留措施，能够最大限度减少软件公司的用户损失情况。

在这篇报告中，我根据Udacity提供的数据，在IBM Watson Studio(free version) 云平台上运用Pyspark完成了对该数据集的大数据处理分析预测。预测流失用户，本质上是针对用户的二分类问题，因此适合采用监督学习的机器学习方法。项目主要流程包括：数据清洗，探索性分析（EDA），特征工程，监督学习建模，建模过程中采用f1分数对模型进行评估和改进。
    
## 项目数据：
完整的数据集大小为 12GB，由于计算调价的限制，我们选取了它的一个迷你子集，大小约为几百兆，并在免费的IBM云完成大数据任务的处理

## 使用到的库：
    1.pyspark.ml, pyspark.sql 大数据库
    2.IBM Watson Studio(free version) 云平台
    3.pandas, numpy, matplotlib 用于基本的数据处理和可视化

## 项目简介：
   ### 项目流程：
    1. 加载数据，并完成数据的清理
    2. 数据的探索和可视化
    3. 特征工程：选取性别，歌曲数目，相关的页面等特征
    4. 建模并预测
### 项目结果：
结果比较：
- LogisticRegression (best f1 score 0.7714)
- GBTClassifier (best f1 score 0.7214 )
- RandomForestClassifier (best f1 score 0.7276)

采用logistice regression, random forest,GBTClassifier三种监督学习模型，logistice regression效果较好，f1_score为0.77
### 反思和改进：
    1. 一开始想在原始数据上进行建模，后来发现独立出来后join比较方便
    2. 数据的向量化和标准化放在特征工程后比较方便

## 结果与讨论
实验了三个模型：LogisticRegression, RandomForestClassifier, GBTClassifier，其中效果最好的是逻辑回归模型（f1_score：0.77），可以采用该模型对数据进行预测流失用户。
    
## 进一步的工作计划
对于该模型，将用户随机分成基于账号ID的两组，一组对预测为流失的用户进行优惠活动，一组照常，然后以顾客流失率作为指标进行A/B测试。
      
## 参考：
https://github.com/Mikemraz/Capstone-Project-Big-Data-Sparkify 
    
## 感谢：
udacity提供课程和相关的数据
