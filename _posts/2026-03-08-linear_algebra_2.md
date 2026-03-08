---
layout: single
title: "10. Vector Space"
categories: Math
tag: [Linear_Algebra]
toc: true
author_profile: false
sidebar:
  nav: "docs"
use_math: false
---
### Vector Space
Vector Space란 뒤에 따라올 8가지 조건을 만족하는 집입니다.<br>
하지만 이를 큰 틀에서 이해하자면 binary operation과 scalar multiplication이 잘 되는 집합 정도로 생각하면 좋을 것 같습니다.<br>

조금 더 자세하게 vector space의 정의를 살펴보면 다음과 같습니다.<br>
$V$는 공집합이 아닌 집합이고 $F$는 field일 때 $V$는 binary operation과 scalar multiplication을 가지고 있으며 아래 8가지 조건을 만족할 때 $F$-vector space라고 부르며 $(V, +, *)$이라고 표기합니다.

또한 vector space의 원소를 vector라고 합니다.

### Associativity(결합법칙)
$\forall v_1, v_2, v_3 \in V: (v_1 + v_2) + v_3 = v_1 + (v_2 + v_3)$

어떻게 생각하면 당연한 것을 이렇게 명시하는 이유는 binary operation은 두 개의 원소를 받아 한 원소로 대응시킨는 함수이기 때문에 3개의 원소를 받아 한 원소로 대응시키는 것은 다른 문제이므로 확실하게 집고 넘어가야 하기 때문입니다.

### Identity(항등원)
$\exist 0\in V : \forall v\in V, v+0 = 0+v = v$

여기서 주의할 점은 항등원 $0$은 모든 $V$의 원소와의 binary operation에서 $v$와 대응되게 해야한다는 점입니다.


### Inverse(역원)
$\forall v\in V,\exist v^{`}\in V: v + v^`= v^`+ v = 0$


### Commutativity(교환법칙)
$\forall v_1, v_2 \in V: v_1 + v_2 = v_2 + v_1$

이 부분도 당연하다고 생각할 수 있지만 +를 binary operation 관점으로 보면 당연하지 않습니다. $+(v_1, v_2), +(v_2, v_1)$은 입력 튜플이 다르기 때문입니다.


### Distributivity(분배법칙)
$a\in F, \forall v_1, v_2\in V: a(v_1 + v_2) = av_1 + av_2$

이 부분에서 $v_1, v_2$는 서로 binary operation을 수행하여 정의에 의해 $V$의 원소가 되고 그 원소와 field의 원소를 곱하면 scalar multiplication이 되면서 $V$의 원소가 된다. 

### Distributivity(분배법칙)
$a, b\in F, \forall v\in V: (a+b)v = av + bv$

해당 결과 또한 $V$의 원소가 된다.

### Distributivity(분배법칙)
$\forall v\in V, a, b \in F: (ab)v = a(bv)$

### Identity of Multiplitation
$\forall v\in V, 1* v = v$

여기서 1은 $v$를 곱해서 $v$를 출력해주는 것을 표현한 것이지 진짜 1은 아닙니다.
물론 실수 집합에서는 이 때 1이 진짜 1입니다.