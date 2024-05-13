---
title: The Scandalous History of the Cubic Formula
source: https://www.quantamagazine.org/the-scandalous-history-of-the-cubic-formula-20220630/
clipped: 2023-10-05
tags:
  - 델페로
  - 타르탈리아
  - 카르다노
  - 아벨
  - 갈루아
---

History is full of backstabbing rivalries: Edison and Tesla, Harding and Kerrigan, Tupac and Biggie. No less dramatic was a 16th-century conflict between Italian mathematicians Gerolamo Cardano, a brilliant but troubled polymath, and Niccolò Fontana, better known as Tartaglia (meaning “the stammerer,” after a teenage facial injury from a French soldier’s sword). The central issue: cubic equations.

Most high school students know how to solve quadratic equations, such as $x^2-x-3=0$, using the quadratic formula. It states that the solutions, or roots, of $ax^2+bx+c=0$ are

$$x=\frac{-b \pm \sqrt{b^2-4ac}}{2a}$$

Are there similar formulas for equations of higher degree (having a larger power of *x*)? Determining this, in essence, was the task before Cardano, Tartaglia and their contemporaries.

Modern algebra as we know it — abstract symbolic expressions like those above and the familiar ways of manipulating them — dates to the 17th century, long after these scholars’ time. But algebraic thinking, and the ability to solve what we recognize as linear and quadratic equations, developed slowly over the preceding millennia.

In the 16th century, algebraic equations were still expressed rhetorically — in words, not symbols — and all coefficients had to be nonnegative, since mathematicians did not recognize negative numbers as legitimate. Without the notion of an unknown variable *x*, cubic equations of the form  $latexx^3+cx=d$ were instead described as “a cube and things equals a number,” and that was seen as different than “a cube equals things and a number,” $latexx^3=cx+d$. So while today we would view solving $latexax^3+bx^2+cx+d=0$ as one problem, at that time it was viewed as more than a dozen distinct problems, with the terms on one or the other side of the equal sign, or absent entirely.

Without modern symbolic algebra, mathematicians would reason geometrically. For instance, we can view the familiar expression $latex(a+b)^2=a^2+2ab+b^2$ as saying that the area of a square of side-length $latexa+b$  is the same as the sum of the areas of a square of side-length *a,* a square of side-length *b,* and two $latexa \\times b$ rectangles.

