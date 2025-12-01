# 🛡️ Store Shield

<div align="center">

**AI 기반 스마트 무인점포 통합관리 시스템**

[![Qualcomm Symposium](https://img.shields.io/badge/Qualcomm-University_Symposium_2025-00B4FF?style=for-the-badge&logo=qualcomm&logoColor=white)](https://youtu.be/7BZvnLclQCs)
[![Demo Video](https://img.shields.io/badge/YouTube-Demo_Video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/4Jdi7Hx5ZVs)

실시간 AI 영상분석으로 무인점포의 **보안·재고·매장관리**를 하나로 통합

</div>

---

## 📺 프로젝트 시연

### 💡 전체 기능 데모
[![Store Shield Demo](https://img.youtube.com/vi/4Jdi7Hx5ZVs/maxresdefault.jpg)](https://youtu.be/4Jdi7Hx5ZVs)
> 🎬 **[시연 영상 보기](https://youtu.be/4Jdi7Hx5ZVs)** - CCTV 추적, 자동 재고 관리, 절도 감지 등 핵심 기능 시연

---

## 🎯 프로젝트 개요

**Store Shield**는 무인점포 운영의 핵심 문제를 AI 기술로 해결하는 통합 관리 시스템입니다.

### 핵심 목표
- 🔐 **실시간 고객 추적** 및 ID 기반 행동 분석으로 절도 위험 감소
- 📦 **자동화된 재고 관리**로 재고 부족 사태 예방 및 발주 효율 향상
- 📊 **데이터 기반 매장 분석**으로 매출 증대 및 고객 만족도 향상
- 📱 **모바일 앱 원격 관리**로 운영 효율 개선

---

## 🏗️ 시스템 아키텍처

![시스템 구조도](https://github.com/user-attachments/assets/af9ec3df-7a79-4f49-b5d3-287a5ff3f347)

### 시스템 구성
```
📱 CCTV (Android)          →  🖥️ Flask Server  →  📱 Manager App (Flutter)
     ↓                              ↓                      ↓
  AI 영상분석              WebSocket 실시간 통신      매장 관리 대시보드
(YOLO-NAS + Face)            MySQL Database          알림 및 모니터링
```

---

## 🎨 전체 실행 화면

![전체 실행화면](https://github.com/user-attachments/assets/22ce0dbf-7486-414b-93d2-97bc480e2d25)

---

## ✨ 주요 기능

### 🔐 보안 관리
**실시간 객체 추적 및 ID 부여**
- 고객 입장 시 고유 ID 자동 할당
- 매장 내 이동 경로 실시간 추적
- AI 기반 고객 행동 패턴 분석

**미결제 퇴장 자동 감지**
- 키오스크 결제 여부 실시간 확인
- 미결제 상태로 퇴장 시도 시 즉시 알림 발송
- 절도 의심 고객 영상 자동 저장

### 📦 재고 관리
**실시간 재고 모니터링**
- 결제 시 재고 자동 업데이트
- 상품 픽업/반납 감지 및 기록
- 재고 부족 임계치 설정 및 알림

**AI 기반 발주 시스템**
- 판매 패턴 분석 기반 최적 발주량 추천
- 재고 회전율 및 수요 예측

### 📊 매장 관리
**실시간 매출 분석**
- 일/주/월 단위 매출 데이터 시각화
- 시간대별 매출 패턴 분석
- 상품 카테고리별 판매 추이

**고객 행동 분석**
- 시간대별 방문자 수 통계
- 평균 체류 시간 및 동선 분석
- 인기 상품 및 진열대 효과 측정

**모바일 통합 모니터링**
- CCTV 실시간 스트리밍
- 푸시 알림 및 원격 대응
- 대시보드 형태의 핵심 지표 확인

---

## 🛠️ 기술 스택

### AI/Computer Vision
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Qualcomm](https://img.shields.io/badge/Qualcomm_AI_Hub-00B4FF?style=flat-square&logo=qualcomm&logoColor=white)

- **YOLO-NAS**: 실시간 객체 감지 및 추적
- **Lightweight Face Detection**: 고객 얼굴 인식 및 ID 부여
- **Qualcomm AI Hub**: 온디바이스 AI 추론 최적화

### Backend
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

- **Flask**: Python 기반 웹 서버
- **Socket.IO**: 실시간 양방향 통신 (WebSocket)
- **MySQL**: 고객/재고/매출 데이터 관리

### Frontend/Mobile
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

- **Android (Java)**: CCTV 앱 (AI 영상 분석)
- **Flutter (Dart)**: 관리자용 모바일 앱
- **HTML/JavaScript**: 키오스크 인터페이스

### Infrastructure
![ngrok](https://img.shields.io/badge/ngrok-1F1E37?style=flat-square&logo=ngrok&logoColor=white)

- **ngrok**: 로컬 서버 외부 접근용 HTTP 터널링

---

## 👥 팀 구성

| 이름 | 역할 | 담당 업무 |
|------|------|-----------|
| **홍혜창** | Backend Developer | Flask 서버 개발, WebSocket 통신, DB 연동 |
| **전상우** | AI/CV Engineer | YOLO-NAS 객체 추적, 온디바이스 AI 최적화 |
| **최은서** | AI/CV Engineer | Face Detection, CCTV 앱 개발 (Android) |
| **윤현도** | Mobile Developer | Flutter 앱 개발, UI/UX 설계 |
| **이선빈** | Mobile Developer | Flutter 앱 개발, DB 설계 |

---

## 🏆 수상 및 발표

### 🎓 Qualcomm University Platform Symposium 2025 선정
- **전세계 유수 대학 중 선정**되어 글로벌 심포지엄에서 프로젝트 발표
- UCSD, IIT 등 해외 명문 대학들과 함께 연구 성과 공유
- 국내 대학 중 컴퓨터공학 분야 대표로 선정

[![Qualcomm Symposium Presentation](https://img.youtube.com/vi/7BZvnLclQCs/maxresdefault.jpg)](https://youtu.be/7BZvnLclQCs)
> 🎤 **[발표 영상 보기](https://youtu.be/7BZvnLclQCs)** - Qualcomm University Platform Symposium 2025

---

## 📦 레포지토리 구조

이 조직은 Store Shield 프로젝트의 각 모듈을 독립된 레포지토리로 관리합니다.

| 레포지토리 | 설명 | 기술 스택 |
|-----------|------|----------|
| **[StoreShield-app](링크)** | 사장님용 관리 앱 | Flutter, Dart |
| **[yolo-nas-app](링크)** | CCTV AI 영상 분석 앱 | Android (Java), YOLO-NAS |
| **[server](링크)** | 백엔드 서버 및 키오스크 | Flask, Socket.IO, MySQL |

---

## 📅 프로젝트 기간

**2025.01.01 ~ 2025.08.01** (7개월)

---

## 🚀 주요 특징

### 🎯 차별화 포인트
1. **온디바이스 AI 처리**: Qualcomm AI Hub를 활용한 경량화 모델로 CCTV에서 직접 AI 추론
2. **실시간 양방향 통신**: Socket.IO 기반 WebSocket으로 즉각적인 데이터 동기화
3. **통합 관리 시스템**: 보안, 재고, 매출을 하나의 플랫폼에서 관리
4. **확장 가능한 구조**: 모듈화된 설계로 추가 기능 통합 용이

### 💡 기술적 도전
- **실시간 객체 추적**: 커스텀 MOT(Multi-Object Tracking) 알고리즘으로 사람 교차 상황에서도 안정적인 ID 유지
- **저전력 AI 추론**: 모바일 환경에서 YOLO-NAS 최적화
- **대용량 실시간 통신**: 영상 스트리밍 + 데이터 전송 동시 처리

---


<div align="center">

**Made with ❤️ by Store Shield Team**

[![GitHub](https://img.shields.io/badge/GitHub-Store--Shield-181717?style=flat-square&logo=github)](https://github.com/Store-Shield)

</div>
