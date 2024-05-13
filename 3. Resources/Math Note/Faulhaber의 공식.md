---
tags:
  - faulhaber
  - 이항정리
---
### 수열의 합
우리는 고등학교에서 다양한 수열의 합을 구하게됩니다. 이때 $\sum$이란 기호를 처음 배우면서 가장 간단한 거듭제곱 수열들의 합을 유도하는 과정에 대해서 배우게 되죠.

$$
\begin{align*}
\sum_{k=1}^n k &=\frac{n(n+1)}{2}\\
\sum_{k=1}^n k^2 &=\frac{n(n + 1)(2n + 1)}{6}\\
\sum_{k=1}^n k^3 &=\frac{n^2(n + 1)^2}{4}
\end{align*}
$$

그런데 여러분들은 이 식들이 생각보다 매우 규칙적이라는 것을 알고 계셨나요? 오늘은 그 비밀을 함께 풀어보도록 하겠습니다.

## 1부터 $n$까지의 정수의 합
우선 가장 쉬운 $\sum_{k=1}^n k$부터 보도록 하겠습니다. 이 식은 흔히 $1$부터 $100$까지 더하여라 같은 등차수열의 합을 구하는데 사용되는 식입니다. 가우스가 어릴 적에 암산으로 풀었다는 사실로 더 유명한 문제죠.

이 식의 답을 구하는 과정은 어렵지 않습니다. 먼저 1부터 $n$까지의 수를 나열한 후 이 값들을 모두 더한 값을 $S$라 하겠습니다. 이제 같은 수열 하나를 더 만들어 방향만 바꾼 후 두 수열을 더해보겠습니다.

$$
\begin{array}{ccccc}
S & + & S & = & 2S \\ 
\hline
1 & & n & & n+1 \\
2 & & n-1 & & n+1 \\
3 & & n-2 & & n+1 \\
\vdots & & \vdots & & \vdots \\
n-1 & & 2 & & n+1 \\
n & & 1 & & n+1 \\
\end{array}
$$

이때 $2S$ 즉, 두 수열의 합을 보면 $n+1$이 $n$번 더해져 있이므로 $n\times(n+1)$입니다. 따라서 우리가 구해야하는 수열의 합 $S$는 두 수열을 더한 값을 $2$로 나눈 값과 같습니다.

$$S = \frac{n(n+1)}{2}$$  
이 식을 이용하면 유용한 값들을 쉽게 찾을 수 있습니다. 예를들어 $n$이 홀수라면 $n=2m-1$을 대입하여 홀수들의 합은 제곱수를 만든다는 사실을 쉽게 증명할 수 있죠. 그리고 등차 수열 $n$에 대한 $1$차 함수이므로 같은 방법으로 빠르게 해결할 수 있습니다.

