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

## 🔧 트러블슈팅

### 사람 추적 시 ID 스위칭 문제 해결

#### 문제 상황: 사람이 교차하거나 빠르게 움직일 때 ID 유지 실패

**초기 추적 방식의 한계**

초기에는 **IoU(Intersection over Union)만을 기반**으로 객체를 추적했습니다. IoU는 두 바운딩 박스가 얼마나 겹치는지를 0~1 사이의 값으로 나타내는 지표입니다.
```
IoU = 교집합 영역 / 합집합 영역

┌────────┐
│ 이전   │
│  프레임│
│    ┌───┼────┐
│    │███│ 현재│  ← 겹치는 부분
└────┼███│ 프레임
     └────────┘

IoU가 높으면 → 같은 사람으로 판단
```

**발생한 문제**

이 방식은 **물품 추적에는 적합**했지만, **사람 추적에는 치명적인 한계**가 있었습니다:

1. **빠른 움직임 시 ID 손실**
```
   프레임 1: 사람(ID 3) 왼쪽에 위치
   프레임 2: 사람이 빠르게 오른쪽으로 이동
   → IoU가 낮아짐 (거의 겹치지 않음)
   → 시스템이 "새로운 사람"으로 인식
   → 새 ID(ID 8) 부여 ❌
```

2. **사람이 교차할 때 ID 스위칭**
```
   사람 A (ID 3, 빨간 옷) →
                              ← 사람 B (ID 5, 파란 옷)
   
   교차 후:
   사람 A (ID 5로 변경!) →  ❌
                              ← 사람 B (ID 3으로 변경!) ❌
```

**왜 문제인가?**

- **물품**: 가상선(y=500)을 넘을 때만 ID가 유지되면 됨
- **사람**: 매장에 들어온 순간부터 나갈 때까지 **하나의 ID를 계속 유지**해야 함
  - 이유 1: 가상의 장바구니가 사람 ID에 연결됨
  - 이유 2: 결제 시 올바른 고객을 찾아야 함
  - 이유 3: 절도 감지 시 정확한 고객 추적 필요

**문제 상황 예시**

![ID 스위칭 문제](docs/id-switching-problem.gif)

> 🔴 **문제**: 두 사람이 교차할 때 ID 추적 문제

---

#### 해결 방법: 다중 특징 기반 추적 알고리즘

**핵심 아이디어**: "어떻게 하면 몇 프레임 뒤의 이 사람이 이전의 그 사람과 같다고 증명할 수 있을까?"

이 질문에 답하기 위해 **IoU 외에 3가지 추가 특징**을 도입했습니다.

---

#### 1️⃣ 속도 벡터 예측

**개념**: 사람은 관성을 가지고 움직이므로, 이전 이동 방향을 고려하면 다음 위치를 예측할 수 있습니다.
```java
// 이동 평균 필터로 속도 계산 (가중치 0.7)
velocityX = 0.7 * (현재X - 이전X) + 0.3 * 이전velocityX
velocityY = 0.7 * (현재Y - 이전Y) + 0.3 * 이전velocityY

// 다음 프레임 위치 예측
predictedX = currentX + velocityX
predictedY = currentY + velocityY
```

**효과**:
```
이전 위치: (100, 200)
현재 위치: (120, 210)
→ 속도: (20, 10)

다음 프레임 예측: (140, 220)
실제 탐지: (138, 222) ← 예측과 가까움!
→ 같은 사람으로 판단 ✅
```

**방향 점수 계산**:
```java
// 예측 방향 ↔ 실제 이동 방향의 일치도 계산
float directionScore = calculateDirectionScore(tracked, detected);

// 일치하면 1.0, 반대면 0.0
```

---

#### 2️⃣ 색상 특징 추출 (사람 전용)

**개념**: 사람은 짧은 시간 내에 옷 색깔이 바뀌지 않습니다.

**추출 방법**:
```
사람 바운딩 박스
├─ 상체 영역 (25%~50% 높이)
│  └─ 중앙 60% 폭만 사용 (좌우 20% 제외)
│     → RGB 평균값 추출 예: [120, 80, 200] (보라색 셔츠)
│
└─ 하체 영역 (60%~85% 높이)
   └─ 중앙 60% 폭만 사용
      → RGB 평균값 추출 예: [50, 50, 60] (검정 바지)
```

