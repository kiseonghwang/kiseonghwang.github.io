---
layout: single
title: "11. Cancellation Law & Subspace"
categories: Math
tag: [Linear_Algebra]
toc: true
author_profile: false
sidebar:
  nav: "docs"
use_math: false
---

### Cancellation Law
Cancellation Law는 우리가 흔히 사용했던 빕칙 중 하나와 매우 닮아있습니다.

정의: Let $V$ be a vector space and let $v, w, u \sub V$ be given. Then $v + w = v + u \Rightarrow w = u$

증명) Let $v` \sub V$ a inverse of $v$ be given. Then $v + v` + w = v + v` + u \Rightarrow w = u$

Vector space에서 identity과 inverse은 오직 하나만 존재하는데 이는 수학에서 하나만 있음을 보일 때 사용하는 방법인 2개가 있다고 가정하고 그 2개가 사실 1개였음을 보이는 방법으로 증명할 수 있습니다.

다음 증명은 Identity가 2개 $(0, 0`)$ 있다고 했을 때 두 identity가 같음을 보입니다.
<br>
<br>
증명 1) $0 + v = v = 0` + v \Rightarrow 0 = 0`$  by the cancellation law

혹은 다음과 같이 증명할 수 있습니다. 

증명 2) $0 = 0 + 0`= 0`$

### Subspace
Set과 subset의 관계는 부분 관계라고 생각할 수 있지만 조금 더 생각해보면 subset은 set의 특징인 원소들을 모아두었다고 생각할 수 있습니다.
따라서 우리는 sub이라는 것을 부분인데 특징을 가져온 부분이라고 이해할 수 있습니다.

vector space의 특징은 3가지로 집합, linear operation, 8가지 조건입니다.
따라서 subspace는 vector space의 특징인 linear operation과 8가지 조건을 만족하면서 subset인 경우 해당 vector space의 subspace라고 부릅니다.

정의는 다음과 같습니다.

정의) $(V, +, *) : \text{F-vector space}, \empty \not= W \sub V, (W, +, *) : \text{F-vector space}$
이 때 vector space의 linear operation과 subspace의 linear operation이 다르다면 둘은 sub 관계가 아닙니다.