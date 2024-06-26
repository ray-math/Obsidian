>[!tip]  그래프를 그리기 전에
>- $x$축을 그린다 $\Rightarrow$ 개형을 그린다 $\Rightarrow$ 점을 찍는다
>- $y$축은 필요할 때만 그린다. (때에 따라 $x$축 또한 생략한다.)
>- $f$의 최고차항의 계수와 차수가 개형을 결정한다.
>- $f'>0$이면 $f$는 증가하고, $f'<0$이면 $f$는 감소한다.
>- $f'=0$이면 $f$는 평평하다. 즉, 봉우리가 생길 가능성이 높다.
>- $f''>0$이면 $f$는 아래로 볼록, $f''<0$이면 $f$는 위로 볼록이다.
>- 대칭성(우함수, 기함수, 선대칭, 점대칭)과 주기성을 고려한다.
>- 

```tikz
\begin{document}
\begin{tikzpicture}[scale=1.2]
	%1
    \draw[-latex] (-1.5,0) -- (3,0) node[right] {$x$};
    \draw[-latex, dotted, line width=1pt] (0,-1.3) -- (0,1.7) node[above] {$y$};
    
    \draw[smooth, line width=1.5pt] plot[domain=-0.6:2.6] (\x,{(\x)^2*(\x-2)^2-1});
    
	\node at (-0.41,-0.3) [left] {$1-\sqrt2$};
	\node at (1,-0.1) [below] {$1$};
	\node at (2.41,-0.3) [right] {$1+\sqrt2$};

	\fill (-0.41,0) circle (1.5pt);
	\fill (1,0) circle (1.5pt);
	\fill (2.41,0) circle (1.5pt);

	%2
	\begin{scope}[shift={(5,0)}]

    \draw[-latex,dotted,line width=1pt] (-1.5,2) -- (3,2) node[right] {$x$};
    
    \draw[smooth, orange, dotted, line width=1.5pt] plot[domain=-0.1:2.1] (\x,{4*\x*(\x-1)*(\x-2)+2});
    \draw[smooth, line width=1.5pt] plot[domain=-0.6:2.6] (\x,{(\x)^2*(\x-2)^2-1});
    
	\node[orange] at (0,1.7) [left] {$0$};
	\node[orange] at (0.9,1.9) [below] {$1$};
	\node[orange] at (2,1.7) [right] {$2$};
	\node at (2.1,3) [right, orange] {$f'(x)$};

	\fill[orange] (0,2) circle (1.5pt);
	\fill[orange] (1,2) circle (1.5pt);
	\fill[orange] (2,2) circle (1.5pt);

	\fill (0,-1) circle (1.5pt);
	\fill (1,0) circle (1.5pt);
	\fill (2,-1) circle (1.5pt);

	\draw[dashed] (0,2) -- (0,-1);
	\draw[dashed] (1,2) -- (1,0);
	\draw[dashed] (2,2) -- (2,-1);

	\end{scope}

	%3
	\begin{scope}[shift={(10,0)}]
	
	\draw[-latex] (-1.5,0) -- (3,0) node[right] {$x$};
    \draw[-latex] (0,-1.3) -- (0,1.7) node[above] {$y$};
    
    \draw[smooth, orange, line width=1.5pt, dotted] plot[domain=-0.6:2.6] (\x,{(\x)^2*(\x-2)^2});
    \draw[smooth, line width=1.5pt] plot[domain=-0.6:2.6] (\x,{(\x)^2*(\x-2)^2-1});
    
	\node[orange] at (0,-0.2) [left] {$0$};
	\node[orange] at (2.2,0) [below] {$2$};
	\node at (-0.2,-1) [left] {$-1$};

	\fill[orange] (0,0) circle (1.5pt);
	\fill[orange] (2,0) circle (1.5pt);
	\fill (0,-1) circle (1.5pt);
	
	\draw[dashed] (2,0) -- (2,-1);
	\draw[dashed] (0,-1) -- (2,-1);
	
	\end{scope}
	  
\end{tikzpicture}
\end{document}
```
#### 인수분해를 이용한 그래프 그리기
$f(x)=x^4 - 4x^3 + 4x^2 - 1 = (x-1)^2 (x-1+ \sqrt{2})(x-1- \sqrt{2})$이므로, $x=1$(중근), $x=1- \sqrt{2}$, $x=1+ \sqrt{2}$을 근으로 가진다. 따라서 $x=1$에서 $f(x)$의 그래프는 $x$축에 접하며, $x=1 \pm \sqrt{2}$에서는 근을 갖는 사차함수를 그린다.

#### 미분을 이용한 그래프 그리기
$f'(x) = 4x^3 - 12x^2 + 8x = 4x(x - 1)(x - 2)$이므로 $x=0$, $x=1$, $x=2$에서 근을 갖는 삼차함수를 그린다. **$f'=0$인 곳을 기준으로 $f'>0$이면 $f$가 증가(우상향)하도록, $f'<0$이면 $f$는 감소(우하향)하도록** 사차함수를 그린다.

#### 평행이동을 이용한 그래프 그리기
$f(x) = x^4 - 4x^3 + 4x^2 - 1 = x^2 (x - 2)^2 - 1$이므로, $x=0$, $x=2$에서 중근을 갖는 사차 함수를 그린 후, $y$축으로 $-1$만큼 평행이동 한다. **상수항은 함수의 그래프를 $y$축 방향으로 평행이동 시킬 뿐이다.**