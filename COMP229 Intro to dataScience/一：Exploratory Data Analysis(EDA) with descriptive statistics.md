Z = all integers
R = all real numbers
For every new dataset, 
                start with develop a problem which we need to solve;
                data dictionary (data such as meaning, relationships to each data) from IBM Dictionary of computing
Missing values
         Missing Completely At Random(MCAR) = a random related missing values that you cannot reconstruct
         Missing at random(MAR) = missing at random that can be reconstructed with more information
         Missing Not At Random(MNAR)= missing for a reason
 Dealing with missingness
         omit it (patrial or full)把有缺失值的行直接删掉。
         full analysis using EDA
         简单填补:数值型：用均值、中位数、众数替换缺失值/分类变量：用众数替换; 
                模型预测填补：用 KNN、回归、随机森林等方法预测缺失值。


## 描述性统计（Descriptive Statistics）：features by numbers or diagrams
                                 集中趋势：均值 (mean)、中位数 (median)、众数 (mode)
                                 离散程度：方差 (variance)、标准差 (standard deviation)、极差 (range)、四分位距 (IQR)
		                                   样本方差（sample variance(分母为n-1，n为样本容量))，总体反差（population variance（分母为n，n为样本容量))
                                 分布形态：偏度 (skewness)、峰度 (kurtosis)
                                 图形表示：直方图、箱线图、饼图、柱状图


 ## 推断性统计（Inferential Statistics）: learn about unobserved population from a smaller sample--据样本做出关于总体的结论
                              bias--difference between population value and sample value



 中位数--样本量分奇数个和偶数个，从小到大排序后，奇数个取中间值，偶数个取中间两个的mean值
 
		   positive skew（正偏）--均值 > 中位数 > 众数（大部分数据集中在较小的数值区域,长尾在右边)
		   Symmetrical Distribution（对称分布）--均值 = 中位数 = 众数(数据集中在中间，两边逐渐减少)
		   Negative Skew（负偏分布 / 左偏分布）--均值 < 中位数 < 众数(大部分数据集中在较大的数值区域,长尾在左边)

 ## **几分位数（quantiles）**
          计算步骤（以四分位数为例）
              6,7,15,36,39,40,41,42,43,47,49（共 11 个数, 已经排好序）
              找 Q2（中位数）--Q2 = 第 (n+1)/2 = **40**
              找 Q1（下四分位数）--取前一半数据：6,7,15,36,39;    个数 = 5，Q1 = 第(5+1)/2 = 3=15
              找 Q3（上四分位数）--取后一半数据：41,42,43,47,49;       ...43
              