## TEST TIPS FOR LINEAR ALGEBRA

矩阵在转置前后不改变行列式的值

应用于证明行列式为0或其他等式（尤其适用于对称矩阵），例

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627135442101.png" alt="image-20210627135442101" style="zoom:67%;" />

![image-20210627135523908](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627135523908.png)

代数余子式的标记：

$A_{12}$ 指的是第一行第二列元素所对应的代数余子式

我们应用代数余子式，实际上是通过行列式的性质（见linear algebra），将矩阵拆成了一个个小矩阵并利用行列式部分线性的性质来求算行列式。我们知道，假如我们取第一行的代数余子式，根据定义我们不难知道它们之间必然是（指那些被拆开的小矩阵）是可逆矩阵，但如果我们去求第二行的元素乘以第一行的代数余子式的行列式，那么必然为0，例题如下

![image-20210627141732549](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627141732549.png)

要注意的是，代数余子式的值与其展开的行之间毫无关系（这是说，假如我们想计算第一行元素展开得到的代数余子式，但不难想象，我们所求出的代数余子式的值与第一行中的元素的大小毫无关系）无论第一行中的元素大小如何改变，假如其他位置的元素大小不改变，那么其求得的代数余子式值不会发生变化。该性质适用于求解某一行（列）对应代数余子式的和，例如

![image-20210627142517608](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627142517608.png)

此外，根据矩阵本身的构成，可以特意构造奇异矩阵来简化计算，例如

![image-20210627142739091](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627142739091.png)

这里第一步不是简单将第三行构造为1、1、1、0、0，而是直接将其构造成奇异矩阵，因此大大简化了计算。再结合我们此前提到过的性质，有

![image-20210627142913634](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627142913634.png)

![image-20210627143219919](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627143219919.png)

此外对于 $n\times n$ 的方阵，除了数学归纳法以外，还可以利用其性质（递推关系）解题，例如

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627143443179.png" alt="image-20210627143443179" style="zoom:67%;" />

这里我们可以将其当作数列来做

以及化为块对角矩阵（两例）

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627143626656.png" alt="image-20210627143626656" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627143905474.png" alt="image-20210627143905474" style="zoom: 67%;" />

首先观察行列式的排列规律，然后利用性质化为容易求解的行列式，例如

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627151005924.png" alt="image-20210627151005924" style="zoom: 67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627151018086.png" alt="image-20210627151018086" style="zoom: 67%;" />

此外还有两种常用的方法和技巧（首先我们要先归纳所求矩阵的特征）

1.把各行（列）加到同一行（列）上去

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627151316845.png" alt="image-20210627151316845" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627151334178.png" alt="image-20210627151334178" style="zoom:67%;" />

即当行列式各行（列）的元素之和相等时，先求和，再提取公因式，然后再用其他方法计算行列式的值（特别是当行列式中存在相同的系数时）

2.拆分法

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627152311335.png" alt="image-20210627152311335" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627152322475.png" alt="image-20210627152322475" style="zoom:67%;" />

较复杂的递推法

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627152707116.png" alt="image-20210627152707116" style="zoom:67%;" />

升阶法

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627153549758.png" alt="image-20210627153549758" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627153602157.png" alt="image-20210627153602157" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627153612842.png" alt="image-20210627153612842" style="zoom:67%;" />

该方法适用于每一行（列）都包含有一个共有元素的情况，下面的例子可能更加明显

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627153808789.png" alt="image-20210627153808789" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627153818842.png" alt="image-20210627153818842" style="zoom:67%;" />



<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627155247067.png" alt="image-20210627155247067" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627155256608.png" alt="image-20210627155256608" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627155800916.png" alt="image-20210627155800916" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627155815622.png" alt="image-20210627155815622" style="zoom:67%;" />

齐次→范德蒙特行列式

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627160505893.png" alt="image-20210627160505893" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627160520104.png" alt="image-20210627160520104" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627160727171.png" alt="image-20210627160727171"  />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161413236.png" alt="image-20210627161413236" style="zoom: 67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161430406.png" alt="image-20210627161430406" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161447180.png" alt="image-20210627161447180" style="zoom: 80%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161500362.png" alt="image-20210627161500362" style="zoom:80%;" />



<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161832249.png" alt="image-20210627161832249" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161847561.png" alt="image-20210627161847561" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627161941472.png" alt="image-20210627161941472" style="zoom:67%;" />

![image-20210627181915229](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627181915229.png)



注意，虽然内积 $A=\alpha^T\beta$ (其中$α$ 和 $β$ 是一个向量)，但 $A^n$ 是一个矩阵，例如

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627182322540.png" alt="image-20210627182322540" style="zoom:67%;" />

同样的，外积也是如此

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627183752435.png" alt="image-20210627183752435" style="zoom:67%;" />

注意方阵阶数和行列式值得对应关系，例如假如将三阶方阵乘以二，那么行列式的值会变大八倍；而同样的操作对于四阶方阵则会变大十六倍，例如

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627185601069.png" alt="image-20210627185601069" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627185619385.png" alt="image-20210627185619385" style="zoom: 67%;" />

此外，求行列式和求矩阵不同，还请注意

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627185733278.png" alt="image-20210627185733278" style="zoom:67%;" />

