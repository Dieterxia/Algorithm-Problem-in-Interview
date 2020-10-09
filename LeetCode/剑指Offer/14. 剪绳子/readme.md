# 一
## 题目描述
给你一根长度为 n 的绳子，请把绳子剪成整数长度的 m 段（m、n都是整数，n>1并且m>1），
每段绳子的长度记为 k[0],k[1]...k[m-1] 。请问 k[0]*k[1]*...*k[m-1] 可能的最大乘积是多少？
例如，当绳子的长度是8时，我们把它剪成长度分别为2、3、3的三段，此时得到的最大乘积是18。

## 思路
* https://leetcode-cn.com/problems/jian-sheng-zi-lcof/solution/mian-shi-ti-14-i-jian-sheng-zi-tan-xin-si-xiang-by/
### 函数极值
* 算术-几何平均值不等式:   
![](http://latex.codecogs.com/gif.latex?\\frac{x_1+x_2...+x_n}{n}>=\\sqrt[n]{x_1x_2...x_n}) 等号成立当且仅当![](http://latex.codecogs.com/gif.latex?x_1=x_2=...=x_n) 
* 分成a段，求x^a的极大值，求导，得x=e时最佳。因为x只能取整数3最佳。如有剩余则2则保留，1则最终分为4
* Python 中常见有三种幂计算函数： ** 和 pow() 的时间复杂度均为 O(loga) ；而 math.pow() 始终调用 C 库的 pow() 函数，其执行浮点取幂，时间复杂度为 O(1) 。

### 动态规划
* 将每一个小于n的最大值算出，然后将n分成两部分遍历相乘取最大。

# 二
## 描述
数值太大超出边界，结果只能取模1e9+7

##思路
* https://leetcode-cn.com/problems/jian-sheng-zi-ii-lcof/solution/mian-shi-ti-14-ii-jian-sheng-zi-iitan-xin-er-fen-f/
* 直接用结果取模无用，因为结果以超限
* ![](http://latex.codecogs.com/gif.latex?(xy)%p=[(x%p)(y%p)]%p)
* 不可用中途用除法再取模
