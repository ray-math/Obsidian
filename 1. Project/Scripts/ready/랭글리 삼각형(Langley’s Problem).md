---
tags:
  - 기하
---
랭글리의 도형문제는 기하학적 도형에서 주어진 각도들로부터 다른 각도를 추론하는 퍼즐입니다. 1922년 에드워드 맨 랭글리에 의해 'The Mathematical Gazette'에 처음 제시된 문제는
다음과 같습니다

- 삼각형 ABC는 이등변삼각형인데, $\angle CBA = \angle ACB = 80^\circ$ 입니다.
- CF는 AC에 대해 $30^\circ$로 AB를 F에서 만납니다.
- BE는 AB에 대해 $20^\circ$로 AC를 E에서 만납니다.
- 증명해야 할 것은 $\angle BEF = 30^\circ$ 입니다.

얼핏보면 몇개의 보조선을 그리면 풀 수 있을 것 같습니다. 하지만 실제로 풀어보려하면 꽤나 어렵습니다. 여러가지 풀이가 있지만 가장 일반적으로 알려진 풀이를 같이 보도록 하겠습니다.

1. BG를 BC에 대해 $20^\circ$로 그리고 AC와 G에서 만납니다.
2. $\angle BCG = 80^\circ$와 $\angle CBG = 20^\circ$이므로 $\angle BGC = 80^\circ$이고 삼각형 BCG는 이등변삼각형이며 BC = BG입니다.
3. $\angle BCF = 50^\circ$와 $\angle CBF = 80^\circ$이므로 $\angle BFC = 50^\circ$이고 삼각형 BCF도 이등변삼각형이며 BC = BF입니다.
4. $\angle FBG = 60^\circ$이고 BF = BG이므로 삼각형 BGF는 정삼각형입니다.
5. $\angle BGE = 100^\circ$와 $\angle GBE = 40^\circ$이므로 $\angle GEB = 40^\circ$이고 삼각형 BGE도 이등변삼각형이며 GB = GE입니다.
6. 따라서 그림의 모든 빨간 선은 같은 길이를 가집니다.
7. GE = GF이므로 삼각형 EFG는 이등변삼각형이고 $\angle GEF = 70^\circ$입니다.
8. 따라서 $\angle BEF = 30^\circ$입니다.

