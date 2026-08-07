---
title: "양자역학 Chapter 2 — Classical Mechanics / Lagrangian"
created: 2026-08-07
updated: 2026-08-07
tags: [learning]
source: "학습 세션 → Issue #6 (수집기: ingest_learning_note.py)"
status: active
kind: mixed
runner: GPT-5.6 Sol
source_issue: 6
---

# 양자역학 Chapter 2 — Classical Mechanics / Lagrangian

## 오늘 직접 학습한 지식

1. 뉴턴 역학에서는 입자의 운동 경로를 global적인 관점보다는 순간. 특정 시점에 대한 해석으로 결정해. 뉴턴의 2법칙을 통해 x(t), x'(t)를 알고 있다면 x_cl(t+delta) = x(t) + x'(t)*delta와 같이 순간, 순간이 모여 이후의 경로가 정해진다는 느낌.
2. Lagrangian에서는 입자의 순간이 아닌, 입자의 전체 운동 경로를 기준으로 문제를 바라봐. x(t)를 한 시점, 한 시점을 따로 보는 것이 아니라, 경로의 시작부터 끝 전체를 기준으로 하는거지. 이때 라그랑지안에서 제시하는 새로운 물리량 L은 입자의 운동 경로 x(t)라는 함수에 대한 함수야. 라그랑지안 역학에서 유도되는 Euler-Lagrange equation을 통해, Cartesian이 아닌 다른 직교 좌표계에서 물체의 운동을 일반적으로 기술하는데 용이하지.

아이쿠 쓰다 보니까 요건 잘못 적었네 ㅇㅋㅇㅋ

L은 x, x', t에 대한 함수고 S는 x에 대한 함수이기에, L은 function, S는 functional이지 않아?

저 임의의 경로를 설정하는 이유가, 시작점과 도착점 자체는 동일하고, 그 입자의 운동하는 '경로'에서 변화가 발생했을 때 생기는 action 값이 minimum인 점을 찾고 싶기 때문에 그렇게 놓은 것으로 이해했어.

## 취약 영역

- Lagrangian L 자체와 action S의 입력 대상 구분은 스스로 바로잡음. S는 x라는 숫자가 아니라 경로 함수 x(t) 전체를 입력으로 받는 functional이라는 표현을 더 엄밀히 할 필요가 있음.
- Euler-Lagrange 방정식의 좌표 일반성을 '다른 직교 좌표계'로 한정했으나, 실제로는 독립적인 generalized coordinates에 대해 같은 형태를 유지한다는 점을 보완해야 함.
- principle of least action을 단순 minimum이 아니라 stationary action, 즉 1차 variation이 0인 조건으로 엄밀히 표현하는 부분을 계속 확인할 필요가 있음.

## 다음 복습 질문

- Newtonian mechanics가 local하고 Lagrangian mechanics가 global하다는 것은 정확히 무슨 뜻인가?
- 왜 L은 function이고 S는 functional인가?
- 왜 variation η(t)는 η(t_i)=η(t_f)=0이어야 하는가?
- stationary action과 minimum action의 차이는 무엇인가?
- x(t)→x(t)+εη(t)로 바꾸면 xdot과 L의 1차 변화는 어떻게 바뀌는가?

> ⚠️ 아래 헤딩은 수집기가 자동 보정했다 — 세션에 실제 기록이 없었다는 뜻이다.

## 현재 이해 수준
- (이번 세션 기록 없음)

## 미해결 질문
- (이번 세션 기록 없음)
