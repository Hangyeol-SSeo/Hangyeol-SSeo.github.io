---
layout: page
title: 1minute
permalink: /experience/1minute/
---

<div style="margin-top: 20px; margin-bottom: 40px;">
  <h1 style="margin-bottom: 10px;">1minute</h1>
  <p style="font-size: 1.6rem; color: #333; margin-bottom: 8px;">HRV / MWS 검사를 통해 고객의 상태를 측정하고 분석하여, 마음 건강을 챙겨주는 AI assistant 앱</p>
  <p style="font-size: 1.6rem; color: #333; margin-bottom: 20px;">2025.12 ~   | 프론트엔드 개발자</p>
</div>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">서비스 설명</h1>

## 배경:
현대인의 스트레스와 수면 부족 문제가 심화함에 따라, 주관적인 느낌이 아닌 객관적인 데이터에 기반한 멘탈 케어 솔루션이 필요함.

## 목적:
- MWS(심리 설문)와 HRV(심박 변이도) 데이터를 융합하여 사용자의 심신 상태를 정량적으로 분석
- 분석 결과에 따라 AI 기반 맞춤형 콘텐츠(명상 등)와 AI 상담사 서비스를 제공하여 실질적인 회복을 유도
- 일회성이 아닌, 지속 가능한 마음 회복 여정을 설계

<br/>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">핵심 기능</h1>

<div style="display: flex; gap: 20px; margin: 20px 0;">
  <div style="flex: 1; background: #f8f9fa; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">🫀 HRV / MWS 검사</h3>
    <p style="color: #666;">PPG 기반 심박 측정과 심리 설문으로 심신 상태를 정량적으로 측정 및 시각화</p>
  </div>
  <div style="flex: 1; background: #f8f9fa; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">🤖 AI 상담</h3>
    <p style="color: #666;">유형·연령·성별을 선택한 AI 상담사와 맞춤형 심리 상담 및 콘텐츠 추천</p>
  </div>
  <div style="flex: 1; background: #f8f9fa; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">🎬 마음건강 콘텐츠</h3>
    <p style="color: #666;">구독 기반 프리미엄 영상 콘텐츠 제공 및 수료 시스템</p>
  </div>
</div>

<br/>

---

<h1 class="growth-section-header" style="font-size: 2.8rem; margin-bottom:8px">🌱 역경과 성장</h1>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🛜 Webview를 활용한 React Native(RN) 앱</h2>
  <b>문제</b>: React Native를 다뤄본 팀원이 별로 없어, 개발 편의성을 위해 webview를 활용하기로 결정 <br/>
  <b>해결</b>: React-RN bridge 코드를 활용하여, 앱에서 webview로 띄운 웹사이트와 상호작용을 가능하게 구현<br/>
  <b>교훈</b>: Navigation 처리를 RN에서도 어느 정도 수행해야, bridge 코드가 한곳에 몰리지 않아 안정성이 있다는 것을 배움. 또한 webview로 띄운 화면의 배경 색상 처리와 기기의 상, 하단을 고려한 설계를 고민하는 시간을 가짐 <br/>
</div>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🧬 생체인증 구현(Android - fingerprint / iOS - face id)</h2>
  <b>문제</b>: 고객사에서 로그인 중 생체 인증을 사용하기를 원하여, React Native에서 생체 인증을 구현해야 함 <br/>
  <b>해결</b>: expo-local-authentication 라이브러리를 활용하여 OS에 맞춘 생체 인증 시스템을 구현함 <br/>
  <b>교훈</b>: 낯선 기능도 라이브러리 분석과 빠른 시도로 충분히 구현 가능하다는 것을 확인함. 그리고 일반 카메라 권한과 face id의 권한이 다르다는 사실도 배움. face id는 성공/실패 결과만 전달받고 이미지 데이터에 접근이 불가함 <br/>
</div>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🍀 Expo-Modules-Api를 사용하여 Native 모듈 구현</h2>
  <b>도전 과제</b>: PPG(Photoplethysmography) 심박 측정 기능 구현 시, 카메라로 초당 60프레임의 데이터를 실시간으로 수집하고 처리해야 했음. React Native로 구현한 초기 버전에서는 프레임 드롭과 발열 문제가 발생하여 안정적인 측정이 어려웠음 <br/>
  <b>문제 분석</b>: React Native의 JavaScript bridge를 통한 카메라 데이터 처리는 고빈도 실시간 연산에서 병목 현상을 일으키는 문제가 발생. 네이티브 언어(Swift, Kotlin) 대비 성능 차이가 명확했고, 이는 배터리 효율, 발열에도 영향을 미침 <br/>
  <b>해결</b>: Expo Modules API를 사용해 카메라 데이터 수집 및 신호 처리 로직을 Swift/Kotlin 네이티브 모듈로 구현 <br/>
  <b>교훈</b>: Expo 환경에서도 네이티브 코드 통합이 가능함을 확인. AI 도구를 활용해 미숙한 언어(Swift/Kotlin)로도 효과적으로 구현할 수 있었음 <br/>
</div>

<!--
<div style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">Webview를 활용한 React-Native 앱</h2>
  <b>문제</b>:  <br/>
  <b>원인</b>:  <br/>
  <b>해결</b>:  <br/>
  <b>교훈</b>:  <br/>
</div>
-->

<br/>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">🛠️ Tech Stack</h1>

<table style="width: 100%; border-collapse: collapse; font-size: medium">
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd; width: 30%;">Frontend</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      TypeScript, React-Native, React+Vite, Expo, Husky, firebase hosting
    </td>
  </tr>
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd;">Backend</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      SpringBoot, GKE(Google Kubernetes Engine)
    </td>
  </tr>
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd;">Database</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      Mysql
    </td>
  </tr>
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd;">Tools</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      Jira, Confluence, Figma, Slack
    </td>
  </tr>
</table>

<br/>

<hr class="print-hide"/>

<h1 style="font-size: 2.8rem; margin-bottom:8px">팀&역할</h1>

<div class="team-section" style="display: flex; gap: 20px; margin: 20px 0;">
  <div style="flex: 1; background: #f8f9fa; padding: 20px; border-radius: 8px; font-size: medium">
    <h3 style="margin-top: 0;">팀 구성</h3>
    <p style="color: #666; font-size: large">팀원 8명</p>
    - PM <br/>
    - 디자인 <br/>
    - 백엔드 1 <br/>
    - 인프라 1 <br/>
    - 프론트엔드 4 <br/>
  </div>
  <div style="flex: 1; background: #e3f2fd; padding: 20px; border-radius: 8px; font-size: medium">
    <h3 style="margin-top: 0;">나의 역할</h3>
    <p style="color: #666; font-size: large">프론트엔드 개발</p>
    - React Native + React 프론트엔드 개발 <br/>
    - Apple connect store, Google play console 세팅 <br/>
    - Expo Modules API 도입(Swift, Kotlin) <br/>
    - Native bridge 구현 <br/>
  </div>
</div>

<br/>

---

<div style="text-align: center; margin-top: 60px;">
  <a href="/" style="display: inline-block; font-size: medium; padding: 12px 30px; background: #333; color: white; text-decoration: none; border-radius: 6px; transition: all 0.3s;">이력서 홈으로 돌아가기</a>
</div>
