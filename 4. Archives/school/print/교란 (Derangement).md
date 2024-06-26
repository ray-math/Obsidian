```tikz
\begin{document}
\begin{tikzpicture}
  % Ellipse for Set X
  \draw (0,0) ellipse (1cm and 2cm);
  \node at (0,2.2) {$X$};
  \draw (3,0) ellipse (1cm and 2cm);
  \node at (3,2.2) {$Y$};
  \node at (1.5,2.5) {$f$};

  % Nodes for elements of set X
  \node (x1) at (0,1.5) {1};
  \node (x2) at (0,1) {2};
  \node (x3) at (0,0.5) {3};
  \node (x4) at (0,0) {$\vdots$};
  \node (x5) at (0,-0.5) {$x$};
  \node (x6) at (0,-1) {$\vdots$};
  \node (x7) at (0,-1.5) {$n$};
  

  % Nodes for elements of set Y
  \node (y1) at (3,1.5) {1};
  \node (y2) at (3,1) {2};
  \node (y3) at (3,0.5) {3};
  \node (y4) at (3,0) {$\vdots$};
  \node (y5) at (3,-0.5) {$x$};
  \node (y6) at (3,-1) {$\vdots$};
  \node (y7) at (3,-1.5) {$n$};

  % Arrows
  \draw[->] (0.5,2.2) -- (2.5,2.2);
  \draw[->] (x1) -- (y2);
  \draw[->] (x2) -- (y3);
  \draw[->] (x3) -- (y4);
  \draw[->] (x4) -- (y5);
  \draw[->] (x5) -- (y6);
  \draw[->] (x6) -- (y7);
  \draw[->] (x7) -- (y1);
  
\end{tikzpicture}
\end{document}
```

학생이 시험을 치른 후 자신의 시험지가 아닌 서로의 시험지를 채점해 주는 경우의 수는 어떻게 될까? 이는 앞선 그림과 같이 일대일 대응 함수 중 고정점이 없는 함수의 개수와 같다. 즉, $f:X \rightarrow X$, $f(x) \not= x$인 일대일 대응 함수이다. 이는 모든 원소의 위치를 바꾸는 순열과 같아 ‘완전 순열’ 또는 ‘교란’이라 부른다. 기호는 $!n$라 적고, n subfactorial이라 읽는다.

```tikz
\begin{document}
\begin{tikzpicture}
  % Ellipse for Set X
  \draw (0,0) ellipse (1cm and 2cm);
  \node at (0,2.2) {$X$};
  \draw (3,0) ellipse (1cm and 2cm);
  \node at (3,2.2) {$Y$};
  \node at (1.5,2.5) {$f$};

  % Nodes for elements of set X
  \node (x1) at (0,1.5) {1};
  \node (x2) at (0,1) {2};
  \node (x3) at (0,0.5) {3};
  \node (x4) at (0,0) {$\vdots$};
  \node (x5) at (0,-0.5) {$x$};
  \node (x6) at (0,-1) {$\vdots$};
  \node (x7) at (0,-1.5) {$n$};
  

  % Nodes for elements of set Y
  \node (y1) at (3,1.5) {1};
  \node (y2) at (3,1) {2};
  \node (y3) at (3,0.5) {3};
  \node (y4) at (3,0) {$\vdots$};
  \node (y5) at (3,-0.5) {$x$};
  \node (y6) at (3,-1) {$\vdots$};
  \node (y7) at (3,-1.5) {$n$};

  % Arrows
  \draw[->] (0.5,2.2) -- (2.5,2.2);
  \draw[->,blue,line width=1] (x1) -- (y5);
  \draw[->, teal,line width=1] (x5) -- (y7);
  
  \draw[orange, line width=1pt, rounded corners=1pt] (-0.4,1.2) rectangle (0.4,-1.7);
  \node[orange, left] at (-0.5,0) {$!(n-1)$};

\begin{scope}[shift={(8,0)}]
 \draw (0,0) ellipse (1cm and 2cm);
  \node at (0,2.2) {$X$};
  \draw (3,0) ellipse (1cm and 2cm);
  \node at (3,2.2) {$Y$};
  \node at (1.5,2.5) {$f$};

  % Nodes for elements of set X
  \node (x1) at (0,1.5) {1};
  \node (x2) at (0,1) {2};
  \node (x3) at (0,0.5) {3};
  \node (x4) at (0,0) {$\vdots$};
  \node (x5) at (0,-0.5) {$x$};
  \node (x6) at (0,-1) {$\vdots$};
  \node (x7) at (0,-1.5) {$n$};
  

  % Nodes for elements of set Y
  \node (y1) at (3,1.5) {1};
  \node (y2) at (3,1) {2};
  \node (y3) at (3,0.5) {3};
  \node (y4) at (3,0) {$\vdots$};
  \node (y5) at (3,-0.5) {$x$};
  \node (y6) at (3,-1) {$\vdots$};
  \node (y7) at (3,-1.5) {$n$};

  % Arrows
  \draw[->] (0.5,2.2) -- (2.5,2.2);
  \draw[->,blue, line width=1] (x1) -- (y5);
  \draw[->, teal, line width=1] (x5) -- (y1);
  
  \draw[orange, line width=1pt, rounded corners=1pt] (-0.4,1.2) rectangle (0.4,-0.3);
  \draw[orange, line width=1pt, rounded corners=1pt] (-0.4,-0.7) rectangle (0.4,-1.7);
  \node[orange, left] at (-0.5,0) {$!(n-2)$};
\end{scope}
  
\end{tikzpicture}
\end{document}
```

- 우선 $f(1)=x$라 하면, $x \not= 1$이다. 따라서 $x$가 될 수 있는 원소의 수는 총 $n-1$이다.
- $f(x) \not=1$이라면 $1$을 제외한 $n-1$개의 원소들이 완전순열을 이루어야 하므로 경우의 수는 $!(n-1)$이다.(남은 정의역의 원소는 $2$부터 $x$까지 $n-1$개이고, 치역의 원소는 $1$부터 $n$까지 중에 $x$를 뺀 $n-1$개다. 이때, $x$는 $1$을 선택하지 못하고 나머지 원소도 자신을 선택하지 못하므로 결국 원소의 개수가 $n-1$인 완전순열을 이룬다.)
- $f(x)=1$이라 하면 $1$과 $x$를 제외한 남은 $n-2$개의 원소들의 완전순열은 $!(n-2)$이다.

따라서 교란은 아래와 같이 귀납적으로 정의할 수 있다. 또는 포함배제의 원리에 의해 같은 값을 유도하는 식을 얻을 수도 있다.

>[!note]
>$${!n} = (n - 1) \times \left( !(n - 1) + !(n - 2) \right) = n! \sum_{i=0}^{n} \frac{(-1)^i}{i!}$$

일반적인 고등학교 수준의 문제에서는 고정점이 $5$개 이상이 나오는 경우는 거의 없어 위의 식보다는 차라리 $!0$부터 $!4$까지의 값을 외우고 있는 것이 좋다.

$$\begin{array}{*{5}{c}}
!0=1 & !1=0 & !2=1 & !3 = 2 & !4 =9 & !5=44 & !6=265 & !7 = 1854
\end{array}$$
