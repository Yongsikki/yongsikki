---
{"dg-publish":true,"permalink":"/source/ppm-icd-mode/","tags":["source"],"created":"2025-12-11T19:57:08.436+10:00","updated":"2025-12-11T19:57:08.436+10:00"}
---

# PPM (Permanent Pacemaker), ICD, 그리고 Mode 정리

## 1. PPM (Permanent Pacemaker)

-   **역할**: 서맥(Bradycardia) 등으로 인해 맥박이 너무 느릴 때,
    규칙적인 전기 자극을 줘서 심박수를 유지하는 장치.
-   **적응증**
    -   Sick sinus syndrome(SSS)
    -   AV block (2도 Mobitz type 2, 3도 AV block 등)
    -   심박수가 너무 느려 증상이 있을 때
-   **구성 요소**
    -   Pulse generator(배터리 + 회로)
    -   Lead(전극)
-   **기능**
    -   심박수가 낮으면 pacing
    -   필요 시만 pacing하는 demand mode 존재

------------------------------------------------------------------------

## 2. ICD (Implantable Cardioverter Defibrillator)

-   **역할**: 치명적인 부정맥(VT/VF)을 감지하고 자동으로 전기 충격을
    주어 정상 리듬으로 되돌리는 기기.
-   **적응증**
    -   심근경색 후 EF \< 35%로 지속
    -   재발성 sustained VT
    -   VF episode 과거력
-   **기능**
    -   Defibrillation: 고에너지 전기 쇼크
    -   Cardioversion: 저에너지 쇼크
    -   Anti-tachycardia pacing(ATP): 빠른 빈맥을 pacing으로 종료

------------------------------------------------------------------------

## 3. Pacemaker Mode (NBG Code)

Pacemaker 모드는 **5자리 코드(NBG code)** 로 구성된다.

### ▸ 1번째 자리: Pace하는 부위

-   **O**: 없음\
-   **A**: Atrium\
-   **V**: Ventricle\
-   **D**: Dual (A+V)

### ▸ 2번째 자리: Sense하는 부위

-   **O**: 없음\
-   **A**: Atrium\
-   **V**: Ventricle\
-   **D**: Dual

### ▸ 3번째 자리: 반응 방식

-   **O**: 반응 없음\
-   **I**: Inhibition (감지되면 pacing 중단)\
-   **T**: Triggering (감지되면 pacing 유발)\
-   **D**: Dual (I + T)

### ▸ 4번째 자리: Rate modulation

-   **O**: 없음\
-   **R**: 있음 (activity에 따라 pacing rate 조절)

### ▸ 5번째 자리: Pacing mode

-   **O**: 없음\
-   **A**: Atrium\
-   **V**: Ventricle\
-   **D**: Dual

------------------------------------------------------------------------

## 주요 Mode 예시

-   **VVI**
    -   Ventricle pace\
    -   Ventricle sense\
    -   Inhibited\
        → 심실이 기준보다 느리면 pace, 감지되면 pace 중단\
-   **DDD**
    -   A/V pace\
    -   A/V sense\
    -   Dual response\
        → 가장 fiziologic한 mode\
-   **AAI**
    -   Atrium만 pace/sense\
    -   Sick sinus syndrome에서 사용

------------------------------------------------------------------------

## PPM vs ICD 비교

  항목          PPM                ICD
  ------------- ------------------ ---------------------------
  목적          서맥 치료          치명적 부정맥(VT/VF) 예방
  기능          Pacing만           Pacing + Shock + ATP
  적응증        SSS, AV block 등   EF 저하, VT/VF 병력 등
  충격(Shock)   없음               있음

------------------------------------------------------------------------

## Obsidian 사용 팁

-   제목은 `#` 사용\
-   내부 링크는 `[[파일명]]`\
-   표는 markdown 표 형식 그대로 사용 가능\
-   구분선 `---` 사용 가능