![Squares showing an equality between quadratic expressions](https://d2r55xnwy6nx47.cloudfront.net/uploads/2022/06/CUBIC_EQUATIONS3_Mobile.svg)

Merrill Sherman/Quanta Magazine

Likewise, decomposing a cube with side-length *t* into six boxes shows that

![](https://d2r55xnwy6nx47.cloudfront.net/uploads/2022/06/Screen-Shot-2022-06-30-at-10.22.57-AM.png)

(as long as $latext>u$).

![Cubes showing an equality between cubic expressions](https://d2r55xnwy6nx47.cloudfront.net/uploads/2022/06/CUBIC_EQUATIONS2_Mobile_cube.svg)

Merrill Sherman/Quanta Magazine

Scipione del Ferro, a professor at the University of Bologna in the early 16th century, was first to make significant headway into solving cubic equations. Unfortunately, we do not know all his accomplishments, thanks to a curious culture of academic secrecy at the time. Rather than racing to publish their work and basking in the recognition of proving a theorem or solving a problem, scholars would challenge each other to “mathematical duels.” They would send each other challenging problems, and the one who solved the most was the winner. The victors often garnered professional advancement and more students. Thus, discoveries would sometimes be held in reserve, secret weapons to be deployed in future contests.

But we do know del Ferro could solve equations of the form $latexx^3+cx=d$, when *c* and *d* are positive. A cubic equation with no squared term, such as this one, is called a “depressed cubic.” Although no 16th-century mathematician would express it this way, del Ferro showed that one root is

![](https://d2r55xnwy6nx47.cloudfront.net/uploads/2022/06/Screen-Shot-2022-06-30-at-10.23.12-AM.png)

This modern formula applies to any depressed cubic, but because cubic equations with different signs on the coefficients were considered different problems, del Ferro’s solution did not automatically carry over to other depressed cubics. We only know del Ferro could solve these cubics because he taught the technique to his student Antonio Fior, who bragged that he could solve such equations after del Ferro’s death.

Meanwhile, the self-taught Tartaglia discovered how to solve a different form of the cubic — one missing the linear term, *cx*. This set the stage for a mathematical duel between Fior and Tartaglia. In 1535, they exchanged 30 problems with a deadline of a month and a half. Tartaglia sent Fior a variety of problems, whereas the mathematically weaker Fior employed the “all eggs in one basket” strategy and sent Tartaglia 30 depressed cubics. Just days before the deadline, Tartaglia figured out how to solve them, and in two hours finished all 30. Fior, meanwhile, solved none of his problems. News spread throughout Italy of Tartaglia’s achievement, and Fior, humiliated, faded from view.

The prevailing wisdom was that solving the cubic was impossible, so Tartaglia’s accomplishment shocked Cardano. At this time, Cardano was a highly sought physician but cantankerous, beset by trouble after trouble. He gambled, he struggled with misbehaving sons, he was jailed during the Inquisition and more. Yet he ended up making contributions in mathematics, medicine, philosophy, religion, music and physics. Decades later, Gottfried Leibniz wrote, “Cardano was a great man with all his faults; without them, he would have been incomparable.” His collected works fill 7,000 pages and include the first serious investigations of probability theory.

Cardano tried, and failed, to replicate Tartaglia’s success with the cubic, so he began a pressure campaign to convince Tartaglia to share his method, even promising a vow of secrecy:

> I swear to you by the Sacred Gospel, and on my faith as a gentleman, not only never to publish your discoveries, if you tell them to me, but I also promise and pledge my faith as a true Christian to put them down in cipher so that after my death no one shall be able to understand them.

Eventually, in 1539, Tartaglia relented and shared his technique for depressed cubics with Cardano, but he did not share the proof that it worked. For the clever Cardano, however, just knowing the method was enough to discover the underlying mathematics. Before long, Cardano could solve any depressed cubic. He then observed that substituting

$latexx=t-\\frac{b}{3a}$

into $latexax^3+bx^2+cx+d=0$ yields a depressed cubic with variable *t.* By solving this equation for *t* and plugging that back into the substitution formula, he could find *x.* Thus, Cardano was able to solve every cubic equation.

Despite his vow to Tartaglia, Cardano taught these results to his talented assistant Ludovico Ferrari. Although he began as Cardano’s servant, Ferrari eventually became Cardano’s mathematical equal. By helping Cardano with his work on the cubic, he became so algebraically adept that he discovered how to reduce any quartic equation (one of degree 4) to a cubic. Thus, Cardano and Ferrari could solve any equation of degree four or less.

Cardano recognized the importance of these accomplishments and desperately wanted to publish the results. But since they all grew from the seeds planted by Tartaglia, doing so would break his oath.

Then, on a trip to Bologna in 1543, Cardano saw in del Ferro’s notebooks that he had solved the depressed cubic before Tartaglia. In Cardano’s mind, this discovery freed him of his obligation to Tartaglia. Two years later, Cardano published *Ars Magna* (*Great Art*), which contained his and Ferrari’s work on cubic and quartic equations.

Tartaglia was livid, even though Cardano acknowledged his work in the book. Tartaglia accused Cardano of theft and of breaking a sacred vow. Cardano left the rebukes to his loyal attack dog, Ferrari. The acrimonious back-and-forth, in the form of public pamphlets, continued for many months, leading to a mathematical duel between Tartaglia and Ferrari and eventually a public debate in Ferrari’s hometown, Milan. Tartaglia would much rather have battled the esteemed Cardano, but Cardano refused. Details are scarce, but the debate went terribly for Tartaglia, especially with the raucous hometown crowd. The next day, when it was time to continue the debate, Tartaglia was nowhere to be found — he’d left Milan.

Ferrari was flooded with job offers, and Tartaglia’s reputation was ruined. Despite many notable accomplishments beyond those related to the cubic, Tartaglia died penniless and largely unknown, whereas Cardano achieved everlasting fame. Many argue that the publication of *Ars Magna* marked the beginning of modern mathematics*.*

Having conquered cubic and quartic equations, mathematicians wondered how high they could go. As it turned out, not very far.

The story of quintic equations (polynomials of degree 5) is also fascinating, and it has a shocking conclusion: In general, it is impossible to express the roots of $latexax^5+bx^4+cx^3+dx^2+ex+f=0$ in terms of *a*, *b*, *c*, *d*, *e* and *f* using only addition, subtraction, multiplication, division and *n*th roots. For instance, the polynomial $latexx^5-x+1$ has a root of approximately $latex–1.167304$, but the exact value is impossible to express with those tools.

Niels Abel gave the first full proof of this fact in 1824, nearly three centuries after *Ars Magna*. Then, in 1830, the 18-year-old political firebrand Évariste Galois extended this work by giving exact criteria for when a polynomial of any degree is solvable. Although Galois died two years later in a duel (one fought with guns, not mathematics), his contributions to mathematics were oversized.

These impossibility results were not the end of the story. Mathematicians still study polynomials, their roots and their properties. As but one example, a famous problem proposed by David Hilbert in 1900 is about the roots of seventh-degree polynomials. It was thought to have been resolved in the 1950s but is now [the subject of renewed interest](https://www.quantamagazine.org/mathematicians-resurrect-hilberts-13th-problem-20210114/). Presumably, modern mathematicians can make headway on the problem without re-creating the rivalry surrounding the cubic.

***Correction: July 1, 2022**  
An earlier version of this article incorrectly stated that a root of the polynomial $latex x^5-x+1$ is approximately $latex-1.67304$; the correct value is $latex-1.167304$.* Quanta *regrets the error.*


16세기 초, 볼로냐 대학의 교수였던 Scipione del Ferro는 3차 방정식을 풀기 위한 중요한 발전을 이루었습니다. 당시의 학계 문화가 꽤 특이했기 때문에 그의 모든 업적을 알 수는 없습니다. 학자들은 자신의 연구를 빠르게 출판하고 정리하거나 문제를 해결한 것에 대한 인정을 받는 대신, 서로를 '수학 결투'에 도전했습니다. 그들은 서로에게 도전적인 문제를 보내고, 더 많은 문제를 해결한 사람이 승자였습니다. 승자는 종종 진급과 더 많은 학생을 얻었습니다. 따라서 발견들은 때로는 미래의 대회에서 사용될 비밀 무기로 보관되기도 했습니다.

그러나 del Ferro가 $x^3+cx=d$ 형태의 방정식, 여기서 $c$와 $d$는 양수, 를 풀 수 있었다는 것은 알고 있습니다. 제곱 항이 없는 이러한 3차 방정식을 'depressed cubic'이라고 부릅니다. 16세기 수학자가 이렇게 표현하지는 않았지만, del Ferro는 하나의 근이 다음과 같다고 보였습니다.

$$x = \sqrt[3]{\frac{b}{2} + \sqrt{\frac{b^2}{4} + \frac{a^3}{27}}} + \sqrt[3]{\frac{b}{2} - \sqrt{\frac{b^2}{4} + \frac{a^3}{27}}}$$

이 현대적인 공식은 모든 depressed cubic에 적용됩니다. 그러나 계수의 부호가 다른 3차 방정식은 다른 문제로 간주되었기 때문에, del Ferro의 해법은 다른 depressed cubic에 자동으로 적용되지 않았습니다. 우리는 그가 이러한 3차 방정식을 풀 수 있었다는 것을 그의 학생 Antonio Fior로부터 알게 되었습니다. del Ferro의 죽음 후에 그는 이러한 방정식을 풀 수 있다고 자랑했습니다.

이러한 역사적인 이야기는 수학의 발전과 학계 문화에 대한 흥미로운 통찰을 제공합니다. 물론, 이러한 '수학 결투'는 오늘날의 학계에서는 상상하기 어려운 일이지만, 그것이 당시에 어떤 역할을 했는지를 이해하는 것은 매우 흥미롭습니다.

그러는 동안, 자가 교육을 받은 Tartaglia는 선형 항 $cx$가 빠진 다른 형태의 3차 방정식을 풀어내는 방법을 발견했습니다. 이로 인해 Fior와 Tartaglia 사이의 수학 결투가 시작되었습니다. 1535년에 그들은 한 달 반의 기한을 두고 30개의 문제를 교환했습니다. Tartaglia는 Fior에게 다양한 문제를 보냈고, 수학적으로 약한 Fior는 "all eggs in one basket" 전략을 사용하여 Tartaglia에게 30개의 depressed cubic 문제를 보냈습니다. 마감일 몇 일 전에 Tartaglia는 그 문제들을 어떻게 풀어야 하는지 깨달았고, 두 시간 만에 모든 문제를 완료했습니다. 한편 Fior는 그의 문제 중 어느 것도 풀지 못했습니다. Tartaglia의 성취가 이탈리아 전역에 퍼지면서, Fior는 굴욕을 당하고 사라졌습니다.

당시의 일반적인 지혜는 3차 방정식을 풀 수 없다고 믿어졌기 때문에, Tartaglia의 성취는 Cardano를 충격에 빠뜨렸습니다. 당시 Cardano는 매우 인기 있는 의사였지만, 성격이 까다롭고 여러 문제에 시달렸습니다. 그는 도박을 했고, 무례한 아들들과 싸웠으며, 신성재판에서도 감옥에 갇혔습니다. 그럼에도 불구하고 그는 수학, 의학, 철학, 종교, 음악, 물리학 등에서 기여를 했습니다. 수십 년 후에 Gottfried Leibniz는 "Cardano는 그의 모든 결점에도 불구하고 위대한 사람이었다. 그 결점이 없었다면 그는 비교할 수 없을 정도로 훌륭했을 것이다."라고 썼습니다. 그의 저작은 7,000 페이지에 달하며 확률 이론에 대한 첫 번째 심각한 조사를 포함하고 있습니다.

Cardano는 Tartaglia의 3차 방정식 성공을 복제하려고 시도했지만 실패했습니다. 그래서 그는 Tartaglia에게 그의 방법을 공유하도록 압박하기 시작했고, 심지어 비밀을 지키겠다고 약속하기까지 했습니다.

> 나는 너에게 신성한 복음서와 신사로서의 나의 신념을 두고 맹세한다. 만약 네가 그것을 나에게 알려준다면, 나는 그것을 공개하지 않을 것이며, 나는 그것을 암호로 적어 내 죽음 후에 아무도 이해할 수 없게 할 것이다.

결국 1539년에 Tartaglia는 Cardano에게 그의 depressed cubic에 대한 기술을 공유했지만, 그것이 작동한다는 증명은 공유하지 않았습니다. 그러나 똑똑한 Cardano에게는 그 방법을 알기만 해도 기초 수학을 발견하는 것에 충분했습니다. 곧 Cardano는 모든 depressed cubic을 풀 수 있었습니다. 그는 다음의 치환을 통해 이를 발견했습니다.

$$
x = t - \frac{b}{3a}
$$

이를 $ax^3 + bx^2 + cx + d = 0$에 대입하면 변수 $t$를 가진 depressed cubic이 나옵니다. 이 방정식을 $t$에 대해 풀고 그것을 다시 치환 공식에 대입하면 $x$를 찾을 수 있습니다. 따라서 Cardano는 모든 3차 방정식을 풀 수 있었습니다.

Tartaglia에게 약속했음에도 불구하고, Cardano는 이러한 결과를 그의 뛰어난 조수 Ludovico Ferrari에게 가르쳤습니다. 처음에는 Cardano의 하인으로 시작했지만, Ferrari는 결국 Cardano의 수학적 동등한 사람이 되었습니다. 3차 방정식에 대한 Cardano의 작업을 도와주면서, 그는 4차 방정식(차수가 4인 방정식)을 3차로 축소하는 방법을 발견할 정도로 대수학적으로 능숙해졌습니다. 따라서 Cardano와 Ferrari는 차수가 4 이하인 모든 방정식을 풀 수 있었습니다.

Cardano는 이러한 성취의 중요성을 인식하고 결과를 꼭 출판하고 싶어했습니다. 그러나 이 모든 것이 Tartaglia가 심은 씨앗에서 자란 것이기 때문에, 그렇게 하면 그의 맹세를 깨게 됩니다.

그러다가 1543년 볼로냐로 여행을 간 Cardano는 del Ferro의 노트에서 그가 Tartaglia보다 먼저 depressed cubic을 풀어냈다는 것을 발견했습니다. Cardano의 마음속에서 이러한 발견은 그를 Tartaglia에 대한 의무에서 해방시켰습니다. 두 년 후, Cardano는 그와 Ferrari의 3차와 4차 방정식에 대한 작업을 담은 _Ars Magna_(_Great Art_)를 출판했습니다.

Tartaglia는 분노했고, 책에서 그의 작업을 인정했음에도 불구하고 Cardano를 도둑질과 신성한 맹세를 깬 것으로 고발했습니다. Cardano는 그의 충실한 공격견인 Ferrari에게 비난을 맡겼습니다. 이러한 악의적인 대립은 공개된 팜플릿의 형태로 여러 달 동안 계속되었고, 결국 Tartaglia와 Ferrari 사이의 수학 결투와 Ferrari의 고향인 밀라노에서의 공개 토론으로 이어졌습니다. Tartaglia는 고명한 Cardano와 싸우고 싶었지만, Cardano는 거부했습니다. 자세한 내용은 부족하지만, 토론은 Tartaglia에게 끔찍하게 진행되었습니다, 특히 그의 고향의 시끄러운 관중 앞에서는 더욱 그랬습니다. 다음 날, 토론을 계속할 시간이 되었을 때, Tartaglia는 어디에도 없었습니다—그는 밀라노를 떠났습니다.

Ferrari는 일자리 제안으로 물처럼 쏟아졌고, Tartaglia의 명성은 망가졌습니다. 3차 방정식과 관련된 것 이상의 많은 주목할만한 업적에도 불구하고, Tartaglia는 무명하고 빈털터리로 죽었습니다. 반면에 Cardano는 영원한 명성을 얻었습니다. 많은 사람들이 _Ars Magna_의 출판이 현대 수학의 시작을 표시한다고 주장합니다.

3차와 4차 방정식을 정복한 후, 수학자들은 얼마나 더 높은 차수의 방정식을 풀 수 있을지 궁금해했습니다. 결과적으로, 그렇게 먼 것은 아니었습니다.

5차 방정식(차수가 5인 다항식)의 이야기도 흥미롭고, 놀라운 결론이 있습니다: 일반적으로 $ax^5+bx^4+cx^3+dx^2+ex+f=0$의 근을 $a, b, c, d, e, f$와 덧셈, 뺄셈, 곱셈, 나눗셈, $n$제곱근을 사용해서만 표현할 수 없습니다. 예를 들어, 다항식 $x^5-x+1$은 대략 $-1.167304$의 근을 가지지만, 그 정확한 값은 그러한 도구로 표현할 수 없습니다.

Niels Abel은 이 사실에 대한 첫 번째 완전한 증명을 1824년에 제공했고, 거의 3세기 후에 _Ars Magna_가 나온 후였습니다. 그리고 1830년에 18세의 정치적 활동가 Évariste Galois는 이 작업을 확장하여 어떤 차수의 다항식이 풀 수 있는지에 대한 정확한 기준을 제시했습니다. Galois는 두 년 후에 결투(총으로 싸운 것, 수학이 아님)에서 죽었지만, 그의 수학에 대한 기여는 엄청났습니다.