**왜 중앙만 추출?**
- 바운딩 박스 가장자리에는 배경이나 다른 사람이 포함될 수 있음
- 중앙 60%만 사용하면 순수한 옷 색깔만 추출 가능

**색상 유사도 계산**:
```java
// 유클리드 거리 계산
float distance = sqrt(
    (R1-R2)² + (G1-G2)² + (B1-B2)²
);

// 거리가 작을수록 유사 → 점수로 변환
float colorSimilarity = max(0, 1 - distance/441.7);
```

**실제 예시**:
```
프레임 1: 사람 ID 3
  상체: [120, 80, 200] (보라색)
  하체: [50, 50, 60] (검정색)

프레임 10: 후보 1
  상체: [122, 78, 198] (거의 같은 보라색)
  하체: [48, 52, 58] (거의 같은 검정색)
  → 색상 유사도: 0.92 ✅ 같은 사람!

프레임 10: 후보 2
  상체: [200, 200, 50] (노란색)
  하체: [100, 120, 200] (파란색)
  → 색상 유사도: 0.15 ❌ 다른 사람!
```

**코드 구현**:
```java
// SimpleTracker.java
private void extractColorFeatures(TrackedObject obj, Bitmap bitmap) {
    // 상체 영역: 25%~50% 높이
    int upperBodyTop = top + (int)(height * 0.25);
    int upperBodyBottom = top + (int)(height * 0.50);
    
    // 하체 영역: 60%~85% 높이
    int lowerBodyTop = top + (int)(height * 0.60);
    int lowerBodyBottom = top + (int)(height * 0.85);
    
    // 중앙 60% 폭만 사용 (좌우 20% 제외)
    int widthMargin = (int)(width * 0.2);
    int centeredLeft = left + widthMargin;
    int centeredRight = right - widthMargin;
    
    // RGB 평균값 계산
    float[] upperBodyColors = calculateAvgColor(bitmap, 
        centeredLeft, upperBodyTop, centeredRight, upperBodyBottom);
    float[] lowerBodyColors = calculateAvgColor(bitmap, 
        centeredLeft, lowerBodyTop, centeredRight, lowerBodyBottom);
    
    obj.setColorFeatures(upperBodyColors, lowerBodyColors);
}
```

---

#### 3️⃣ 통합 매칭 점수 계산

**일반 상황 (사람이 혼자 움직일 때)**
```java
점수 = IoU × 0.4           // 겹침 정도
     + 크기유사도 × 0.1     // 바운딩 박스 크기
     + 색상유사도 × 0.25    // 옷 색깔
     + 방향점수 × 0.25      // 이동 방향
```

**예시**:
```
후보 A:
  IoU: 0.6 → 0.6 × 0.4 = 0.24
  크기: 0.9 → 0.9 × 0.1 = 0.09
  색상: 0.92 → 0.92 × 0.25 = 0.23
  방향: 0.85 → 0.85 × 0.25 = 0.21
  ─────────────────────────────
  총점: 0.77 ✅ 높은 점수!

후보 B:
  IoU: 0.7 → 0.7 × 0.4 = 0.28
  크기: 0.85 → 0.85 × 0.1 = 0.085
  색상: 0.15 → 0.15 × 0.25 = 0.0375
  방향: 0.3 → 0.3 × 0.25 = 0.075
  ─────────────────────────────
  총점: 0.4775 ❌ 낮은 점수

→ 후보 A를 같은 사람으로 선택!
```

---

#### 4️⃣ 교차 상황 특별 처리

**교차 감지 조건**:
```java
// 1. 두 사람이 충분히 가까움
float distance = sqrt((x1-x2)² + (y1-y2)²);
boolean isClose = (distance < 평균너비 × 1.2);

// 2. 서로 반대 방향으로 이동
float dotProduct = vx1*vx2 + vy1*vy2;  // 속도 내적
boolean oppositeDirection = (dotProduct < 0);

// 교차 상황!
if (isClose && oppositeDirection) {
    // 특별 처리 적용
}
```

**교차 시 처리 방법**:
```java
// 1. 속도 벡터 1.5배 부스트
person1.boostVelocity(1.5f);
person2.boostVelocity(1.5f);

// 2. 방향 점수 가중치 유지 (0.25)
// → 빠른 움직임으로 방향 정보가 더 신뢰도 높아짐
```

