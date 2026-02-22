---
layout: single
title: "9. Binary_Operation & Scalar_Multiplication."
categories: Math
tag: [Linear_Algebra]
toc: true
author_profile: false
sidebar:
  nav: "docs"
use_math: false
---

### Linear Algebra
<!-- 선으로 대신한다는 말을 조금 더 자세하게 하자면 우리 주위의 무언가를 수학의 관점으로 바라봤을 때 선형적인 것은 해석하거나 다룰때 큰 무리가 없지만,
선형적이지 않은 것들은 정보가 부족하기 때문에 해석하기 매우 어렵다.(이 때문에 선형적이지 않은 곡선 등을 선형적으로 이해하기 위해 미분이라는 것을 사용함, 또한 모든 것을 선형적으로 볼 수 있다면 딥러닝이 탄생하지 않았을거임.) -->
Algebra의 뜻을 검색해보면 "숫자 대신 문자(기호)를 사용하여 수의 성질, 관계, 계산 법칙을 연구하는 수학의 한 분야"라고 설명한다.<br>
 그럼 Linear Algebra는 당연하게 숫자 대신 선형을 이용하여 수의 성질, 관계, 계산 법칙을 연구하는 것으로 이해할 수 있다.<br>
이를 다른 말로 표현하면 집합 위에 선형연산(binary operation, scalar multiplication)을 주고 그 행동을 살펴보는 학문이라고도 생각할 수 있다.


### Binary Operation
Binary Operation의 큰 그림은 그냥 두 숫자끼리 연산을 한다는 것이다.(+, -, *, /...)<br>
하지만 두 수끼리 연산한다는 것을 더욱 깊이 파해쳐본다면 결국 두 개의 입력을 받아 한 개의 결과로 출력하는 함수라는 결론에 도달할 수 있다.

위 말을 수식으로 나타내면 다음과 같이 쓰고 binary operation on $A$라고 한다.<br>
A가 집합일 때, function * : $A\times A\rightarrow A$ (곱하기 기호는 cartesian product를 의미한다.)<br>

위 수식을 보았을 때 두 수의 연산을 정석으로 쓰려면 다음과 같이 작성해야 하지만 불편하고 많이 사용하기 때문에 단순화해서 작성한다.<br>
$*((a_1, a_2)) =: a_1 * a_2$

Note: 위 식을 보면 알 수 있듯 Binary Operation은 연산에 대해 닫혀있어야 한다. 즉 연산의 결과가 자신의 집합보다 크면 Binary Operation을 만족하지 않는다는 뜻이다.
예를들어 정수는 +, -, * 연산에 대해 닫혀있지만 / 연산에 대해서는 닫혀있지 않다. 따라서 나누기는 정수에서 Binary Operation이 될 수 없다.

### Scalar Multiplication
우선 Scalar가 무엇인지 살펴보자면 간단하게 숫자하나! 라고 생각할 수 있지만(틀리진 않음) 조금 더 엄밀히 집고 넘어가자면 field의 원소를 말한다.

field란 대수적 대상 중 사칙연산을 잘 수행할 수 있는 공간(유리수, 실수, 복소수)을 말하며 사칙연산에 대해 닫혀있다는 특징있다.<br>

즉, Scalar는 field의 원소를 말하므로 유리수, 실수, 복소수 집합 중 하나 이상에 속한다.<br>
그럼 이제 Scalar Multiplication을 이해할 수 있는데 집합에 scalar를 곱한다고 생각할 수 있다.<br>

식은 다음과 같고 이 때 $F-$ scalar multiplication on A라고 한다.<br>
Let A be a set, function *: $F\times A\rightarrow A$.