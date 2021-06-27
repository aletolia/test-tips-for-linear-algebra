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























