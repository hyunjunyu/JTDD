---
title: "이해도 원장 (Mastery Ledger)"
kind: mastery
---

# 이해도 원장 — "진짜 공부했다"의 증거

> 개념마다 상태를 추적한다. **상태가 아니라 변화로** 기록한다.
> 상태: `미학습` → `암기`(답은 아는데 스스로 설명 못 함) → `설명가능`(스스로 유도·설명함).
> **`설명가능`은 AI의 반박을 통과하고, 증거(그 세션의 daily 링크)가 있을 때만.** 증거 없는 `설명가능`은 자기기만이다.
>
> ⚙️ 아래 표는 **자동 관리된다** — 세션에서 승급이 나오면 CI가 여기에 접어 넣는다.
> 손으로 고쳐도 되지만, `MASTERY-TABLE` 마커는 지우지 말 것(지우면 자동 갱신이 멈춘다).

<!-- MASTERY-TABLE:START -->
| 개념 | 상태 | 중요도 | 최근 검증일 | 증거(daily 세션) | 변화 메모(무엇이·왜 바뀌었나) |
|---|---|---|---|---|---|
| lagrangian-vs-action-function-functional | can_explain | L은 x, x', t에 대한 함수고 S는 x에 대한 함수이기에, L은 function, S는 functional이지 않아? |  |  |  |
| fixed-endpoint-variation | can_explain | 저 임의의 경로를 설정하는 이유가, 시작점과 도착점 자체는 동일하고, 그 입자의 운동하는 '경로'에서 변화가 발생했을 때 생기는 action 값이 minimum인 점을 찾고 싶기 때문에 그렇게 놓은 것으로 이해했어. |  |  |  |
| stationary-action | memorized | S[x+e]를 유도하는 과정에서 피적분식이 L(x,x')과 (dL/dx)\**e+ (dL/dx')\**e' + ... 로 테일러 전개되면서 S[x] + dS + HOT로 유도되는데, 이때 dS가 0이라는 전제 때문에 Euler-Lagrange eq가 유도되는 것으로 학습했어 |  |  |  |
| variation-of-velocity | memorized | x'가 어떻게 바뀌는지..?는 잘 모르겠네. |  |  |  |
| fundamental-lemma-of-variations | can_explain | η(t)를 그 어떤 함수로 잡아도, 즉 어떤 방식으로 기존 x를 흔들더라도 적분값이 0이 나와야 하기 때문에 모든 t에서 해당 함숫값이 0이 나와야하는거지 |  |  |  |
| newton-equation-from-euler-lagrange | memorized | d/dt(mx') = -kx |  |  |  |
| canonical-momentum | memorized | 일반적인 선운동량과 달라. q를 어떤 좌표계에 적용하는지에 따라 canonical momentum이 의미하는 물리량도 달라져. 일례로 theta를 q로 잡으면 p_q가 우리가 아는 각운동량으로 유도돼. |  |  |  |
| cyclic-coordinate-angular-momentum-conservation | can_explain | 각운동량 보존 법칙이 나오지. torque가 0일 때 p_theta가 보존된다는 내용 |  |  |  |
<!-- MASTERY-TABLE:END -->

## 읽는 법

- **암기**가 많다 = 답은 아는데 설명은 못 하는 상태. 그 개념부터 다시 설명해 보면 된다.
- **설명가능**이 늘어나는 것이 발전의 증거다. 개수보다 *무엇이* 올라갔는지를 본다.
- 같은 개념이 나중에 올라가면 새 줄로 쌓여 **변화**가 보인다(덮어쓰지 않는다).