**왜 1.5배 부스트?**
```
일반 상황:
  속도: (10, 5)
  예측 위치: 현재 + (10, 5)

교차 상황:
  속도: (10, 5) × 1.5 = (15, 7.5)
  예측 위치: 현재 + (15, 7.5)
  
→ 더 큰 이동을 예측하여 빠른 움직임 대응
→ 방향 정보의 신뢰도 향상
→ ID 스위칭 방지 ✅
```

**코드 구현**:
```java
// SimpleTracker.java
private void detectCrossings(List<Detection> detections, boolean[] matched) {
    for (int i = 0; i < persons.size() - 1; i++) {
        for (int j = i + 1; j < persons.size(); j++) {
            TrackedObject person1 = persons.get(i);
            TrackedObject person2 = persons.get(j);
            
            // 거리 계산
            float distance = calculateDistance(person1, person2);
            float avgWidth = (person1.width + person2.width) / 2;
            
            // 겹침 확인
            if (distance < avgWidth * 1.2f) {
                // 방향 내적 계산
                float dirDot = person1.vx * person2.vx + 
                               person1.vy * person2.vy;
                
                // 반대 방향이면 교차 중
                if (dirDot < 0) {
                    // 속도 부스트 적용
                    person1.boostVelocity(1.5f);
                    person2.boostVelocity(1.5f);
                    
                    Log.d(TAG, "교차 감지: ID " + person1.id + 
                          " ↔ ID " + person2.id);
                }
            }
        }
    }
}
```

---

#### 개선 결과

**Before (문제 있는 방식)**
```
사람 A (ID 3, 빨간 옷) →
                           ← 사람 B (ID 5, 파란 옷)

IoU만 사용:
├─ 빠르게 움직여서 IoU 낮음
├─ 두 사람이 겹쳐서 IoU 혼란
└─ 결과: ID 3 ↔ ID 5 스위칭 ❌

교차 후:
사람 A (ID 5로 변경!) ❌
사람 B (ID 3으로 변경!) ❌
```

**After (개선된 방식)**
```
사람 A (ID 3, 빨간 옷) →
                           ← 사람 B (ID 5, 파란 옷)

다중 특징 사용:
├─ IoU: 낮음 (0.3)
├─ 색상: 빨간 옷 → 빨간 옷 (0.9) ✅
├─ 방향: 오른쪽 → 오른쪽 (0.85) ✅
└─ 속도 부스트: 1.5배 적용 ✅

교차 후:
사람 A (ID 3 유지!) ✅
사람 B (ID 5 유지!) ✅
```

**개선 효과 비교**

| 상황 | Before (IoU만) | After (다중 특징) |
|------|--------------|-----------------|
| **빠른 움직임** | ID 손실 (새 ID 부여) | 속도 예측으로 ID 유지 ✅ |
| **사람 교차** | ID 스위칭 발생 | 색상+방향으로 ID 유지 ✅ |
| **일시적 가림** | ID 손실 | 색상 정보로 복구 ✅ |
| **동일 의상** | ID 혼란 | 방향 정보로 구분 ✅ |

**실제 개선 결과**

![ID 추적 개선](docs/id-tracking-solved.gif)

> 🟢 **해결**: 교차 상황에서도 ID가 안정적으로 유지되는 모습

---

#### 학습 및 느낀 점

**1. 알고리즘 설계의 중요성**

> "같은 YOLO-NAS 모델을 사용해도, 추적 알고리즘을 어떻게 짜느냐에 따라 성능이 천차만별이었습니다."

- **모델은 도구일 뿐**: YOLO-NAS는 "이 위치에 사람이 있다"만 알려줌
- **알고리즘이 핵심**: "이 사람이 이전의 그 사람과 같다"는 것은 우리가 증명해야 함
- **특징 선택의 중요성**: 어떤 특징(색상, 방향, 속도)을 사용할지가 성능을 결정

**2. 문제 정의의 중요성**

처음에는 "IoU가 높으면 같은 사람"이라는 단순한 가정에서 출발했지만, 실제 상황을 관찰하며 문제를 재정의했습니다:

- **질문 1**: "빠르게 움직이는 사람은 왜 ID를 잃을까?"
  - → 답: IoU가 낮아지기 때문 → 해결: 속도 예측 추가

- **질문 2**: "교차 시 왜 ID가 바뀔까?"
  - → 답: 두 사람의 IoU가 비슷해지기 때문 → 해결: 색상 정보 추가

