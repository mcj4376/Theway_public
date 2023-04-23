[Desmos | 免费领略数学之美](https://www.desmos.com/?lang=zh-CN)

# 第一章 函数与极限

## 第一节 映射与函数

### 1、映射

$$
定义： 设 X,Y是两个非空集合，如果存在一个法则f，使得对X中每个元素x，\\按法则f，在Y中有唯一确定的元素y与之对应，那么称f为从X到Y的映射，记作：\\f:X \rightarrow Y
$$

### 2、双曲函数

### 3、极限

$$
定义：设 \{ x_n\} 为一数列，如果存在常数 a , 对于 \forall ，\varepsilon > 0 , \exists : N > 0, 使得当 n > N 时，\\ 不等式 \mid  x_n - a \mid < \varepsilon 都成立，那么就称常数 a 是数列 \{ x_n \} 的极限，记为 \lim\limits_{n\to\infty} x_n = a, \\ 或者称数列 \{ x_n \} 收敛于 a ,记为 x_n \to a \quad (n \to \infty)
$$

### 4、无穷小

$$
如果函数 f(x) 当 x \to x_0 \quad (或x \to \infty)时的极限为零，那么称函数 f(x) 为当x \to x_0 \quad (或x \to \infty)时的无穷小。
$$

### 5、无穷大

$$
设函数 f(x) 在 x_0 的某一去心邻域内有定义 （或 \mid x \mid 大于某一正数时有定义）。如果对于 \forall \quad M > 0,\quad \exists: \delta > 0, \\只要 0 < \mid x - x_0 \mid < \delta,对应的函数值 f(x)总满足不等式 \quad  \mid f(x) \mid > M,那么称函数f(x) 是当 x \to x_0时的无穷大
$$

### 6、极限运算法则

- 两个无穷小的和是无穷小

- 有界函数与无穷小的乘积是无穷小

  > - 常数与无穷小的乘积是无穷小
  >
  > - 有限个无穷小的乘积是无穷小
  >
  > - $$如果 limf(x) = A,limg(x) = B,那么$$
  >
  >   > - $$(1) \quad lim[f(x) \pm g(x) ] = limf(x) \pm limg(x) = A \pm B;$$
  >   >
  >   > - $$(2) \quad lim[f(x) \cdot g(x)] = limf(x) \cdot limg(x) = A \cdot B;$$
  >   >
  >   > - $$若又有 B \neq 0,则$$
  >   >
  >   >   $$lim \frac{f(x)}{g(x)} = \frac{limf(x)}{limg(x)} = \frac{A}{B}$$

- 如果 $$limf(x)存在，而c为常数，那么：$$$$ lim[cf(x)] = climf(x)$$

- 如果 $$limf(x)存在，而n是正整数，那么：$$$$ lim[f(x)]^n = [limf(x)]^n$$

### 7、极限存在准则

#### 7.1 夹逼准则

- **准则$$I$$：如果数列$$\{x_n\}，\{y_n\}及\{z_n\}$$满足下列条件：**

  ​              $$(1) \quad 从某项起，即\exists \quad n_0 \in N_+,当\quad n > n_0 \quad 时,有\quad  y_n \le x_n \le z_n $$

​                     $$(2) \quad \lim\limits_{n\to\infty} y_n = a,\lim\limits_{n\to\infty} z_n = a$$

​                     那么数列$$\{x_n\}$$的极限存在，且$$\lim\limits_{n\to\infty} x_n = a$$

- **准则$$I'$$：如果：**

  ​              $$(1) \quad 当 x \in \mathring{U} (x_0,r)(或\mid x \mid > M)时,\quad  g(x) \le f(x) \le h(x)$$

​                     $$(2) \quad  g(x) = A,\lim\limits_{{x\to\infty}或{x \to x_0}} h(x) = A$$

​                     那么数列$$\lim\limits_{{x\to\infty}或{x \to x_0}}f(x)，且等于A$$

- 单调有界数列必有极限

#### 7.2 两个重要极限

<font color=#ff0000>$\lim\limits_{x \to 0} \frac{sinx}{x} = 1 \quad \quad \quad \quad \lim\limits_{x \to \infty} (1 + \frac{1}{x})^x = e$</font>
