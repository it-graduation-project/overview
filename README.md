# 🎵 RhyFeel - 청각 없이도 음악을 '경험'하는 법

> 청각장애인을 위한 멀티모달 음악 번역 플랫폼  
> 음악의 **리듬과 비트**를 시각과 촉각으로 동기화해 체험할 수 있도록 설계했습니다.

![RhyFeel 포스터](./assets/poster.png)

---

## 🧠 Why RhyFeel?

청각장애인은 여전히 음악 감상에서 소외되어 있습니다.  
RhyFeel은 소리를 ‘보게’ 하고, ‘느끼게’ 함으로써  
**음악의 감각적 접근성**을 실현하는 실험적 플랫폼입니다.

---

## ⚙️ What It Does

- 🎧 **실시간 주파수 분석**  
  - 10ms 단위 음악 분석 (Web Audio API 기반 FFT)

- 🎨 **3D 시각화**  
  - 음악 리듬에 따라 실시간으로 형태 변화 (Three.js + Shader)

- 📳 **손목 진동 피드백**  
  - 진동 모터 4개가 음악 강약에 맞춰 즉각 반응 (ESP32 + Web Serial)

- ✋ **제스처 기반 제어**  
  - 손 펼치면 재생, 주먹 쥐면 정지 (MediaPipe Hands 활용)

- 🚀 **웹에서 즉시 실행**  
  - 설치 없이, 브라우저에서 바로 체험 가능 → [rhyfeel.site](https://rhyfeel.site)

---

## 🧩 How It Works

1️⃣ **🎵 음악 업로드**  
  └─ 사용자가 로컬 음악 파일 업로드

2️⃣ **🔍 주파수 분석 (10ms 단위)**  
  └─ Web Audio API를 통해 실시간 FFT 분석

3️⃣ 출력 분기  
- 🎨 **3D 시각화** (Three.js)  
  ↳ 음악 리듬에 따라 이코사헤드론 형태 실시간 변화  
- 🔉 **손목 진동 출력** (ESP32 + Web Serial API)  
  ↳ 주파수 강도에 따라 진동 강도 실시간 조절

4️⃣ ✋ **제스처 제어** (MediaPipe Hands)  
  └─ 손 펼치면 ▶️ 재생 / 주먹 쥐면 ⏸️ 정지

---

## 🌐 기술 스택 요약

| 구분 | 기술 |
|------|------|
| Frontend | React, Three.js, Web Audio API, MediaPipe |
| Backend | Spring Boot, MySQL, AWS EC2 |
| 하드웨어 | ESP32, L9110S 모터드라이버, 진동 모터 4개 |
| 통신 방식 | Web Serial API (USB 기반 실시간 전송) |

---

## 🎯 핵심 가치

- **청각장애인의 음악 감상 접근성 향상**
- **시각 + 촉각 통합**으로 몰입형 감각 경험 제공
- **하드웨어 + 웹의 경량화 통합 시스템**
- **누구나 어디서든 체험 가능한 보편적 UX**

---

## 📄 발표 자료

👉 [2024_RhyFeel_Presentation.pdf](./2024_RhyFeel_Presentation.pdf)

---

## 🔗 웹사이트

📌 [https://rhyfeel.site](https://rhyfeel.site)

> USB로 디바이스 연결 후, 음악 파일을 업로드해보세요.  
> 음악이 눈으로, 손목으로 ‘들립니다’.

---
