---
title: "Shankar Chapter 2 Classical Mechanics - Lagrangian"
created: 2026-08-07
updated: 2026-08-07
tags: [learning]
source: "학습 세션 → Issue #11 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: GPT-5.6 Sol
source_issue: 11
---

# Shankar Chapter 2 Classical Mechanics - Lagrangian

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

## 취약 영역

- L과 action S의 function/functional 구분은 교정 후 이해함. 정확한 표기는 S가 x라는 수가 아니라 경로 함수 x(t)를 입력받는 functional이라는 점.
- least action을 minimum으로 표현했으나 실제 조건은 stationary/extremum인 δS=0임.
- 일반화 좌표는 직교 좌표계로 제한되지 않음.
- Euler-Lagrange 식에 L=T-V를 대입할 때 ∂L/∂x=-dV/dx이므로 부호를 주의해야 함.

## 다음 복습 질문

- x→x+εη일 때 왜 x'→x'+εη'가 되는가?
- η(t_i)=η(t_f)=0이어야 하는 이유는 무엇인가?
- 왜 모든 허용 가능한 η(t)에 대해 ∫f(t)η(t)dt=0이면 f(t)=0이어야 하는가?
- L=1/2 m x'^2 - V(x)를 Euler-Lagrange equation에 넣어 Newton의 제2법칙을 유도해보라.
- 조화진동자 V=1/2 kx^2의 운동방정식을 Lagrangian으로부터 유도해보라.

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
