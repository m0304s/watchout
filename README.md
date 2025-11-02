<div align="center">
    <h1>🚧 WatchOut : AI 기반 건설현장 안전관리 플랫폼</h1>
    <p><i>산업재해 예방을 위한 AI 영상 분석 스마트 안전관제 시스템</i></p>
    <p><b>삼성 청년 SW·AI 아카데미 13기</b></p>
    <p><b>공통 프로젝트 부울경 1반 TEAM 02 </b></p>
    <p>🏆 <b>우수상 수상</b></p>
    <p>🏆 <b>영상 포트폴리오 입상</b></p>
</div>

---

![랜딩 페이지](docs/assets/image/Landing.jpg)

## 💡 프로젝트 소개
건설현장의 산업재해는 매년 반복적으로 발생하며, 주요 원인은 **안전장비 미착용**과 **즉각적인 사고 대응 부재**입니다.  
**WatchOut**은 **AI 영상 분석을 통한 실시간 안전장비 감지**와 **스마트워치를 활용한 낙상 감지·SOS 신고** 기능을 제공하여, 현장의 위험 상황을 신속히 파악하고 대응할 수 있는 **통합 안전관리 플랫폼**입니다.
### 🎬 소개 영상 (YouTube 바로가기)
[![Watch the video](https://img.youtube.com/vi/e0pj5abjkTo/hqdefault.jpg)](https://youtu.be/e0pj5abjkTo)

---

## 📑 목차
1. [💡 프로젝트 소개](#-프로젝트-소개)
2. [💡 주요 기능 및 플랫폼](#-주요-기능-및-플랫폼)
3. [🗓️ 개발 일정](#-개발-일정)
4. [📝 산출물](#-산출물)
5. [👨‍👩‍👧‍👦 개발 팀 소개](#-개발-팀-소개)
6. [🛠️ 기술 스택](#-기술-스택)
7. [🖥️ 서비스 화면](#-서비스-화면)
8. [📂 아키텍처 구조](#-아키텍처-구조)
9. [🏗️ 프로젝트 구조](#-프로젝트-구조)
10. [⚙️ 실행 방법](#-실행-방법)

---

## 💡 주요 기능 및 플랫폼
`WatchOut`은 AI 영상 분석을 중심으로 **웹, 모바일 앱, 스마트워치** 세 가지 플랫폼이 유기적으로 연동되는 통합 안전 관리 솔루션입니다.

---

### 🤖 AI 기반 안전 기능
* **주요 역할:** CCTV 영상을 실시간으로 분석하여 잠재적 위험을 사전 감지 및 예방
* **핵심 감지 기능:**
  * ⛑️ **안전장비 미착용 감지:** YOLACT 모델 활용, 작업자의 안전모 및 안전조끼 착용 여부 실시간 감지
  * 🚚 **중장비 위험 감지:** CCTV 영상 내 작업자와 중장비(지게차 등)의 위험한 접근 상황 감지
  * 👨‍ **안면인식 출입 관리:** ArcFace 모델 활용, 등록된 작업자의 현장 출퇴근 및 주요 구역 입출입 기록 자동화

---

### 💻 웹 플랫폼 (Web Platform)
* **주요 역할:** 현장 총괄 관리자를 위한 종합 관제 대시보드
* **핵심 기능:**
  * 📊 **종합 대시보드:** 실시간 안전 현황, **AI 감지 위반 통계**, 작업자 상태 등 현장 데이터 총괄 모니터링
  * 📹 **CCTV 실시간 모니터링 및 관리:** 다수 CCTV의 구역별 실시간 스트리밍 및 **AI가 감지한 위험 상황(안전장비 미착용, 중장비 접근 등) 확인**
  * 🚨 **통합 알림 관리:** 현장에서 발생하는 모든 안전 알림(**AI 감지**, 낙상, SOS 등)의 실시간 수신 및 이력 관리
  * 👥 **자원 통합 관리:** 현장 작업자, 작업 구역, 스마트워치 등 시스템의 모든 자원 등록 및 관리
  * 📢 **공지 관리:** 현장 전체 또는 특정 그룹 대상 중요 공지사항 발송

---

### 📱 모바일 앱 (Mobile App)
* **주요 역할:** 현장 관리자 및 작업자를 위한 실시간 현장 대응 및 정보 확인 도구
* **핵심 기능 (관리자용):**
  * 📹 **이동 중 CCTV 확인:** 모바일 환경에서 언제 어디서든 현장 CCTV 확인으로 즉각적인 상황 파악
  * 🚨 **실시간 위험 알림:** 푸시 알림을 통한 **AI 감지 위험 상황**, 낙상, SOS 등 즉시 인지 및 대응
  * 👥 **현장 작업자 관리:** 모바일에서의 작업자 상태 확인 및 관리
* **핵심 기능 (작업자용):**
  * 📢 **알림 수신:** 안전 관련 공지 및 위험 알림 수신
  * 📍 **작업 구역 확인:** 자신의 현재 작업 구역 정보 확인

---

### ⌚ 스마트워치 (Smartwatch)
* **주요 역할:** 작업자의 신체에 가장 가까운 곳에서 생명과 안전을 지키는 최전방 장비
* **핵심 기능:**
  * 🤕 **낙상 감지 & 자동 신고:** Health Services API 연동, 심각한 낙상 자동 감지 및 응답 부재 시 SOS 자동 전송
  * 🆘 **수동 SOS 신고:** 위급 상황 발생 시 버튼을 통한 즉각적인 긴급 구조 요청
  * 📍 **작업 정보 확인:** 할당된 작업 구역 및 담당 관리자 정보 확인

---

## 🗓️ 개발 일정

### **개발 기간** : 2025.08.25 ~ 2025.09.28 **(5주)**

- **1주차 (8/25 ~ 8/31)**: 프로젝트 기획 및 요구사항 분석
- **2주차 (9/1 ~ 9/7)**: 시스템 설계 및 기술 스택 선정
- **3주차 (9/8 ~ 9/14)**: 인프라 구축 및 기본 기능 구현
- **4주차 (9/15 ~ 9/21)**: AI 모델 연동 및 고도화
- **5주차 (9/22 ~ 9/28)**: 테스트 및 최적화
- **9/29**: 최종 프로젝트 평가

---

## 📝 산출물

### 1. 🔗 [기획서](https://phase-football-921.notion.site/261ab603db8b813c9841c3c24fa45eea?pvs=74)
### 2. 🔗 [기능 명세서](https://phase-football-921.notion.site/261ab603db8b81f78b06c520da6e7e1f?pvs=74)
### 3. 🔗 [ERD](https://www.erdcloud.com/d/YyZAC7CE8xsfReyes)
### 4. 🔗 [API 문서](https://phase-football-921.notion.site/API-25bab603db8b8090ac11f65f7fb4884e?pvs=74)

---
## 👨‍👩‍👧‍👦 개발 팀 소개
<div align="center">
<img src="docs/assets/image/팀사진.png" alt="팀사진" width="600"/>

### **🥢 최가네 사각김박**

AI 기반 건설현장 안전관리 플랫폼 WatchOut을 개발한 팀입니다. <br>
팀원 구성은 최씨 1명, 김씨 4명, 박씨 1명으로, 이를 합쳐 최가네 사각김박이라는 팀명을 지었습니다.

---
<table>
  <tbody>
    <tr>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/m0304s">
          <img src="docs/assets/image/민석.png" width="140px" alt="최민석"/>
        </a><br>
        <b><sub>최민석 (Team Leader)</sub></b><br>
        <sub><a href="https://github.com/m0304s">@m0304s</a></sub><br><br>
        <img src="https://img.shields.io/badge/Backend-0771A1?style=flat&logo=springboot&logoColor=white"/>
        <img src="https://img.shields.io/badge/Infra-FF9900?style=flat&logo=amazonaws&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>인프라 구축</li>
              <li>대시보드 API 개발</li>
              <li>FCM 알림 구현</li>
            </ul>
          </small>
        </div>
      </td>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/donggyu-kim12">
          <img src="docs/assets/image/동규.png" width="140px" alt="김동규"/>
        </a><br>
        <b><sub>김동규</sub></b><br>
        <sub><a href="https://github.com/donggyu-kim12">@donggyu-kim12</a></sub><br><br>
        <img src="https://img.shields.io/badge/Frontend-41B883?style=flat&logo=vue.js&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>모바일 화면 설계</li>
              <li>갤럭시 워치 API 연동</li>
            </ul>
          </small>
        </div>
      </td>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/yeneua">
          <img src="docs/assets/image/예나.png" width="140px" alt="김예나"/>
        </a><br>
        <b><sub>김예나 (FE Leader)</sub></b><br>
        <sub><a href="https://github.com/yeneua">@yeneua</a></sub><br><br>
        <img src="https://img.shields.io/badge/Frontend-41B883?style=flat&logo=vue.js&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>Capacitor 코드 연동</li>
              <li>웹 화면 설계</li>
            </ul>
          </small>
        </div>
      </td>
    </tr>
    <tr>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/khyunse0">
          <img src="docs/assets/image/현서.png" width="140px" alt="김현서"/>
        </a><br>
        <b><sub>김현서</sub></b><br>
        <sub><a href="https://github.com/khyunse0">@khyunse0</a></sub><br><br>
        <img src="https://img.shields.io/badge/Backend-0771A1?style=flat&logo=springboot&logoColor=white"/>
        <img src="https://img.shields.io/badge/AI-F78F1E?style=flat&logo=tensorflow&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>AI 모델 연동</li>
              <li>안전장비 미착용 감지 기능 개발</li>
            </ul>
          </small>
        </div>
      </td>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/KimHS17">
          <img src="docs/assets/image/환수.png" width="140px" alt="김환수"/>
        </a><br>
        <b><sub>김환수</sub></b><br>
        <sub><a href="https://github.com/KimHS17">@KimHS17</a></sub><br><br>
        <img src="https://img.shields.io/badge/Backend-0771A1?style=flat&logo=springboot&logoColor=white"/>
        <img src="https://img.shields.io/badge/Infra-FF9900?style=flat&logo=amazonaws&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>로그인/회원가입 API 개발</li>
              <li>웨어러블 디바이스 어플 개발</li>
            </ul>
          </small>
        </div>
      </td>
      <td align="center" style="border: none; padding: 15px;">
        <a href="https://github.com/Leehwa531">
          <img src="docs/assets/image/정훈.png" width="140px" alt="박정훈"/>
        </a><br>
        <b><sub>박정훈</sub></b><br>
        <sub><a href="https://github.com/Leehwa531">@Leehwa531</a></sub><br><br>
        <img src="https://img.shields.io/badge/Backend-0771A1?style=flat&logo=springboot&logoColor=white"/>
        <img src="https://img.shields.io/badge/AI-F78F1E?style=flat&logo=tensorflow&logoColor=white"/>
        <br><br>
        <div align="left">
          <small>
            <ul>
              <li>안면인식 모델 개발</li>
              <li>웨어러블 디바이스 어플 개발</li>
            </ul>
          </small>
        </div>
      </td>
    </tr>
  </tbody>
</table>
</div>

---


## 🛠️ 기술 스택

<a name="techStack"></a>

### 🌕 Frontend
<div align="center">

![React](https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Capacitor](https://img.shields.io/badge/Capacitor-119EFF?style=for-the-badge&logo=capacitor&logoColor=white)<br>
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-181717?style=for-the-badge&logo=react&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-671DDf?style=for-the-badge&logo=axios&logoColor=white)

</div>

### 🔙 Backend
<div align="center">

![Java](https://img.shields.io/badge/Java-17-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.5.5-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)<br>
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-02569B?style=for-the-badge)

</div>

### 🤖 AI & Computer Vision
<div align="center">

![YOLACT](https://img.shields.io/badge/YOLACT-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![ArcFace](https://img.shields.io/badge/ArcFace-FF5722?style=for-the-badge&logo=pytorch&logoColor=white)

</div>

### 📱 Mobile & Watch
<div align="center">

![Android](https://img.shields.io/badge/Android-Kotlin-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Wear OS](https://img.shields.io/badge/Wear_OS-4285F4?style=for-the-badge&logo=wearos&logoColor=white)<br>
![Health Services API](https://img.shields.io/badge/Health_Services_API-34A853?style=for-the-badge&logo=google&logoColor=white)
![Wearable Data API](https://img.shields.io/badge/Wearable_Data_API-4285F4?style=for-the-badge&logo=google&logoColor=white)

</div>

### ☁️ Infra & DevOps
<div align="center">

![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)<br>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)<br>
![EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white)
![S3](https://img.shields.io/badge/AWS_S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)
![RDS](https://img.shields.io/badge/AWS_RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)

</div>

### 🗄️ Database
<div align="center">

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

</div>

### 🛠️ Tools
<div align="center">

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)<br>
![Jira](https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![MatterMost](https://img.shields.io/badge/MatterMost-0072C6?style=for-the-badge&logo=mattermost&logoColor=white)

</div>

---

## 🖥️ 서비스 화면

### 📱 모바일 앱

#### 🔐 로그인 & 계정
| 로그인 | 회원가입 | 안면인식 등록 |
| :---: | :---: | :---: |
| <img src="docs/assets/image/모바일-로그인.jpg" width="200"/> | <img src="docs/assets/gif/모바일-회원가입.gif" width="200"/> | <img src="docs/assets/gif/모바일-안면인식등록.gif" width="200"/> |

#### 🛠️ 현장 관리
| 작업자 관리 | CCTV 현장 관리 |
| :---: | :---: |
| <img src="docs/assets/image/모바일-작업자관리.jpg" width="200"/> | <img src="docs/assets/image/모바일-현장관리.jpg" width="200"/> |

#### 🚨 안전 알림
| 작업자 입출입 알림 | 안전장비 미착용 알림 | 중장비 접근 알림 | SOS 긴급 알림 |
| :---: | :---: | :---: | :---: |
| <img src="docs/assets/gif/모바일-입출입알림.gif" width="200"/> | <img src="docs/assets/gif/모바일-안정장비미착용알림.gif" width="200"/> | <img src="docs/assets/gif/모바일-중장비알림.gif" width="200"/> | <img src="docs/assets/gif/모바일-sos알림.gif" width="200"/> |

---

### ⌚️ 갤럭시 워치 앱
| 구역 정보 | 낙상 감지 | SOS |
| :---: | :---: | :---: |
| <img src="docs/assets/image/워치-구역정보.png" width="200"/> | <img src="docs/assets/gif/워치-낙상감지영상.gif" width="200"/> | <img src="docs/assets/gif/워치-수동sos.gif" width="200"/> |
| 낙상 감지 활성화 | 낙상 신고 완료 |  |
| <img src="docs/assets/image/워치-감지활성화.png" width="200"/> | <img src="docs/assets/gif/워치-낙상신고완료.gif" width="200"/> |  |


---

## 📂 아키텍처 구조

### 🏗️ System Architecture
![System Architecture](docs/assets/image/Architecture.jpg)

### 🌐 Network Architecture (Test & Production)
![Network Architecture](docs/assets/image/NetworkArchitecture.jpg)

- **사용자(User)** → Nginx(443) → Frontend / Backend
- **Backend** → DB(PostgreSQL), Cache(Redis), Messaging(Kafka)
- **AI 서버** → CCTV 영상 분석 → 안전장비 위반 감지 → Backend 전달
- **스마트워치** → 낙상 감지 → 모바일 앱 → Backend 알림
- **Jenkins** → CI/CD 파이프라인 관리

---

## 🏗️ 프로젝트 구조

### frontend-repo - React 웹 애플리케이션
<details>
<summary>frontend-repo/</summary>

```
frontend-repo/
|-- android/                # Capacitor Android bridge (Wear OS companion)
|   |-- app/
|   |-- build/
|   `-- gradle/
|-- docker/
|   |-- edge/
|   `-- frontend/
|-- public/
|   |-- fonts/
|   `-- firebase-messaging-sw.js
|-- scripts/
|   `-- copy-sw.js
|-- src/
|   |-- api/
|   |-- bootstrap/
|   |-- components/
|   |-- constants/
|   |-- features/
|   |-- hooks/
|   |-- layouts/
|   |-- notification/
|   |-- routes/
|   |-- stores/
|   |-- styles/
|   |-- types/
|   `-- utils/
|-- capacitor.config.ts
|-- package.json
|-- pnpm-lock.yaml
`-- vite.config.ts
```
</details>

### backend-repo - Spring Boot 백엔드

<details>
<summary>backend-repo/</summary>

```
backend-repo/
|-- src/
|   |-- main/
|   |   `-- java/watch/out/
|   |       |-- accident/         # 사고 이력 및 대응 관리
|   |       |-- announcement/     # 공지 게시 모듈
|   |       |-- area/             # 작업 구역 · 출입 제어
|   |       |-- auth/             # 인증 및 토큰 처리
|   |       |-- cctv/             # CCTV 연동 및 스트림 제어
|   |       |-- common/           # 공통 설정 · 예외 · 유틸리티
|   |       |-- company/          # 현장/기업 마스터 데이터
|   |       |-- dashboard/        # 대시보드 통계 API
|   |       |-- notification/     # FCM 알림 발송
|   |       |-- s3/               # 파일 업로드(S3)
|   |       |-- safety/           # 안전장비 위반 기록
|   |       |-- user/             # 사용자 · 역할 관리
|   |       `-- watch/            # 스마트워치 연동 API
|   `-- test/
|       `-- java/watch/out/
|-- dummy_data.sql
|-- build.gradle
|-- settings.gradle
|-- Dockerfile
`-- gradlew
```
</details>

### watch-repo - Wear OS 스마트워치 앱

<details>
<summary>watch-repo/</summary>

```
watch-repo/
|-- app/
|   |-- src/
|   |   |-- main/
|   |   |   |-- AndroidManifest.xml
|   |   |   |-- java/com/ssafy/watchout/
|   |   |   |   |-- core/          # DI, 서비스 및 계약 정의
|   |   |   |   |-- data/          # 원격 데이터 모델
|   |   |   |   |-- domain/        # Health Services 도메인 로직
|   |   |   |   `-- presentation/  # Wear Compose UI 화면
|   |   |   `-- res/               # 리소스 (레이아웃, 이미지 등)
|   |   `-- test/
|   |-- build.gradle.kts
|   `-- proguard-rules.pro
|-- build.gradle.kts
|-- gradle/
|   `-- wrapper/
|-- gradlew
`-- settings.gradle.kts
```
</details>

### ai-repo - 안전장비 미착용 및 중장비 감지 서비스

<details>
<summary>ai-repo/</summary>

```
ai-repo/
|-- main.py                    # Flask 진입점 (멀티 스트림 제어)
|-- config.py
|-- util/
|   |-- capture_utils.py
|   |-- cctv_bound.py
|   |-- kafka_client.py
|   |-- kafka_control_consumer.py
|   `-- stream_workers.py
|-- templates/
|   |-- form.html
|   `-- multi.html
|-- snapshot/                  # 탐지 스냅샷 예시
|-- weights/
|   `-- yolact_resnet101_safety_33_200000.pth
|-- yolactMaster/              # 커스텀 YOLACT 백본
|   |-- data/
|   |-- layers/
|   |-- scripts/
|   |-- utils/
|   `-- yolact.py
|-- check_bytes.py
|-- check_s3.py
```
</details>

### ai-repo2 - 얼굴 인식 서비스
<details>
<summary>ai-repo2/</summary>

```
ai-repo2/
|-- app/
|   |-- main.py                 # FastAPI 엔트리포인트
|   |-- adapters/               # 외부 연동 레이어 (S3, Redis 등)
|   |-- routes/                 # API 엔드포인트 정의
|   |-- services/               # ArcFace 추론 · 업무 로직
|   `-- config.py
|-- models/                     # 얼굴 인식 모델 자산
|-- scripts/
|   `-- run_local_registration.py
|-- requirements.txt
|-- evaluate_lfw.py
|-- test_api_request.py
`-- test_arcface.py
```
</details>


---

## ⚙️ 실행 방법

<details>
<summary>1. 환경 변수 설정</summary>

```bash
# API 설정
VITE_API_BASE_URL=https://j13e102.p.ssafy.io/api

# Firebase 설정
VITE_FIREBASE_API_KEY=AIzaSyBWaaDFnie2q0uxVsoKDJsxxer6h1DUh98
VITE_FIREBASE_AUTH_DOMAIN=watchout-238c7.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=watchout-238c7
VITE_FIREBASE_STORAGE_BUCKET=watchout-238c7.firebasestorage.app
VITE_FIREBASE_MESSAGING_SENDER_ID=276857840662
VITE_FIREBASE_APP_ID=1:276857840662:web:562f09d8f2913211314137

# Firebase VAPID Key
VITE_FIREBASE_VAPID_KEY=BEHWGdHjQhnW_MM32MDtb46uvYxA6HnN-FH5Z4R0NbN07UEn_rIABoTr7Hnz8cO1Bap4eeqnMuiwSMXWj8Ckm2E

# Firebase CDN URL
VITE_FIREBASE_CDN_URL=https://www.gstatic.com/firebasejs/9.0.0/

# API Timeout 설정 (ms)
VITE_API_TIMEOUT=30000
VITE_API_TIMEOUT_SHORT=10000

# 운영 환경 설정
VITE_IS_DEVELOPMENT=true
````

</details>

<details>
<summary>2. Docker 실행</summary>

```bash
# 전체 서비스 실행
docker-compose up -d

# 로그 확인
docker-compose logs -f

# 개별 서비스 빌드 & 실행 예시
# Backend
cd backend-repo
./gradlew build
docker build -t watchout/backend-app .
cd ..

# Frontend
cd frontend-repo
pnpm install
pnpm run build
docker build -t watchout/frontend-app .
cd ..

# AI Service
cd ai-repo
docker build -t watchout/ai-service .
cd ..

# (옵션) 재시작/중지
docker-compose restart
docker-compose down
```

**기본 접속(예시)**

* Frontend(Nginx 경유): `https://localhost` 또는 배포 도메인
* Backend(API): `http://localhost:8080`
* AI Service: 프로젝트 설정 포트(예: `:9000`)
* Swagger(사용 시): `http://localhost:8080/swagger-ui/index.html`

</details>

<details>
<summary>3. 개발 환경 실행 (로컬)</summary>

```bash
# Backend
cd backend-repo
./gradlew bootRun

# Frontend
cd frontend-repo
pnpm install
pnpm run dev   # 기본: http://localhost:5173

# AI Service
cd ai-repo
pip install -r requirements.txt
python main.py
```

**로컬 접속(예시)**

* Vite Dev Server: `http://localhost:5173`
* Spring Boot: `http://localhost:8080`

</details>

<details>
<summary>4. 자주 발생하는 이슈 & 팁</summary>

* **포트 충돌**: 사용 중인 포트 확인 → `lsof -i :PORT` 후 프로세스 종료
* **CORS 오류**: 개발 모드에서는 `VITE_API_BASE_URL`이 백엔드와 일치하는지 확인
* **이미지 캐시 문제**: 프런트 변경 후 `pnpm run build` 재실행 또는 브라우저 캐시 비우기
* **Docker 빌드 실패**: `docker builder prune`로 캐시 정리 후 재빌드
* **푸시 알림(Firebase)**: 서비스 워커 파일과 `VAPID_KEY`가 일치하는지 확인

</details>


<div align="center">
  <p>🚧 <strong>Watchout</strong> - 건설현장의 안전을 지키는 스마트 솔루션 🚧</p>
</div>
