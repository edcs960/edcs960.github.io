---
title: "DevRoster 개발기: 시리즈 목차"
date: 2026-11-10 08:00:00 +0900
categories: [DevRoster, 개발기]
tags: [devroster, ai-agent, series]
pin: true
---

DevRoster는 기획서 한 장을 명세서, 화면 목업, 승인된 개발 작업으로 바꿔 여러 AI 코딩 도구에 넘기는 로컬 작업대다. 그걸 만들면서 부딪힌 것들을 순서대로 적어 두고 있다. 글은 작업이 끝날 때마다 하나씩 늘어난다.

공개 저장소: <https://github.com/edcs960/devroster>

## 목차

1. [DevRoster는 무엇이고 왜 만들었나](/posts/devroster-01-intro/)
   기획서가 승인된 작업이 되기까지, 어디서 사람이 손을 대고 어디서 AI가 움직이는지
2. [구조를 지키는 법: 층 규칙을 테스트로 만들기](/posts/devroster-02-architecture/)
   adapters 층에 3만 줄이 쌓여 있던 이야기, 그리고 import 방향을 AST로 검사하게 된 과정
3. [Claude·Codex·Gemini·K-EXAONE를 한 흐름으로](/posts/devroster-03-multi-ai/)
   내 터미널의 AI와 분리하는 법, 도구가 달라도 같은 계약으로 부르는 법
4. [로컬 앱도 공격받는다: 보안 점검과 신뢰 경계](/posts/devroster-04-security/)
   여섯 가지 공격자를 세우고, 재현해 보고, "이 설정을 믿어도 되나"를 코드로 답한 기록
5. [구글 EGM에서 한 걸음 더: 독립 검토와 드리프트 검사](/posts/devroster-05-independent-review/)
   맥락 모르는 검토자를 여러 모델로 세우고, 명세와 코드가 어긋난 곳을 양쪽으로 찾기
6. [AI 토큰과 비용을 숫자로 보기: 사용량 대시보드](/posts/devroster-06-usage-dashboard/)
   대시보드를 만들다 걸린 집계 버그 셋, 그리고 가격을 왜 그때 값으로 고정하는지
7. [구독형과 종량제를 나눠 세는 비용 추적기](/posts/devroster-07-cost-tracking/)
   토큰 네 종과 캐시 수명별 단가, 실측으로 잡은 0.084달러 오차, 실패한 호출도 비용이라는 것
8. [SI 납품 산출물 파이프라인과 브라우저 콘솔 오류](/posts/devroster-08-deliverables-and-console/)
   기록보다 많이 말하지 않는 시험 결과서, 명세 밖에 둔 초안 4종, 콘솔 오류를 가려서 남기기
9. [순환 참조 0개, 파일 원복, OS 키링](/posts/devroster-09-hardening-and-cycles/)
   순환 import 44개 묶음을 0으로 만든 리팩토링, 파일을 건드리지 않는 되돌리기, 인증 값의 이사
10. [흩어진 화면 경계 다시 긋기 — 메뉴 다섯 묶음, 단계 승인, 설정 분리](/posts/devroster-10-navigation-and-settings/)
   소유 범위로 나눈 메뉴 16항목, 상태 문구 정본, 단계 승인을 작업실로 옮기며 만난 경쟁 조건, 단계별 설정 저장과 공통값 미리보기
11. [AI가 테스트를 약하게 만들거나 비밀값을 흘릴 때](/posts/devroster-11-weakened-tests-and-secrets/)
   테스트 약화 신호를 경고로, 읽지 못한 비밀값은 작업 중단으로, 보내기 직전 경계에서 한 번 더 가리기
12. [확정 디자인을 고정하고 QA가 나란히 보게 하기](/posts/devroster-12-approved-designs-and-skills/)
   검토한 스킬 통합과 목록 한도, Figma·Stitch 확정 디자인의 digest 고정·역할 전달·인계 ZIP, QA 비교와 목업 격리
