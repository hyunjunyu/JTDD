---
title: "Shankar Chapter 2 — Lagrangian Mechanics에서 Symmetry와 Conservation까지"
created: 2026-08-07
updated: 2026-08-07
tags: [learning]
source: "학습 세션 → Issue #19 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: GPT-5.6 Sol
source_issue: 19
---

# Shankar Chapter 2 — Lagrangian Mechanics에서 Symmetry와 Conservation까지

## 오늘 직접 학습한 지식

1. 뉴턴 역학에서는 입자의 운동 경로를 global적인 관점보다는 순간. 특정 시점에 대한 해석으로 결정해. 뉴턴의 2법칙을 통해 x(t), x'(t)를 알고 있다면 x_cl(t+delta) = x(t) + x'(t)*delta와 같이 순간, 순간이 모여 이후의 경로가 정해진다는 느낌.
2. Lagrangian에서는 입자의 순간이 아닌, 입자의 전체 운동 경로를 기준으로 문제를 바라봐. x(t)를 한 시점, 한 시점을 따로 보는 것이 아니라, 경로의 시작부터 끝 전체를 기준으로 하는거지. 이때 라그랑지안에서 제시하는 새로운 물리량 L은 입자의 운동 경로 x(t)라는 함수에 대한 함수야. 라그랑지안 역학에서 유도되는 Euler-Lagrange equation을 통해, Cartesian이 아닌 다른 직교 좌표계에서 물체의 운동을 일반적으로 기술하는데 용이하지.

아이쿠 쓰다 보니까 요건 잘못 적었네 ㅇㅋㅇㅋ

L은 x, x', t에 대한 함수고 S는 x에 대한 함수이기에, L은 function, S는 functional이지 않아?

저 임의의 경로를 설정하는 이유가, 시작점과 도착점 자체는 동일하고, 그 입자의 운동하는 '경로'에서 변화가 발생했을 때 생기는 action 값이 minimum인 점을 찾고 싶기 때문에 그렇게 놓은 것으로 이해했어.

x'가 어떻게 바뀌는지..?는 잘 모르겠네. 근데 S[x+e]를 유도하는 과정에서 피적분식이 L(x,x')과 (dL/dx)*e+ (dL/dx')*e' + ... 로 테일러 전개되면서 S[x] + dS + HOT로 유도되는데, 이때 dS가 0이라는 전제 때문에 Euler-Lagrange eq가 유도되는 것으로 학습했어

너의 힌트에 답이 있네. η(t)를 그 어떤 함수로 잡아도, 즉 어떤 방식으로 기존 x를 흔들더라도 적분값이 0이 나와야 하기 때문에 모든 t에서 해당 함숫값이 0이 나와야하는거지

그대로 대입하면 d/dt(mx') - dV/dx = 0이라는 결과가 나오고, 이는 뉴턴 2법칙과 일치해

d/dt(mx') = -kx

일반적인 선운동량과 달라. q를 어떤 좌표계에 적용하는지에 따라 canonical momentum이 의미하는 물리량도 달라져. 일례로 theta를 q로 잡으면 p_q가 우리가 아는 각운동량으로 유도돼.

p_theta = mr(theta') 맞나?

각운동량 보존 법칙이 나오지. torque가 0일 때 p_theta가 보존된다는 내용

L이 theta에 대해 무관하다는 것은, 각에 따라 L값이 바뀌지 않는다는 rotational symmetry로 이어지고, 이러한 symmetry는 Euler-Lagrange equation에서 유도된 결과에 따라 p_theta의 보존으로 이어져.
이를 일반적으로 적용하여 특정 직교좌표계의 basis q_i에 대해 L이 대칭이라면, 이는 p_q_i의 보존으로 이어진다는 결과를 도출할 수 있을 것 같아

Cartesian에서 x,y가 cyclic이 아니더라도, Polar로 변환하면 theta가 cyclic coordinate가 되고, 아까 유도했던 방식 그대로 적용할 수 있기 때문에..? 일반화해서 설명하기 살짝 버겁네

## 취약 영역

- stationary action을 minimum과 구분해서 표현하기
- 경로 variation에서 x→x+εη일 때 xdot→xdot+εηdot 관계를 즉시 떠올리기
- L=T-V를 Euler–Lagrange 식에 넣을 때 potential 항의 부호 실수 줄이기
- 극좌표에서 p_theta=mr^2 theta_dot의 r^2 계수 정확히 기억하기
- generalized coordinate q_i를 basis 또는 직교좌표계에 한정하지 않고 이해하기
- cyclic coordinate가 continuous symmetry를 특정 좌표 하나에 드러낸 특수한 경우라는 점 일반화하기
- Cartesian 좌표에서 여러 coordinate가 함께 변하는 rotational symmetry와 conserved generator의 관계 이해하기
- Noether theorem의 일반형을 교재 §2.8과 연결해 스스로 설명하기

## 다음 복습 질문

- 왜 η(t_i)=η(t_f)=0이어야 하는가?
- 왜 모든 허용 가능한 η(t)에 대해 ∫f(t)η(t)dt=0이면 f(t)=0이어야 하는가?
- L=1/2 m xdot^2 - V(x)에서 Euler-Lagrange equation이 Newton의 제2법칙을 어떻게 복원하는가?
- 극좌표 중심력 문제에서 p_theta는 무엇이며 왜 보존되는가?
- L이 theta에 의존하지 않는다는 사실은 왜 rotational symmetry를 뜻하는가?
- cyclic coordinate q_i가 있으면 왜 conjugate momentum p_i가 보존되는가?
- Cartesian 좌표에서 x,y가 cyclic coordinate가 아니어도 rotational symmetry가 존재하는 이유는 무엇인가?
- polar 좌표에서 rotational symmetry가 theta의 cyclic coordinate 형태로 드러나는 이유는 무엇인가?
- Shankar §2.8에서 symmetry의 generator가 conserved quantity가 되는 논리를 설명할 수 있는가?

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
