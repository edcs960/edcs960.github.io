---
title: "DevRoster 개발기: 시리즈 목차"
date: 2026-11-10 08:00:00 +0900
categories: [DevRoster, 개발기]
tags: [devroster, ai-agent, series]
pin: true
---

여러 AI 코딩 도구로 실제 개발을 진행하는 로컬 작업대 **DevRoster**를 만들며 배운 것을 정리하는 시리즈입니다. 글은 작업이 진행될 때마다 계속 추가됩니다.

DevRoster 공개 저장소: <https://github.com/edcs960/devroster>

## 목차

1. [DevRoster는 무엇이고 왜 만들었나](/posts/devroster-01-intro/)
   기획서 한 장에서 승인된 개발 작업까지, 사람이 승인하고 AI가 일하는 흐름
2. [구조를 지키는 법: 층 규칙을 테스트로 만들기](/posts/devroster-02-architecture/)
   3만 줄짜리 adapters 층을 발견하고, import 방향을 AST로 검사하기까지
3. [Claude·Codex·Gemini·K-EXAONE를 한 흐름으로](/posts/devroster-03-multi-ai/)
   AI 도구를 격리하고, 같은 규칙으로 부르고, 다른 모델로 서로 검토하게 하기
4. 로컬 앱도 공격받는다: 보안 점검과 신뢰 경계 *(공개 예정)*
   위협 모델을 세우고, 재현하고, "이 설정을 믿어도 되는가"를 코드로 답하기
5. 구글 EGM에서 한 걸음 더: 독립 검토와 드리프트 검사 *(공개 예정)*
   맥락 없는 검토자를 여러 모델로 꾸리고, 명세와 코드의 차이를 양방향으로 찾기
6. [AI 토큰과 비용을 숫자로 보기: 사용량 대시보드](/posts/devroster-06-usage-dashboard/)
   대시보드를 만들다 찾은 집계 버그 세 가지와 가격을 고정하는 이유
