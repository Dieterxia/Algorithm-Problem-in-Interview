### 题目描述：
把一个数组最开始的若干个元素搬到数组的末尾，我们称之为数组的旋转。
输入一个非递减排序的数组的一个旋转，输出旋转数组的最小元素。
例如数组[3,4,5,1,2]为[1,2,3,4,5]的一个旋转，该数组的最小值为1。
NOTE：给出的所有元素都大于0，若数组大小为0，请返回0。

### 我的思路：
既然只有一个旋转，那就从后往前找到第一个转折点 与数组第一位比较

### 主流思路：

二分法查找（前提数据有序）：

![image](https://github.com/Dieterxia/Interview-algorithm-questions/blob/master/%E7%89%9B%E5%AE%A2%E7%BD%91/%E5%89%91%E6%8C%87offer/006-%E6%97%8B%E8%BD%AC%E6%95%B0%E7%BB%84%E7%9A%84%E6%9C%80%E5%B0%8F%E6%95%B0%E5%AD%97/%E4%BA%8C%E5%88%86%E6%B3%95%E5%8F%98%E7%A7%8D.png)

(https://blog.nowcoder.net/n/dcb0f2e6ffd44e1895b7a5297e362778?f=comment)
