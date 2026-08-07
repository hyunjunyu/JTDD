---
title: "학습 상태 — 러너 진입점"
updated: 2026-08-07
kind: status
---

# 🎯 학습 상태 (Runner Entrypoint)

> **"오늘 세션 시작"을 누르면 러너(Custom GPT)가 가장 먼저 읽는 한 파일.**
> 여기서 현재 위치를 잡고 시작한다 — 전체를 스캔하지 않는다.
> **작게 유지한다** — 전체 목록(약점·복습·개념)은 `mastery.md`·`daily/`에 두고, 여기엔 **지금 초점만**.
> 세션이 끝나면 러너가 이 파일을 갱신한다(아래 §쓰기 계약).

<!-- 처음 시작할 때: 아래 <...> 를 내 목표로 바꾸면 된다. 러너에게 "새 목표 세우기"라고 해도 된다. -->

## 지금 활성 트랙

| 트랙 | 목표 (끝나면 무엇을 스스로 설명/수행할 수 있나) | 모드 |
|---|---|---|
| **<트랙 이름 — 예: "딥러닝 복원" / "SSL 랩 컨택 준비">** | <목표 한 줄> | <진도 / 복원 / 논문> |

> 📌 **정해진 날짜(시험 등)가 있으면만** 여기 적는다. 없으면 비워 둔다 —
> 이 시스템은 일정표가 아니라 **오늘 15~60분**을 굴리는 도구다.

> **모드**: `진도`(지금 듣는 과목 — 주차·시험 기준) · `복원`(들었는데 기억 안 나는 과목 — 스캔부터) · `논문`(논문·랩·교수)

## 🎯 오늘의 추천 목표 — 오늘 할 것 (15~60분)

- <오늘 무엇을 이해할 것인가 — 러너가 채워줌. 처음엔 "기초부터 시작"이라고 둬도 됨>

## 지금 약한 것 (top 5 — 세션은 여기서 시작)
> 전체는 [[mastery.md]]. 아직 `설명가능`이 아닌 것부터.
1. 처음에는 L을 경로 전체의 함수로 잘못 표현했으나 이후 L은 x, x', t의 function이고 S가 경로 x(t)의 functional임을 바로잡음
2. stationary action을 minimum으로 표현하는 습관이 있어 extremum/stationary와 minimum의 차이를 계속 점검할 필요가 있음
3. Euler-Lagrange equation을 L=T-V에 대입할 때 potential 항의 부호를 한 번 놓침
4. 극좌표에서 p_theta 계산 시 r^2 계수를 놓침
5. L과 S의 역할을 처음에는 혼동했으나, L은 x, x', t의 function이고 S는 경로 x(t)의 functional이라는 구분으로 교정함.

## 다음 복습 질문 (top 5 — 세션 시작 시 1~2개 예측용)
> 다음 세션에서 다시 물을 것. 러너가 채워 나간다.
1. Newtonian mechanics의 local 관점과 Lagrangian mechanics의 global 관점을 자기 말로 설명하라.
2. 왜 L은 function이고 S는 functional인가?
3. 왜 variation η(t)는 양 끝점에서 0이어야 하는가?
4. 왜 임의의 η(t)에 대해 ∫f(t)η(t)dt=0이면 f(t)=0이어야 하는가?
5. L=(1/2)m x_dot^2 - V(x)에서 Euler-Lagrange equation이 Newton의 제2법칙을 어떻게 복원하는가?

## 최근 궤적 (러너가 갱신)

- 2026-08-07 · 양자역학 Chapter 2 — Newtonian vs Lagrangian → [daily/2026-08-07-chapter-2-newtonian-vs-lagrangian.md](daily/2026-08-07-chapter-2-newtonian-vs-lagrangian.md)
- 2026-08-07 · 양자역학 Chapter 2 — Classical Mechanics → [daily/2026-08-07-chapter-2-classical-mechanics.md](daily/2026-08-07-chapter-2-classical-mechanics.md)
- 2026-08-07 · 양자역학 Chapter 2 — Classical Mechanics / Lagrangian → [daily/2026-08-07-chapter-2-classical-mechanics-lagrangian.md](daily/2026-08-07-chapter-2-classical-mechanics-lagrangian.md)
- 2026-08-07 · 양자역학 Chapter 2 — Lagrangian mechanics → [daily/2026-08-07-chapter-2-lagrangian-mechanics-4.md](daily/2026-08-07-chapter-2-lagrangian-mechanics-4.md)
- 2026-08-07 · Shankar Chapter 2 Classical Mechanics → [daily/2026-08-07-shankar-chapter-2-classical-mechanics-2.md](daily/2026-08-07-shankar-chapter-2-classical-mechanics-2.md)
- 2026-08-07 · Shankar Chapter 2 Classical Mechanics - Lagrangian → [daily/2026-08-07-shankar-chapter-2-classical-mechanics-lagrangian.md](daily/2026-08-07-shankar-chapter-2-classical-mechanics-lagrangian.md)
- 2026-08-07 · Shankar Chapter 2 — Classical Mechanics 복습 및 이해 점검 → [daily/2026-08-07-shankar-chapter-2-classical-mechanics-4.md](daily/2026-08-07-shankar-chapter-2-classical-mechanics-4.md)

## 세션 진행 프로토콜 (러너가 따르는 대본)
**① 목표 → ② 예측(내가 먼저 자기 말로) → ③ 설명·교정(오개념을 근거와 함께) → ④ 퀴즈/적용 → ⑤ 채점·기록.**
떠먹여주지 않는다. 내가 먼저 설명하게 하고, 약한 고리를 근거와 함께 짚는다.

## 쓰기 계약 (세션 종료 시 러너가 하는 일)
1. `daily/YYYY-MM-DD-<주제>.md` 생성 — `templates/session-card.md` 형식, **정규 헤딩 준수**(`## 오늘 직접 학습한 지식` / `## 취약 영역` / `## 다음 복습 질문`).
2. 이해 승급이 있으면 `mastery.md`에 한 줄 append — `설명가능`은 **반박 통과 + 증거(오늘 daily 링크)** 있을 때만.
3. **이 STATUS.md 갱신** — 작게: 오늘 목표·top5 약점·top5 복습·최근 궤적 한 줄. (전체는 mastery/daily에, 여기엔 초점만.)
