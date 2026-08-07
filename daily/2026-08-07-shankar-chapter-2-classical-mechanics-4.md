---
title: "Shankar Chapter 2 — Classical Mechanics 복습 및 이해 점검"
created: 2026-08-07
updated: 2026-08-07
tags: [learning]
source: "학습 세션 → Issue #13 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: GPT-5.6 Sol
source_issue: 13
---

# Shankar Chapter 2 — Classical Mechanics 복습 및 이해 점검

## 오늘 직접 학습한 지식

양자역학을 다음 교재와 강의록을 활용하여 천천히 공부하고 싶어. 현재는 아직 Shankar 교재 기준 chapter 2의 Lagrangian에 대한 내용까지 학습을 진행했고, 이전 내용을 완벽하게 이해했는지는 불확실해. 일단 지금 보고 있는 내용인 chapter2의 classical mechanics에 대한 내용부터 시작해보고 싶어.

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

## 취약 영역

- 처음에는 L을 경로 전체의 함수로 잘못 표현했으나 이후 L은 x, x', t의 function이고 S가 경로 x(t)의 functional임을 바로잡음
- stationary action을 minimum으로 표현하는 습관이 있어 extremum/stationary와 minimum의 차이를 계속 점검할 필요가 있음
- Euler-Lagrange equation을 L=T-V에 대입할 때 potential 항의 부호를 한 번 놓침
- 극좌표에서 p_theta 계산 시 r^2 계수를 놓침

## 다음 복습 질문

- Newtonian mechanics의 local 관점과 Lagrangian mechanics의 global 관점을 자기 말로 설명하라.
- 왜 L은 function이고 S는 functional인가?
- 왜 variation η(t)는 양 끝점에서 0이어야 하는가?
- 왜 임의의 η(t)에 대해 ∫f(t)η(t)dt=0이면 f(t)=0이어야 하는가?
- L=(1/2)m x_dot^2 - V(x)에서 Euler-Lagrange equation이 Newton의 제2법칙을 어떻게 복원하는가?
- generalized coordinate q에 대한 canonical momentum p_q는 왜 항상 일반적인 선운동량이 아닌가?
- 극좌표 L=(1/2)m(r_dot^2+r^2 theta_dot^2)-V(r)에서 p_theta를 계산하고 theta가 cyclic coordinate일 때 무엇이 보존되는지 설명하라.

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