例如在上面这道题中，不必先解矩阵方程得到矩阵 $B$ 得具体值也可以计算出其行列式大小

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627185915549.png" alt="image-20210627185915549" style="zoom:67%;" />

几个特殊矩阵的行列式

![image-20210627190600097](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627190600097.png)

单位矩阵的应用

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627190641146.png" alt="image-20210627190641146" style="zoom:67%;" />

抽象化的代数余子式

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627190835268.png" alt="image-20210627190835268" style="zoom:67%;" />

有用的小结论1

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627191102236.png" alt="image-20210627191102236" style="zoom:67%;" />

两道相似的题目：

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627191755409.png" alt="image-20210627191755409" style="zoom: 67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627191817414.png" alt="image-20210627191817414" style="zoom:67%;" />

注意，矩阵的内外次幂可以交换，在遇到 $-1$ 要尤其注意

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627192813290.png" alt="image-20210627192813290" style="zoom: 80%;" />

注意单位矩阵的插入位置

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627193142815.png" alt="image-20210627193142815" style="zoom:67%;" />

这里将算式展开以后在右侧项的 $BA$ 中间插入了一个单位矩阵 $E$ 变为 $BEA$ ，完成了化简

此外单位矩阵还可以添置在矩阵两边来辅助计算

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627194144724.png" alt="image-20210627194144724" style="zoom:67%;" />

求等价标准型，这里的 $P$ 和 $Q$ 分别组合了 $A$ 的行和列，从而得到了标准型

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627201538848.png" alt="image-20210627201538848" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627201600721.png" alt="image-20210627201600721" style="zoom:67%;" />



<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627201621554.png" alt="image-20210627201621554" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627201644687.png" alt="image-20210627201644687" style="zoom:67%;" />

矩阵等价指的是两个矩阵在化为上三角阵以后有同样的形式

灵活使用行列式和矩阵的秩之间的联系

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627203321768.png" alt="image-20210627203321768" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627203336122.png" alt="image-20210627203336122" style="zoom:67%;" />

利用不等关系来判断矩阵秩的大小

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627204006416.png" alt="image-20210627204006416" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627204349212.png" alt="image-20210627204349212" style="zoom:67%;" />

怪题一

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627205005689.png" alt="image-20210627205005689" style="zoom:67%;" />

怪题的爸爸

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627205205214.png" alt="image-20210627205205214" style="zoom:67%;" />

结论1

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210627210204357.png" alt="image-20210627210204357" style="zoom: 67%;" />

通过将单位矩阵替换为矩阵于其逆矩阵的乘积来化简；$(A^T)^{-1}=(A^{-1})^T$，如果 $A$ 是对称矩阵，那么有 $(A^T)^{-1}=(A^{-1})^T=A^{-1}$

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628111546164.png" alt="image-20210628111546164" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628135643770.png" alt="image-20210628135643770" style="zoom:67%;" />

二项式展开+矩阵的 $n$ 次幂

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628112414862.png" alt="image-20210628112414862" style="zoom:67%;" />

想不清楚就算，要记住从定义出发

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628112735514.png" alt="image-20210628112735514" style="zoom: 50%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628113124361.png" alt="image-20210628113124361" style="zoom: 50%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628113556194.png" alt="image-20210628113556194" style="zoom:67%;" />

切忌生搬硬套

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628113915729.png" alt="image-20210628113915729" style="zoom: 50%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628134309155.png" alt="image-20210628134309155" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628135301859.png" alt="image-20210628135301859" style="zoom:67%;" />

凑配系数

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628135948192.png" alt="image-20210628135948192" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628140001334.png" alt="image-20210628140001334" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628140236646.png" alt="image-20210628140236646" style="zoom: 80%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628140628341.png" alt="image-20210628140628341" style="zoom:67%;" />

有关秩的一些小结论

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628140713791.png" alt="image-20210628140713791" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628140818818.png" alt="image-20210628140818818" style="zoom:67%;" />

求解矩阵方程时，若矩阵不可逆，则用待定系数法求解

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628142309836.png" alt="image-20210628142309836" style="zoom: 80%;" />

判断向量线性表示问题的常用方法

![image-20210628142723078](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628142723078.png)

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628144402862.png" alt="image-20210628144402862" style="zoom:80%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628144521792.png" alt="image-20210628144521792" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628144826499.png" alt="image-20210628144826499" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628152947774.png" alt="image-20210628152947774" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628154802427.png" alt="image-20210628154802427" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628160244577.png" alt="image-20210628160244577" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628160259739.png" alt="image-20210628160259739" style="zoom:67%;" />



基础解系的条件

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628182514055.png" alt="image-20210628182514055" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628182525735.png" alt="image-20210628182525735" style="zoom:67%;" />

概念判断

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628183510795.png" alt="image-20210628183510795" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628184636310.png" alt="image-20210628184636310" style="zoom:67%;" />

文字语言到数学语言的转化

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628191604350.png" alt="image-20210628191604350" style="zoom: 67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628191623584.png" alt="image-20210628191623584" style="zoom:67%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628195501509.png" alt="image-20210628195501509" style="zoom: 80%;" />

<img src="C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20210628200553550.png" alt="image-20210628200553550" style="zoom: 80%;" />























































































































































































