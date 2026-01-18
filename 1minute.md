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
현대인의 스트레스와 수면 부족 문제가 심화됨에 따라, 주관적인 느낌이 아닌 객관적인 데이터에 기반한 멘탈 케어 솔루션이 필요함.

## 목적:
- MWS(심리 설문)와 HRV(심박변이도) 데이터를 융합하여 사용자의 심신 상태를 정량적으로 분석
- 분석 결과에 따라 AI 기반 맞춤형 콘텐츠(명상 등)와 AI 상담사 서비스를 제공하여 실질적인 회복을 유도
- 일회성이 아닌, 지속 가능한 마음 회복 여정을 설계

<!-- 추후 스크린샷 추가 -->

<br/>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">핵심 기능</h1>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 20px 0;">
  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 HRV / MWS 검사</h3>
    <p style="color: #666;">유저의 몸 상태 & 심리 상태를 측정하여 정량적 데이터로 시각화</p>
    <ul>
      <li>PPG(Photoplethysmography) 기반 HRV(Heart Rate Variability) 측정</li>
      <li>MWS 심리 설문(성격 BIG5, 우울, 불안, 스트레스) 진행</li>
      <li>검사 결과와 최근 기록 변동은 홈 탭이나 검사 탭 등 여러 화면에서 확인 가능</li>
    </ul>
  </div>

  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 AI 상담</h3>
    <p style="color: #666;">유저가 선택하는 AI 상담사와 심리 상담</p>
    <ul>
      <li>심리 상담사 유형(마음 지킴이, 마음 트레이너, 마음 분석가, 마음 친구)과 연령대, 성별을 결정하여 AI 상담사와 채팅</li>
      <li>AI 상담 종료 후 맞춤 컨텐츠 추천</li>
      <li>AI 채팅 신고 기능</li>
    </ul>
  </div>

  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 마음건강 컨텐츠 시청</h3>
    <p style="color: #666;">주기적으로 배포되는 마음 건강 컨텐츠 동영상 시청 기능 제공</p>
    <ul>
      <li>일반 컨텐츠, 프리미엄 컨텐츠 구분</li>
      <li>프리미엄 컨텐츠는 구독을 활성화한 유저만 시청 가능</li>
      <li>마음에 드는 컨텐츠 북마크</li>
      <li>동영상의 80%이상 시청시 수료</li>
    </ul>
  </div>
</div>

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

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">🌱 역경과 성장</h1>
<!--
지문, face id
webview
-->
<div style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">Webview를 활용한 React Native(RN) 앱</h2>
  <b>문제</b>: React Native를 다뤄본 팀원이 별로 없어, 개발 편의성을 위해 webview를 활용하기로 결정 <br/>
  <b>해결</b>: React-RN bridge 코드를 활용하여, 앱에서 webview로 띄운 웹사이트와 상호작용을 가능하게 구현<br/>
  <b>교훈</b>: Navigation 처리를 RN에서도 어느 정도 수행해야, bridge 코드가 한곳에 몰리지 않아 안정성이 있다는 것을 배움. 또한 webview로 띄운 화면의 배경 색상 처리와 기기의 상, 하단을 고려한 설계를 고민하는 시간을 가짐 <br/>
</div>

<div style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">생체인증 구현(Android - fingerprint / iOS - face id)</h2>
  <b>문제</b>: 고객사에서 로그인 중 생체 인증을 사용하기를 원하여, React Native에서 생체 인증을 구현해야 함 <br/>
  <b>해결</b>: expo-local-authentication 라이브러리를 활용하여 OS에 맞춘 생체 인증 시스템을 구현함 <br/>
  <b>교훈</b>: 구현이 생각보다 어렵지 않아서 겁먹지 않고 뭐든 시도해 보아야겠다고 깨달음. 그리고 일반 카메라 권한과 face id의 권한이 다르다는 사실도 배움. face id는 성공/실패 결과만 전달받고 이미지 데이터에 접근이 불가함 <br/>
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

<h1 style="font-size: 2.8rem; margin-bottom:8px">팀&역할</h1>

<div style="display: flex; gap: 20px; margin: 20px 0;">
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
