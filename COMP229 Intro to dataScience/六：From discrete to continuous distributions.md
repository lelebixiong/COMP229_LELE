**期望的线性性**：E[aX+bY]=aE[X]+bE[Y]
随机变量 X的 **CDF** 定义为：F(k)=P(X≤k)      =k∑i=0​P(X=i)

## 伯努利随机变量
	 它只取两个可能的值：X∈{0,1}
		- X=1X = 1X=1：表示“事件发生”（成功）  
		- X=0X = 0X=0：表示“事件未发生”（失败）  
P(X = 1) = p, P(X = 0) = 1 − p

概率质量函数（PMF)：
 f(k)=P(X=k)={  p，    k=1---------------》f(k)=p^k (1−p)^1−k,k∈{0,1}
            { 1−p，k=0​---------------》
E[X]=0×(1−p)+1×p=p
方差（Var(X)）：E[X2]−(E[X])2=p−p2=p(1−p)


## 二项分布
![[Pasted image 20251007092008.png]]
**期望（Expectation）**：E[X]=np
**方差（Variance）**：Var(X)=np(1−p)
PMF 图是“柱状图”，表示每个成功次数 k 的概率：


## **Poisson 分布**（泊松分布）
在**固定时间或空间区间**中，某个事件**随机且独立地发生**的次数。
![[Pasted image 20251007092650.png]]


## Poisson 极限定理（Poisson limit theorem，又称稀有事件定律 law of rare events）
当满足:n→∞,p→0,且 np=λ 固定
则：Binomial(n,p)  ⇒  Poisson(λ)
即 **二项分布趋近于泊松分布**。
直观地说：
> 当试验次数很多，但每次成功概率极小（“稀有事件”）时，Poisson 是 Binomial 的极限形式。

应用场景
![[Pasted image 20251007093218.png]]

## 离散均匀分布（Uniform discrete distribution）
![[Pasted image 20251007093326.png]]


连续型均匀分布（Uniform Continuous Distribution）
![[Pasted image 20251007093547.png]]
![[Pasted image 20251007093600.png]]
![[Pasted image 20251007093611.png]]


均匀变量的密度（The density of a uniform variable）
![[490f36eabb04f1f36094f9dc046d7e7a.jpg]]
均匀密度（Uniform density）
![[00e525132d34e453ca2fd431f6a40d0d.jpg]]

例题：
![[Pasted image 20251007095910.png]]
![[Pasted image 20251007100049.png]]
![[Pasted image 20251007100105.png]]



## **累积分布函数 (CDF)**
- FX(v) = P(X ≤ v) 表示随机变量X小于或等于v的概率
## **离散随机变量**
- 用**概率质量函数 (PMF)** 定义
- pi = P(X = vi) 表示X取特定值vi的概率
## **连续随机变量**
- 用**概率密度函数 (PDF)** 定义
- PDF是CDF的导数
## **均匀分布**
在有界区间内，密度函数为常数
![[Pasted image 20251008102332.png]]
总结一下：概率密度函数 f(x)是非负的，它表示每个点附近的概率密度；  
积分（曲线下的面积）代表实际概率，总面积必须为 1；  
因此 f(x)在两端必须趋向 0。


## Exponential function：
e 是唯一使得指数函数 e^x 的导数等于它自身的数。  
因此函数 e^x 的切线斜率等于其 y 值，表现为快速的指数增长。

指数分布：
![[Pasted image 20251008103047.png]]

二项分布 B(n,p)表示 n 次独立试验（每次实验是一次 **Bernoulli 试验（伯努利试验）**）中的成功次数
	 结果只有两种：  
	 ✅ 成功（probability = p）  
	 ❌ 失败（probability = 1 - p）
当 n 很大、p 很小时，它可以近似为泊松分布；  
而泊松过程的事件间隔时间服从指数分布。  
所以它们之间的“相似”并不是巧合，而是数学上的联系。
![[Pasted image 20251008103524.png]]



## 一维和高维情况
![[Pasted image 20251008104629.png]]

![[Pasted image 20251008104618.png]]


### 维度诅咒（The curse of dimensionality）
![[Pasted image 20251008105846.png]]