- **질문 3**: "어떻게 하면 몇 프레임 뒤의 이 사람이 같은 사람임을 증명할까?"
  - → 답: 불변 특징(색상) + 연속성(속도) 결합

**3. 다양한 시도와 실험**

문제 해결 과정에서 시도했던 방법들:

- ✅ **상체/하체 색상 분리**: 상의와 하의 색깔을 각각 추출 → 효과적!
- ✅ **중앙 영역만 추출**: 가장자리 배경 노이즈 제거 → 정확도 향상!
- ✅ **속도 부스트**: 교차 시 방향 정보 신뢰도 증가 → ID 유지 성공!
- ❌ **얼굴 특징 사용**: 해상도 낮고 각도 변화에 민감 → 채택 안 함
- ❌ **DeepSORT**: 모바일 환경에서 너무 무거움 → 커스텀 알고리즘 개발

**4. 모바일 AI의 현실적 제약**

- **연산량 제한**: 복잡한 알고리즘은 프레임 드롭 유발
- **최적화의 중요성**: 
  - 색상 추출을 전체 박스가 아닌 중앙 60%만 → 연산량 40% 감소
  - 교차 감지를 모든 프레임이 아닌 매칭 실패 시에만
    - 1단계: 높은 IoU(0.5 이상)로 확실하게 매칭되는 것들 먼저 처리
    - 교차 감지: 1단계에서 매칭 안 된 객체들만 대상으로 교차 상황 확인
    - 2단계: 남은 객체들을 색상, 방향 등 추가 특징으로 매칭
- **Trade-off 고려**: 정확도와 속도의 균형점 찾기

**5. 실전 경험의 가치**

> "이론으로는 간단해 보였지만, 실제 구현하며 수많은 엣지 케이스를 마주했습니다."

- 두 사람이 완전히 겹쳐서 한 명처럼 보일 때
- 세 명 이상이 동시에 교차할 때
- 조명 변화로 옷 색깔이 달라 보일 때
- 카메라 각도 변화로 바운딩 박스 크기가 급변할 때

이러한 경험을 통해 **"완벽한 알고리즘은 없으며, 상황에 맞는 최선의 해법을 찾는 것"**이 중요함을 배웠습니다.

**6. 가중치 튜닝의 예술**
```java
// 최종 가중치
점수 = IoU × 0.4 + 크기 × 0.1 + 색상 × 0.25 + 방향 × 0.25
```

이 가중치는 **수십 번의 실험**을 통해 도출되었습니다:

- 처음: IoU × 0.8 + 나머지 × 0.2 → IoU 과의존으로 교차 시 실패
- 시도 2: 색상 × 0.5 + 나머지 → 조명 변화에 취약
- 시도 3: 방향 × 0.5 + 나머지 → 정지 상태에서 ID 손실
- **최종**: 균형 잡힌 가중치로 모든 상황에서 안정적 추적 달성 ✅

---

#### 기술적 성과 요약

| 구분 | 개선 내용 | 효과 |
|------|----------|------|
| **추적 방식** | IoU 단독 → 다중 특징 (IoU + 색상 + 속도 + 방향) | ID 유지율 95% 이상 달성 |
| **색상 추출** | 전체 박스 → 중앙 60% + 상하체 분리 | 배경 노이즈 제거, 정확도 향상 |
| **속도 예측** | 없음 → 이동 평균 필터 적용 | 빠른 움직임에서도 ID 유지 |
| **교차 처리** | 없음 → 속도 부스트 + 방향 가중치 | 교차 시 ID 스위칭 방지 |
| **연산 최적화** | 매 프레임 전체 연산 → 필요 시에만 | CPU 사용률 30% 감소 |

---



## 📦 레포지토리 구조

이 조직은 Store Shield 프로젝트의 각 모듈을 독립된 레포지토리로 관리합니다.

| 레포지토리 | 설명 | 기술 스택 |
|-----------|------|----------|
| **[StoreShield-app](https://github.com/Store-Shield/StoreShield-app)** | 사장님용 관리 앱 | Flutter, Dart |
| **[yolo-nas-app](https://github.com/Store-Shield/yolo-nas-app)** | CCTV AI 영상 분석 앱 | Android (Java), YOLO-NAS |
| **[server](https://github.com/Store-Shield/server)** | 백엔드 서버 및 키오스크 | Flask, Socket.IO, MySQL |

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