$$\sum_{k=1}^n 2k-1 = 2\times \frac{n(n+1)}{2} - n=n^2$$
![홀수의 합|200](https://upload.wikimedia.org/wikipedia/commons/thumb/0/06/Square_number_16_as_sum_of_gnomons.svg/1280px-Square_number_16_as_sum_of_gnomons.svg.png)

## 1부터 $n^2$까지의 정수의 합
$1$부터 $n^2$까지의 합을 구하는 문제는 앞서 본 문제와 같이 마냥 쉽지는 않습니다. 우리는 $k^2$이라는 항을 얻어내 $\sum_{k=1}^n k^2$의 값을 구하기 위해서 $(k-1)^3$의 전개식으로부터 시작해보겠습니다. $(k-1)^3$의 전개식은 다음과 같습니다.

$$
(k-1)^3 = k^3 - 3k^2 + 3k - 1
$$

우리가 필요한 것은 $k^2$이므로 $k^3$을 없애기 위해 식을 변형하면 다음과 같습니다.

$$
k^3 - (k-1)^3 = 3k^2 - 3k + 1
$$

이제 $\sum_{k=1}^n k^2$을을 구하기 위해 양변에 각각 $\sum$을 취한 후 양변을 각각 보도록 하겠습니다.

$$
\sum_{k=1}^n \left( k^3 - (k-1)^3 \right) = \sum_{k=1}^n \left(3k^2 - 3k + 1\right)
$$

먼저 좌변을 보겠습니다. 우변의 일반항에 $1$부터 $n$까지 대입 한 후 각 항을 세로로 적고 모든 항을 더하면 같은 값에 부호만 다른 항들이 반복적으로 나오므로 소거할 수 있습니다. 따라서 우변은 정리하면 $n^2$이 됩니다.

$$
\begin{align*}
&1^3 &-&& 0^3& \\
&2^3 &-&& 1^3& \\
&3^3 &-&& 2^3&\\
&&\vdots&&& \\
+\quad&n^3 &-&& (n-1)^3& \\
\hline
&n^3&&&
\end{align*}
$$

다음으로 우변을 보겠습니다. 우변은 $\sum$에 선형성에 따라 분배해주면 식을 다음과 정리할 수 있습니다.

$$ \begin{align*}
&~\sum_{k=1}^n \left(3k^2 - 3k + 1\right) \\
=~ & 3  \sum_{k=1}^{n} k^2 - 3 \sum_{k=1}^{n} k + \sum_{k=1}^{n} 1 \\
=~ & 3  \sum_{k=1}^{n} k^2 - 3 \times \frac{n(n+1)}{2} + n \\
\end{align*}$$

마지막으로 정리된 결과를 원래식에 대입하여 $\sum_{k=1}^n k^2$으로 식을 정리해주면 $1$부터 $n^2$까지의 합을 구하는 공식을 구할 수 있습니다.

$$\begin{align*}
&&n^3 &= 3  \sum_{k=1}^{n} k^2 - 3 \frac{n(n+1)}{2} + n\\
\Rightarrow&& 3 \sum_{k=1}^{n} k^2 &= n^3 + 3 \times \frac{n(n+1)}{2} - n \\
\Rightarrow&& \sum_{k=1}^{n} k^2 &= \frac{1}{3} n^3 + \frac{1}{2} n^2 + \frac{1}{6} n \\
\Rightarrow&& \sum_{k=1}^{n} k^2 & = \frac{n(n+1)(2n+1)}{6}
\end{align*}$$

그리고 같은 방법으로 어렵지 않게 $1$부터 $n^3$까지의 합을 구하는 공식을 구할 수 있습니다.

$$
\begin{align*}
&&(k-1)^4 &= k^4 - 4k^3 + 6k^2 - 4k + 1\\
\Rightarrow&&\sum_{k=1}^n \left( k^4 - (k-1)^4 \right) &= \sum_{k=1}^n \left( 4k^3 - 6k^2 + 4k - 1 \right) \\
\Rightarrow&&n^4 &= 4 \sum_{k=1}^{n} k^3 - 6 \sum_{k=1}^{n} k^2 + 4 \sum_{k=1}^{n} k - n \\
\Rightarrow&& 4 \sum_{k=1}^{n} k^3 &= n^4 + 6 \times \frac{n(n+1)(2n+1)}{6} - 4 \times \frac{n(n+1)}{2} + n \\
\Rightarrow&& \sum_{k=1}^{n} k^3 &= \frac{1}{4} n^4 + \frac{1}{2} n^3 + \frac{3}{4} n^2 + \frac{1}{4} n \\
\Rightarrow&& \sum_{k=1}^{n} k^3 &= \frac{n^2(n+1)^2}{4}
\end{align*}
$$

여기까지는 고등학교 수업시간에 배우는 내용입니다. 그리고 학교에서 아마 이해를 돕기 위해 다양한 그림을 곁들이죠.

![$n^2$의 합|400](https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/Square_pyramidal_number.svg/1920px-Square_pyramidal_number.svg.png)


![$n^3$의 합|300](https://upload.wikimedia.org/wikipedia/commons/thumb/2/26/Nicomachus_theorem_3D.svg/512px-Nicomachus_theorem_3D.svg.png)


이 때의 결과는 내신이나 수능에 매번 출제되기도하고 나중에 정적분과 급수와의 관계에서 다시 등장하기에 보통은 외우고 있습니다.

$$
\int_{a}^{b} f(x) \, dx = \lim_{{n \to \infty}} \sum_{{i=1}}^{n} f(x_i^*) \Delta x
$$


## 일반화된 패턴
사실 이 공식을 보면서 일정한 규칙이 있다고 상상하기는 어렵습니다. 시험에서도 $3$제곱이상의 식을 물어보는 문제도 잘 출제되지 않으므로 굳이 고민하고 싶지도 않습니다. 그럼에도 불구하고 규칙을 찾아보기 위해 자세히 식을 관찰하면 이 식이 공통적으로 갖고 있는 특성을 찾을 수 있습니다. 이 식을 전개해서 보겠습니다.

$$
\begin{align}
\sum_{k=1}^n k &= \frac{1}{2}n^2 + \frac{1}{2}n &\quad(1)\\
\sum_{k=1}^n k^2 &= \frac{1}{3}n^3 + \frac{1}{2}n^2 + \frac{1}{6} &\quad(2)\\
\sum_{k=1}^n k^3 &= \frac{1}{4}n^4 + \frac{1}{2}n^3 + \frac{1}{4}n^2 &\quad(3)
\end{align}
$$

$(1)$, $(2)$, $(3)$번의 항등식을 보면 좌변은 $k$에 대한 다항식이며, 우변은 $n$에 대한 다항식입니다. 이때, 최고차항을 보면 항상 좌변의 최고차항의 차수보다 우변의 최고차항의 차수가 정확히 $1$만큼 더 크다는 사실을 알 수 있습니다. 사실 이는 자명한 결과입니다. 이 식을 유도하는 과정은 모두 같은 곳에서 출발하기 때문이죠. 바로 $(k-1)$의 거듭 제곱입니다. 

$$
\begin{align*}
(a+b)^n &= \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k\\
\Rightarrow (k-1)^n &= (-1)^{i+1} \sum_{i=0}^{n} \binom{n}{i} k^i
\end{align*}
$$
 
$(k-1)$의 전개식을 보면 상수$1$은 적절히 생략할 수 있으므로 결국 계수들은 조합의 수와 부호차이를 제외하면 같게 됩니다.

$$
\begin{array}{ccccccc}
&&&&&&&& 1 &&&&&&&& \\
&&&&&&& 1 && 1 &&&&&&&& \\
&&&&&& 1 && 2 && 1 &&&&&& \\
&&&&& 1 && 3 && 3 && 1 &&&&& \\
&&&& 1 && 4 && 6 && 4 && 1 &&&&\\
&&& 1 && 5 && 10 && 10 && 5 && 1 &&&\\
&&1 && 6 && 15 && 20 && 15 && 6 && 1 &&\\
&&&&&&&& \vdots &&&&&&&&
\end{array}
$$
따라서 이 식은 

Faulhaber의 공식에 대한 이해

Faulhaber의 공식은 자연수 $n$까지의 양의 정수 $k$의 $p$제곱의 합을 일반화한 공식입니다. 이 공식은 1631년에 J. Faulhaber에 의해 "Academiae Algebrae"라는 출판물에서 처음 발표되었습니다. 

#### 공식의 정의

Faulhaber의 공식은 다음과 같이 표현됩니다.[^1]

$$
\sum_{k=1}^{n} k^p = H_{n, -p} = \frac{1}{p+1} \sum_{i=1}^{p+1} (-1)^{\delta_{ip}} \binom{p+1}{i} B_{p+1-i} n^i
$$

- $H_{n, r}$ 일반화된 조화수(harmonic number)
- $\delta_{ip}$ Kronecker-delta(두 수가 같을 경우 1, 다를 경우 0)
- $\binom{n}{i}$ 조합, 이항계수(binomial coefficient)
- $B_i$ $i$번째 Bernoulli 수

[^1]: [Faulhaber's formula - Wolfram|Alpha](https://www6b3.wolframalpha.com/input?i=Faulhaber%27s+formula)

[Sums of Powers of Positive Integers - Introduction | Mathematical Association of America (maa.org)](https://maa.org/press/periodicals/convergence/sums-of-powers-of-positive-integers-introduction)

https://www.youtube.com/watch?v=k-9YCo_C4J4

[조금은 느리게 살자: 베르누이 수(Bernoulli Number) (ghebook.blogspot.com)](https://ghebook.blogspot.com/2020/07/bernoulli-number.html)

[Sums of Powers (mathpages.com)](https://www.mathpages.com/home/kmath279/kmath279.htm)