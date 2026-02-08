---
layout: post
title: "가계부 웹앱 리디자인: AI 분업화로 품질과 속도 동시에 확보하기"
date: 2026-02-08
categories: [project]
tags: [finance, ui-ux, portfolio, ai-collaboration, codex, gemini, antigravity]
lang: ko
---

# 가계부 웹앱 리디자인: AI 분업화로 품질과 속도 동시에 확보하기

## 프로젝트 개요
이번 작업은 백엔드 API와 데이터 구조를 건드리지 않고, 가계부 웹앱의 화면 품질을 개선하는 리디자인 프로젝트입니다.  
핵심 목표는 단순한 디자인 변경이 아니라, **AI를 역할별로 분업해 실무형 생산성을 끌어올리는 운영 방식**을 정립하는 것이었습니다.

## 왜 이 방식이 중요한가
- 하나의 모델에 기획/디자인/코딩을 모두 맡기면 결과 품질 편차가 커집니다.
- 이번에는 모델별 강점을 분리해서 사용했습니다.
  - **Gemini 3 Pro**: 디자인 제안과 방향성 비교
  - **Codex**: 최소 diff 기반 코드 반영
  - **Antigravity (+ Nano Banana 2)**: 워크플로우 운영 및 시각 자료 정리
- 결과적으로 재작업을 줄이고, 품질을 더 안정적으로 확보했습니다.

## AI별 장단점과 역할 분담
### 1) Gemini 3 Pro (디자인 제안)
- 장점: 화면 톤, 정보 계층, 레이아웃 아이디어를 빠르게 비교 가능
- 단점: 코드 적용 정확도는 별도 검증 필요

### 2) Codex (코드 구현)
- 장점: 제약 조건(기존 API/데이터 구조 유지) 아래에서 안전하게 반영
- 단점: 디자인 발상 자체는 별도 입력이 필요

### 3) Antigravity (운영/자산 관리)
- 장점: 작업 흐름 연결, 결과물 정리, 발표용 자료 준비에 유리
- 단점: 최종 품질은 모델 역할 설계에 따라 달라짐

## 실제 진행 프로세스
1. 리디자인 범위와 제약(데이터/API 변경 금지) 확정
2. Gemini 3 Pro로 복수 시안 생성
3. 하이브리드안(C안 + A안) 채택
4. Codex로 최소 diff 구현
5. 데스크톱/모바일 스크린샷 생성
6. GitHub Pages와 Notion에 프로젝트 기록 동기화

## 결과
- 화면의 시각적 계층이 명확해지고 가독성이 개선됨
- 모바일 390px 기준 레이아웃 깨짐 없이 동작 확인
- 포트폴리오/프로젝트 발표에 바로 쓸 수 있는 시각자료 확보
- 이후 프로젝트에도 재사용 가능한 AI 분업 템플릿 확보

## 스크린샷
![Finance redesign desktop](/images/portfolio/finance-redesign-desktop-2026-02-08.png)
![Finance redesign mobile](/images/portfolio/finance-redesign-mobile-2026-02-08.png)

## 소스 리포지토리
- 워크스페이스 소스: [INO95/moltbot-workspace-202602](https://github.com/INO95/moltbot-workspace-202602)
- 블로그 소스: [INO95/ino95.github.io](https://github.com/INO95/ino95.github.io)

## 전문성 포인트
이번 사례는 “AI를 잘 쓰는 법”을 도구 사용이 아니라 **의사결정 구조**로 보여줍니다.  
기획(제안) - 구현(검증) - 운영(전달)을 분리하면, 속도와 안정성을 동시에 얻을 수 있습니다.
