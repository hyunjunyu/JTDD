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
1. Lagrangian L 자체와 action S의 입력 대상 구분은 스스로 바로잡음. S는 x라는 숫자가 아니라 경로 함수 x(t) 전체를 입력으로 받는 functional이라는 표현을 더 엄밀히 할 필요가 있음.
2. Euler-Lagrange 방정식의 좌표 일반성을 '다른 직교 좌표계'로 한정했으나, 실제로는 독립적인 generalized coordinates에 대해 같은 형태를 유지한다는 점을 보완해야 함.
3. principle of least action을 단순 minimum이 아니라 stationary action, 즉 1차 variation이 0인 조건으로 엄밀히 표현하는 부분을 계속 확인할 필요가 있음.
4. Lagrangian L은 function이고 action S[x(t)]가 functional이라는 구분은 교정 후 이해함.
5. Euler-Lagrange equation의 좌표 일반성은 직교 좌표계에만 제한되지 않고 독립적인 generalized coordinates에 대해 성립한다는 점을 더 익힐 필요가 있음.

## 다음 복습 질문 (top 5 — 세션 시작 시 1~2개 예측용)
> 다음 세션에서 다시 물을 것. 러너가 채워 나간다.
1. Newtonian mechanics가 local하고 Lagrangian mechanics가 global하다는 것은 정확히 무슨 뜻인가?
2. 왜 L은 function이고 S는 functional인가?
3. 왜 variation η(t)는 η(t_i)=η(t_f)=0이어야 하는가?
4. stationary action과 minimum action의 차이는 무엇인가?
5. x(t)→x(t)+εη(t)로 바꾸면 xdot과 L의 1차 변화는 어떻게 바뀌는가?

## 최근 궤적 (러너가 갱신)

---
- 2026-08-07 · 첫 실제 세션 시작 → [daily/2026-08-07-session.md](daily/2026-08-07-session.md)
- 2026-08-07 · Shankar Chapter 2 — Classical Mechanics 복습 및 이해 점검 → [daily/2026-08-07-shankar-chapter-2-classical-mechanics.md](daily/2026-08-07-shankar-chapter-2-classical-mechanics.md)
- 2026-08-07 · 양자역학 Chapter 2 — Newtonian vs Lagrangian → [daily/2026-08-07-chapter-2-newtonian-vs-lagrangian.md](daily/2026-08-07-chapter-2-newtonian-vs-lagrangian.md)
- 2026-08-07 · 양자역학 Chapter 2 — Classical Mechanics → [daily/2026-08-07-chapter-2-classical-mechanics.md](daily/2026-08-07-chapter-2-classical-mechanics.md)
- 2026-08-07 · 양자역학 Chapter 2 — Lagrangian mechanics → [daily/2026-08-07-chapter-2-lagrangian-mechanics.md](daily/2026-08-07-chapter-2-lagrangian-mechanics.md)
- 2026-08-07 · 양자역학 Chapter 2 — Classical Mechanics / Lagrangian → [daily/2026-08-07-chapter-2-classical-mechanics-lagrangian.md](daily/2026-08-07-chapter-2-classical-mechanics-lagrangian.md)

## 세션 진행 프로토콜 (러너가 따르는 대본)
**① 목표 → ② 예측(내가 먼저 자기 말로) → ③ 설명·교정(오개념을 근거와 함께) → ④ 퀴즈/적용 → ⑤ 채점·기록.**
떠먹여주지 않는다. 내가 먼저 설명하게 하고, 약한 고리를 근거와 함께 짚는다.

## 쓰기 계약 (세션 종료 시 러너가 하는 일)
1. `daily/YYYY-MM-DD-<주제>.md` 생성 — `templates/session-card.md` 형식, **정규 헤딩 준수**(`## 오늘 직접 학습한 지식` / `## 취약 영역` / `## 다음 복습 질문`).
2. 이해 승급이 있으면 `mastery.md`에 한 줄 append — `설명가능`은 **반박 통과 + 증거(오늘 daily 링크)** 있을 때만.
3. **이 STATUS.md 갱신** — 작게: 오늘 목표·top5 약점·top5 복습·최근 궤적 한 줄. (전체는 mastery/daily에, 여기엔 초점만.)
