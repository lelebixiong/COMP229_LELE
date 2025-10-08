location:描述数据“集中在什么地方,arithmetic mean（算术平均数);geometric mean（几何平均数）;mode（众数）;median（中位数）;3rd quartile（第三四分位数）
spread:描述数据“分散或变动的大小”,variance（方差）;standard deviation（标准差）;IQR（四分位距）;outlier（离群值）

A Probability space includes 
		1.a sample space样本空间(elementary, single, exclusive events),记作： Ω  P(Ω)=1 
		2.an event space事件空间 由样本空间中的元素（样本点）组成的**子集**，记作`E⊆Ω  
Kolmogorov公理：互斥事件(disjoint event)的概率可以相加
Ai , Aj事件不能同时(simultaneously)发生,那么就称作互斥事件(disjoint, non-intersecting)

![[Pasted image 20250926093104.png]]
![[Pasted image 20250926093116.png]]
**互斥情况**：
P(A∪B)=P(A)+P(B)
**一般情况**：
P(A∪B)=P(A)+P(B)−P(A∩B)
假设 A, B 独立（infependent） → 所以 P(A∩B)=P(A)P(B) 本质：一个事件的发生对另一个事件没有影响
		**事件与自身独立？** 只有在 P(A)=0或1时成立。
		**事件与补集独立？** 也只有在 P(A)=0或1时成立。
		**互斥事件独立？** 除非其中一个事件概率为 0，否则不可能独立。
Monotonicity: 若A⊆B，那么P(A)≤P(B)

pairwise independent成对独立: P(Ai​∩Aj​)=P(Ai​)P(Aj​); 相互独立 ⇒ 成对独立
mutual independent相互独立: 不仅两两独立，还要所有子集都独立




