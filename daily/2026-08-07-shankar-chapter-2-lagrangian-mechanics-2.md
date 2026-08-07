---
title: "Shankar Chapter 2 — Lagrangian Mechanics 개념 지도 반영"
created: 2026-08-07
updated: 2026-08-07
tags: [learning]
source: "학습 세션 → Issue #16 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: GPT-5.6 Sol
source_issue: 16
---

# Shankar Chapter 2 — Lagrangian Mechanics 개념 지도 반영

## 오늘 직접 학습한 지식

L은 x, x', t에 대한 함수고 S는 x에 대한 함수이기에, L은 function, S는 functional이지 않아?

저 임의의 경로를 설정하는 이유가, 시작점과 도착점 자체는 동일하고, 그 입자의 운동하는 '경로'에서 변화가 발생했을 때 생기는 action 값이 minimum인 점을 찾고 싶기 때문에 그렇게 놓은 것으로 이해했어.

x'가 어떻게 바뀌는지..?는 잘 모르겠네. 근데 S[x+e]를 유도하는 과정에서 피적분식이 L(x,x')과 (dL/dx)\**e+ (dL/dx')\**e' + ... 로 테일러 전개되면서 S[x] + dS + HOT로 유도되는데, 이때 dS가 0이라는 전제 때문에 Euler-Lagrange eq가 유도되는 것으로 학습했어

너의 힌트에 답이 있네. η(t)를 그 어떤 함수로 잡아도, 즉 어떤 방식으로 기존 x를 흔들더라도 적분값이 0이 나와야 하기 때문에 모든 t에서 해당 함숫값이 0이 나와야하는거지

그대로 대입하면 d/dt(mx') - dV/dx = 0이라는 결과가 나오고, 이는 뉴턴 2법칙과 일치해

d/dt(mx') = -kx

일반적인 선운동량과 달라. q를 어떤 좌표계에 적용하는지에 따라 canonical momentum이 의미하는 물리량도 달라져. 일례로 theta를 q로 잡으면 p_q가 우리가 아는 각운동량으로 유도돼.

p_theta = mr(theta') 맞나?

각운동량 보존 법칙이 나오지. torque가 0일 때 p_theta가 보존된다는 내용

## 취약 영역

- stationary action을 minimum과 구분해서 표현하기
- 경로 variation에서 x→x+εη일 때 xdot→xdot+εηdot 관계를 즉시 떠올리기
- L=T-V를 Euler–Lagrange 식에 넣을 때 potential 항의 부호 실수 줄이기
- 극좌표에서 p_theta=mr^2 theta_dot의 r^2 계수 정확히 기억하기
- cyclic coordinate와 symmetry, conservation law의 연결을 Noether theorem 관점으로 확장하기

## 다음 복습 질문

- 왜 η(t_i)=η(t_f)=0이어야 하는가?
- 왜 모든 허용 가능한 η(t)에 대해 ∫f(t)η(t)dt=0이면 f(t)=0이어야 하는가?
- L=1/2 m xdot^2 - V(x)에서 Euler–Lagrange equation이 Newton의 제2법칙을 어떻게 복원하는가?
- 극좌표 중심력 문제에서 p_theta는 무엇이며 왜 보존되는가?
- L이 theta에 의존하지 않는다는 사실을 rotational symmetry와 angular momentum conservation으로 어떻게 연결할 수 있는가?

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
