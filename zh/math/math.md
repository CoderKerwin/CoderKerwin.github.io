# 数学

## 几何
- 解析几何
 - 平面解析几何
 - 空间解析几何

## 代数
- 线性代数
- 布尔代数
 - 逻辑与：1 * 1 = 1, 0 * 1 = 1 * 0 = 0 * 0 = 0
 - 逻辑或：0 + 0 = 0, 0 + 1 = 1 + 0 = 1 + 1 = 1
 - 运算律：A + !A = 1, 1 + A = 1, A + AB = A
 - 运算律：A * !A = 0
 - 运算律：(A + B) * (!A + !B) = (A * !B) + (!A * B)

## 数论

1. 进位计数制不一定只能有二进制八进制十进制十六进制，也可以创造三进制六进制九进制，但最常用还是十进制二进制八进制十六进制。
2. 日常生活用了的乘法口诀与加法口诀准确来说应该是十进制乘法口诀与十进制加法口诀，用其算出来的值对应十进制计数值。
3. 当然也可以总结八进制与十六进制口诀表，只是日常生活不常用。
4. 假设有个`A`进制数为`abcd`，其对应值为`a * (A * A * A) + b * (A * A) + c * A + d`，用A进制口诀恰好算的结果为`abcd`，用十进制口诀则算出对应十进制表示数。**注意用A进制必须把每个数都先表示成A进制数**。
5. 电子计算机将所有内容都表示成二进制然后做运算。比如汇编指令`mov eax, 10h`，电子计算机看到的是`mov eax, 10000b`。
6. 用计算机转换进制可以用除数与余数方式，比如`A/B`余数为`B`进制数，商为进1个`B`所表示的数，当其大于B时应继续做除数余数方式，循环直到商小于`B`为止
7. 口算进制运算可以采用拆数与补数方式，举例十六进制`5 * D = 5 * 8 + 5 * 4 + 5 = 20h + 8 + 10h + 4 + 4 + 1 = 41h`或者`5 * D = 5 * 10h - 5 * 3 = 41h`。十六进制用8和10h拆，有时可用4拆。十进制用5拆。
6. 负数表示为`0-1=-1`，比如`INT8`表示`-128 ~ 127`，用`00h`表示0，用`00h - 1 = ffh`表示-1，用`00h - 1 - 7fh = ffh - 7fh = 80h`表示-128。
7. 数的表示最重要是0与1的表示，只有这个确认了，才能计算`1 + 1 = 2`这种运算。也就是**数学公理化**。

## 集合论

## 概率论

## 图论

## 拓扑

## 数学学报

## 参考
1. [数学研发网](https://emath.ac.cn)：幻方
2. [汇心几何学](https://bbs.emath.ac.cn/forum.php?tid=18164&mod=viewthread)
3. [数学书籍](https://bbs.emath.ac.cn/thread-1989-1-1.html)

4. [博士数学家园](https://www.math.org.cn)

5. [康托尔的数学人生](https://page.om.qq.com/page/OdnrB-mpOio1ZnPwWq2rDhAA0)：集合论、超无穷、超限数

6. [USTC学习资料](http://home.ustc.edu.cn/~yx3x/USTCdata.html)

7. [数学证明方法概述](https://blog.csdn.net/cnds123/article/details/127186417)

8. [0.999...=1？数到底是什么？李永乐老师讲数学公理化](https://www.bilibili.com/video/av44942988)

9.  [黎曼几何                                                                          ](https://zhuanlan.zhihu.com/p/49545466)
10. [从韩信点兵到拉格朗日插值多项式及其推广（二）——额外介绍范德蒙行列式方法            ](https://zhuanlan.zhihu.com/p/563564002)
11. [从韩信点兵到拉格朗日插值多项式及其推广（三）——埃尔米插值多项式与范德蒙行列式的推广](https://zhuanlan.zhihu.com/p/563566506)
12. [浙大第四版《概率论与数理统计》课后习题答案解析最全分享                            ](https://zhuanlan.zhihu.com/p/358299124)

13. [概率论与数理统计(浙大四版)](https://github.com/xitongsys/ML/tree/master/books/概率论与数理统计(浙大四版).pdf)

14. [同济大学线性代数第五版课后习题答案](https://www.docin.com/p-1907112302.html)

15. [克莱姆法则](https://baike.baidu.com/item/克莱姆法则)
16. [逆命题    ](https://baike.baidu.com/item/逆命题)
17. [伽玛函数  ](https://baike.baidu.com/item/伽玛函数)
18. [范数      ](https://baike.baidu.com/item/范数)
19. [陶哲轩    ](https://baike.baidu.com/item/陶哲轩)
20. [张益唐    ](https://baike.baidu.com/item/张益唐)

21. [gamma分布 松理解gamma分布](https://blog.csdn.net/weixin_39883433/article/details/111222022)

22. [数学常用希腊字母念法（附字母表）](https://blog.csdn.net/leoleepz/article/details/50313867)

23. [为什么(xe^(-x))当X趋于无穷时的极限是0啊？怎么算出来的？](https://wenwen.sogou.com/question/q657935015.htm)

24. [反常积分∫xe^-x^2 dx，上限无穷大，下限0 怎么求？](https://www.zhihu.com/question/54539278)

25. [定义数学期望的时候为什么一定要求级数满足绝对收敛呢？](https://www.zhihu.com/question/26566795)

26. [EXCEL2007如何找到数据分析工具](https://jingyan.baidu.com/article/8cdccae99e3247315513cd4a.html)

27. [numpy中的log和ln函数](https://blog.csdn.net/u011699626/article/details/118885071)

28. [SPSS——相关分析——Pearson简单相关系数](https://blog.csdn.net/liuyuan_jq/article/details/52517963)

29. [进位计数制](https://baike.baidu.com/item/进位计数制)

30. [科学计数法](https://baike.baidu.com/item/科学计数法/1612882)

31. [中国数学会](http://www.cms.org.cn)

32. [线性代数之——正定矩阵](https://zhuanlan.zhihu.com/p/93392382)

33. [MarkDown数学公式](https://zhuanlan.zhihu.com/p/441454622)

34. [范式球，范式锥，欧式球，椭球](https://blog.csdn.net/robert_chen1988/article/details/80479813)

35. [凸集](https://zhuanlan.zhihu.com/p/33231654)

36. [对称矩阵及重要性质](https://zhuanlan.zhihu.com/p/627861657)

37. [半正定锥](https://zhuanlan.zhihu.com/p/570781608)

38. <https://math.stackexchange.com/questions/1857317/why-deta-1-1-deta>
39. <https://math.stackexchange.com/questions/842898/is-detab-detba>

40. [矩阵求导](https://zhuanlan.zhihu.com/p/273729929)

41. [高等数学和数学分析之间区别](https://www.zhihu.com/question/370000187)
42. [数学分析教材或参考书推荐  ](https://www.zhihu.com/question/427922224)
43. [数学分析                  ](https://www.zhihu.com/topic/19622000)

44. [数学专业最全介绍](https://zhuanlan.zhihu.com/p/399827103)

45. [数学史推参考书荐](https://www.zhihu.com/question/20100262)

46. [数学史浅述](https://zhuanlan.zhihu.com/p/139716871)
