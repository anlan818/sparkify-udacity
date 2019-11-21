# sparkify-udacity

    
## 项目定义和动机（Motivations）：
    1. 根据用户的数据，预测注销的用户，借此推送给这类用户一定的促销措施来挽留用户。
    2. 在大数据平台上完成机器学习的项目，熟悉大数据处理的流程
 
    
## 项目数据：
    完整的数据集大小为 12GB，由于计算调价你的限制，我们选取了它的一个迷你子集，大小约为几百兆，并在免费的IBM云完成大数据任务的处理

    
## 使用到的库：
    1.pyspark.ml, pyspark.sql 大数据库
    2.IBM Watson Studio(free version) 云平台
    3.pandas, numpy, matplotlib 用于基本的数据处理和可视化

    
## 项目简介：
   ### 项目流程：
        1. 加载数据，并完成数据的清理
        2. 数据的探索和可视化
        3. 特征工程，选取性别，歌曲数目，相关的页面等特征
        4. 建模并预测
    ### 项目结果：
        采用logistice regression和random forest两种非监督模型，logistice regression效果较好，最终的结果ROC曲线下的面积约为0.67，结果比较满意

    
## 反思和改进：
    1. 一开始想在原始数据上进行建模，后来发现独立出来后join比较方便
    2. 其他三种非监督模型方法没有试验，有时间可以继续尝试
    3. 数据的向量化和标准化放在特征工程后比较方便
      
## 参考：
    https://github.com/Mikemraz/Capstone-Project-Big-Data-Sparkify 学业导师提供的参考
    
## 感谢：
    udacity提供课程和相关的数据
