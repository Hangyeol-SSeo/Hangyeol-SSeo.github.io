---
layout: page
title: Naver Cafe Video Downloader
permalink: /projects/naver-cafe-downloader/
---

# Naver Cafe Video Downloader

> 네이버 카페의 동영상을 쉽게 다운로드 할 수 있는 Chrome 확장프로그램

[![Chrome Web Store](https://img.shields.io/badge/Chrome%20Web%20Store-Download-red?style=flat-square&logo=googlechrome)](https://chromewebstore.google.com/detail/navercafe-video-downloade/glclhpipfpfammoflcfnknnlddkgpdoe)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=flat-square&logo=github)](https://github.com/Hangyeol-SSeo/NaverCafe-VideoDownloader)

## 프로젝트 개요

네이버 카페에 업로드된 동영상을 개발자 도구 없이 간편하게 다운로드할 수 있는 크롬 확장프로그램입니다.

## 성과

- **WAU (주간 활성 사용자)**: 18,000명
- **평점**: 4.94/5.0 (17개 리뷰)
- **Chrome Web Store** 정식 배포

## 기술 스택

- **Vanilla JavaScript** - 추가 라이브러리 없이 순수 자바스크립트로 구현
- **Chrome Extension API** - 확장프로그램 개발
- **네이버 API 분석** - 네트워크 패킷 분석 및 API 역공학

## 해결한 문제

### 기존 문제점
기존에는 네이버 카페의 동영상을 다운로드하기 위해:
1. 개발자 도구(F12)를 열어야 함
2. Network 탭에서 영상 URL을 찾아야 함
3. URL을 복사하여 새 탭에서 열어야 함
4. 다운로드 버튼을 눌러야 함

이러한 과정이 **번거롭고 일반 사용자에게는 어려운 작업**이었습니다.

### 해결 방법
원클릭으로 게시물의 모든 동영상을 선택한 화질로 다운로드할 수 있도록 구현했습니다.

## 주요 기능

### 1. 원클릭 다운로드
- 확장프로그램 아이콘 클릭 시 팝업 표시
- 게시물의 모든 동영상 자동 감지
- 선택한 동영상 즉시 다운로드

### 2. 화질 선택
- 동영상별 사용 가능한 화질 자동 감지
- 원하는 화질 선택 후 다운로드
- 최고 화질 자동 선택 옵션

### 3. 다중 동영상 지원
- 한 게시물의 여러 동영상을 한 번에 처리
- 각 동영상별 개별 다운로드 가능

### 4. 탭별 독립 작동
- 각 탭에서 독립적으로 동작
- 여러 카페 게시물을 동시에 열어도 충돌 없음

## 구현 세부사항

### 네이버 API 분석
```javascript
// 네이버 카페 동영상 API 엔드포인트 분석
// 네트워크 패킷 분석을 통한 동영상 URL 추출
// 화질별 URL 파싱
```

- Chrome DevTools를 통한 네트워크 요청 분석
- 네이버 카페의 동영상 서빙 구조 파악
- API 엔드포인트 역공학

### Content Script
- 페이지 DOM 분석 및 동영상 요소 감지
- 동영상 메타데이터 추출
- Background Script와 통신

### Background Script
- 탭별 상태 관리
- 다운로드 요청 처리
- 네이버 API 호출

### Popup UI
- 사용자 친화적인 인터페이스
- 동영상 목록 표시
- 화질 선택 옵션

## 기술적 도전

### 1. 추가 라이브러리 없이 구현
- 번들 크기 최소화를 위해 Vanilla JS만 사용
- 네이티브 API만으로 모든 기능 구현

### 2. 네이버 API 분석
- 공식 문서 없이 네트워크 패킷만으로 분석
- 동영상 URL 구조 파악
- 인증 및 보안 메커니즘 우회

### 3. 확장프로그램 권한 최소화
- 필요한 최소한의 권한만 요청
- 사용자 프라이버시 보호

## 사용자 반응

평점 4.94점으로 높은 사용자 만족도를 보이고 있으며, 주간 활성 사용자 18,000명이 꾸준히 사용하고 있습니다.

## 향후 개선 사항

- 일괄 다운로드 기능 추가
- 파일명 자동 생성 옵션
- 다운로드 이력 관리
- 다른 카페 플랫폼 지원 검토

---

[← 프로젝트 목록으로 돌아가기](/#projects)
