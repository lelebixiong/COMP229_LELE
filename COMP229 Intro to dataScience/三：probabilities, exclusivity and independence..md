![[Pasted image 20250930091301.png]]
P(A) = 0.3 + 0.1+ 0.12 = 0.52
P(A|B1)=1
P(A|B2)= 0.12/(0.12 + 0.04)= 0.75
P(A|B3)=0

## **乘法法则**
	P(A∩B)=P(A∣B)P(B) 
	如果事件独立，则公式简化为：P(A∩B)=P(A)⋅P(B) 
加法法则
	P(A∪B)=P(A)+P(B)−P(A∩B) 
	如果 A 和 B **互斥（disjoint）**，则公式简化为： P(A∪B)=P(A)+P(B)

## 全概率公式：
如果 Ω可以被划分为若干个 **互斥且完备的事件** B1,B2,…,Bn​，那么：
- “互斥”表示：Bi∩Bj=∅（不同的 B不会同时发生）
- “完备”表示：⋃nBn=Ω（所有可能结果都被覆盖）
	- 由于P(A∩Bn​)=P(A∣Bn​)⋅P(Bn​)
	-所以P(A)=∑​P(A∩Bn​)=∑​P(A∣Bn​)P(Bn​)

## 贝叶斯公式Bayes formula：
P(A∣B)=P(B∣A)P(A)​/P(B)

![[Pasted image 20250930093745.png]]
	P(cancer)=0.01,P(no cancer)=0.99 
	P(positive∣cancer)=0.8 
	P(positive∣no cancer)=0.1 
	P(cancer∣positive)=P(posotive∣caner)⋅P(cancer)/​P(positive) 
	P(positive)=P(positive∣cancer)P(cancer)+P(positive∣no cancer)P(no cancer)=(0.8)(0.01)+(0.1)(0.99)=0.008+0.099=0.107 

	 灵敏度 Sensitivity(病人中有多少被测出来是病人):Sensitivity=TP/(TP + FN)​      Recall(召回率)=TP/(TP + FN)​ 
	 特异度 Specificity(健康人中有多少被测出来是健康的):Specificity=TN/(TN+FP) 
	 精确率 Precision:Precision=TP/(TP + FP)​

# F-score 的定义
	F-score 是 **精确率（precision）** 和 **召回率（recall）** 的调和平均数： 
	![[Pasted image 20250930101718.png]]
	



 