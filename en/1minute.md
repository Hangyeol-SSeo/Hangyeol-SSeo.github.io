---
layout: page
title: 1minute
permalink: /en/experience/1minute/
---

<style>
  .header-container { display: none !important; }
  @media print { .header-container { display: none !important; } }
</style>

<div style="margin-top: 20px; margin-bottom: 40px;">
  <h1 style="margin-bottom: 10px;">1minute</h1>
  <p style="font-size: 1.6rem; color: #333; margin-bottom: 8px;">An AI assistant app that measures and analyzes users' mental and physical health through HRV/MWS assessments</p>
  <p style="font-size: 1.6rem; color: #333; margin-bottom: 20px;">2025.12 – Present | Frontend Developer</p>
</div>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">Service Description</h1>

## Background
As stress and sleep deprivation worsen among modern people, there is a growing need for mental care solutions based on objective data rather than subjective feelings.

## Purpose
- Quantitatively analyze users' mental and physical states by combining MWS (psychological surveys) and HRV (Heart Rate Variability) data
- Provide AI-powered, personalized content (meditation, etc.) and AI counseling based on analysis results to facilitate meaningful recovery
- Design a sustainable mental health recovery journey, not a one-time fix

<br/>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">Key Features</h1>

<div class="feature-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 20px 0;">
  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 HRV / MWS Assessment</h3>
    <p style="color: #666;">Measures users' physical and psychological states, visualized as quantitative data</p>
    <ul>
      <li>PPG (Photoplethysmography)-based HRV (Heart Rate Variability) measurement</li>
      <li>MWS psychological survey (BIG 5 personality, depression, anxiety, stress)</li>
      <li>Assessment results and recent trend data viewable across multiple screens</li>
    </ul>
  </div>

  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 AI Counseling</h3>
    <p style="color: #666;">Chat with an AI counselor of the user's choice</p>
    <ul>
      <li>Choose counselor type (Mind Guardian, Mind Trainer, Mind Analyst, Mind Friend), age group, and gender for AI chat</li>
      <li>Personalized content recommended after counseling session</li>
      <li>AI chat reporting feature</li>
    </ul>
  </div>

  <div style="background: #fff; border: 2px solid #e0e0e0; padding: 20px; border-radius: 8px;">
    <h3 style="margin-top: 0;">📌 Mental Health Content</h3>
    <p style="color: #666;">Periodically released mental health video content</p>
    <ul>
      <li>Standard and premium content tiers</li>
      <li>Premium content available only to subscribed users</li>
      <li>Bookmark favorite content</li>
      <li>Completion awarded upon watching 80%+ of a video</li>
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
      TypeScript, React-Native, React+Vite, Expo, Husky, Firebase Hosting
    </td>
  </tr>
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd;">Backend</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      SpringBoot, GKE (Google Kubernetes Engine)
    </td>
  </tr>
  <tr>
    <td style="padding: 12px; background: #f5f5f5; font-weight: bold; border: 1px solid #ddd;">Database</td>
    <td style="padding: 12px; border: 1px solid #ddd;">
      MySQL
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

<h1 class="growth-section-header" style="font-size: 2.8rem; margin-bottom:8px">🌱 Adversity & Growth</h1>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🛜 React Native App with WebView</h2>
  <b>Problem</b>: Few team members had React Native experience, so we decided to utilize WebView for development convenience <br/>
  <b>Solution</b>: Implemented React–RN bridge code to enable interaction between the app and the web pages displayed in WebView <br/>
  <b>Lesson</b>: Learned that handling some navigation on the RN side prevents bridge code from being concentrated in one place, improving stability. Also spent time designing around background color handling for WebView screens and device safe areas <br/>
</div>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🧬 Biometric Authentication (Android Fingerprint / iOS Face ID)</h2>
  <b>Problem</b>: The client requested biometric authentication during the login flow in React Native <br/>
  <b>Solution</b>: Implemented an OS-specific biometric authentication system using the expo-local-authentication library <br/>
  <b>Lesson</b>: Realized that the implementation was simpler than expected — a reminder not to fear trying new things. Also learned that camera permissions and Face ID permissions are different; Face ID only returns success/failure without accessing image data <br/>
</div>

<div class="growth-card" style="background: #f5f5f5; padding: 30px; border-radius: 12px; margin: 20px 0; font-size: medium">
  <h2 style="color: #222222">🍀 Native Modules via Expo Modules API</h2>
  <b>Challenge</b>: PPG (Photoplethysmography) heart rate measurement required real-time processing of camera data at 60 FPS. The initial React Native implementation suffered from frame drops and overheating <br/>
  <b>Analysis</b>: Processing camera data through React Native's JavaScript bridge created bottlenecks for high-frequency real-time computation, with a clear performance gap compared to native languages (Swift, Kotlin), also affecting battery efficiency and heat <br/>
  <b>Solution</b>: Used Expo Modules API to implement camera data collection and signal processing logic as native modules in Swift/Kotlin <br/>
  <b>Lesson</b>: Confirmed that native code integration is possible within the Expo ecosystem. Leveraged AI tools to effectively implement in unfamiliar languages (Swift/Kotlin) <br/>
</div>

<br/>

---

<h1 style="font-size: 2.8rem; margin-bottom:8px">Team & Role</h1>

<div class="team-section" style="display: flex; gap: 20px; margin: 20px 0;">
  <div style="flex: 1; background: #f8f9fa; padding: 20px; border-radius: 8px; font-size: medium">
    <h3 style="margin-top: 0;">Team Composition</h3>
    <p style="color: #666; font-size: large">8 members</p>
    - PM <br/>
    - Design <br/>
    - Backend × 1 <br/>
    - Infrastructure × 1 <br/>
    - Frontend × 4 <br/>
  </div>
  <div style="flex: 1; background: #e3f2fd; padding: 20px; border-radius: 8px; font-size: medium">
    <h3 style="margin-top: 0;">My Role</h3>
    <p style="color: #666; font-size: large">Frontend Development</p>
    - React Native + React frontend development <br/>
    - Apple App Store Connect & Google Play Console setup <br/>
    - Expo Modules API adoption (Swift, Kotlin) <br/>
    - Native bridge implementation <br/>
  </div>
</div>

<br/>

---

<div style="text-align: center; margin-top: 60px;">
  <a href="/en/" style="display: inline-block; font-size: medium; padding: 12px 30px; background: #333; color: white; text-decoration: none; border-radius: 6px; transition: all 0.3s;">Back to Resume</a>
</div>
