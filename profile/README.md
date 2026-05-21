<p align="center">
  <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/images/main.png" width="800" alt="SAN Main Banner"/>
</p>

# SAN : Scrap And Notify

> **개발자를 위한 지식을 수집하고 연결하는 AI 지식 리콜 서비스**

SAN은 개발자가 GitHub, 공식 문서, 기술 블로그, 메모, 캡처 등 여러 곳에 흩어져 저장한 지식을 빠르게 수집하고, 현재 작업 맥락에 맞게 다시 연결해 주는 AI 기반 지식 관리 서비스입니다.

단순히 자료를 저장하는 데서 끝나지 않고, 수집된 정보를 **AI 지식 카드**로 구조화하고, GitHub 활동과 현재 화면 맥락을 기반으로 필요한 순간에 다시 떠올릴 수 있도록 돕습니다.

---

## 🪄 프로젝트 소개

개발 과정에서는 수많은 자료를 찾고, 읽고, 저장합니다. 하지만 실제로는 저장한 자료가 다시 활용되지 못한 채 흩어지는 경우가 많습니다.

- 예전에 봤던 문서를 다시 찾기 어렵습니다.
- 특정 문제를 해결하며 남긴 메모가 현재 작업과 연결되지 않습니다.
- GitHub, 블로그, 공식 문서, 캡처 자료가 각각 분리되어 관리됩니다.
- 같은 내용을 반복해서 검색하거나 다시 정리하는 비용이 발생합니다.

**SAN(Scrap And Notify)** 은 이 문제를 해결하기 위해, 개발 지식을 **수집 → 구조화 → 연결 → 리콜**하는 흐름을 하나의 서비스로 제공합니다.

사용자는 필요한 정보를 원탭으로 저장하고, SAN은 저장된 지식을 AI로 정리한 뒤 현재 개발 맥락에 맞는 관련 지식과 복습 내용을 제공합니다.

---

## 🪄 프로젝트 기간

2026.04 ~ 204.05

---

## 🪄 기획 배경

개발자의 지식은 한곳에 머물지 않습니다. GitHub 커밋, README, 기술 문서, 블로그, 개인 메모, 오류 해결 과정, 캡처 이미지처럼 다양한 형태로 누적됩니다.

하지만 대부분의 지식 관리 도구는 **저장**에 초점을 맞추고 있어, 저장 이후의 활용 흐름이 자연스럽지 않습니다. 필요한 순간에 과거 지식을 다시 꺼내려면 사용자가 직접 검색어를 떠올리고, 저장 위치를 기억하고, 다시 맥락을 복원해야 합니다.

SAN은 이런 반복 비용을 줄이기 위해 다음과 같은 방향을 목표로 합니다.

- 지식 저장 장벽을 낮춘다.
- 비정형 정보를 AI가 구조화한다.
- GitHub 기반 개발 흐름을 초기 컨텍스트로 활용한다.
- 현재 보고 있는 내용과 과거 지식을 자동으로 연결한다.
- 하루 1회 리콜로 학습 흐름을 지속시킨다.

---

## 🪄 핵심 기능

### 1. 원탭 지식 수집

> **빠른 입력, 낮은 저장 장벽**

- 드래그, 단축키, 캡처, 링크 저장 등을 통해 필요한 정보를 빠르게 수집
- 사용자의 명시적 액션 기반으로 정보를 저장해 불필요한 노이즈 최소화
- 공식 문서, 기술 블로그, 에러 메시지, 코드 스니펫, 메모 등 다양한 형태의 개발 지식 기록
- 수집 즉시 이후 요약, 태깅, 검색, 추천에 활용할 수 있는 원본 데이터로 저장

---

### 2. GitHub 기반 초기 컨텍스트 확보

> **개발 흐름 반영, 콜드 스타트 완화**

- GitHub 레포지토리를 연동해 README, 커밋, 개발 기록을 기반으로 초기 맥락 구성
- 별도의 수동 입력이 많지 않아도 사용자의 기술 관심사와 학습 흐름을 파악할 수 있도록 설계
- 서비스에서 정리된 학습 내용을 Markdown 형태로 자동 정리
- GitHub 레포에 학습 기록을 축적해 개인 개발 히스토리와 지식 관리 흐름 연결
- 수집된 GitHub 정보는 이후 추천, 요약, 리콜의 기반 데이터로 활용

---

### 3. 실시간 컨텍스트 기반 추천

> **현재 맥락에 맞는 지식 연결**

- 사용자가 현재 보고 있는 문서, 코드, 오류, 기술 키워드를 기준으로 관련 과거 지식 탐색
- 관련 기록이 있을 경우 별도 검색 없이 즉시 다시 확인 가능
- 연결할 데이터가 부족한 경우 핵심 요약과 확장 학습 키워드 제공
- 반복 검색 비용을 줄이고, 이전 학습 내용이 현재 작업에 자연스럽게 이어지도록 지원

---

### 4. AI 지식 카드 생성

> **비정형 정보의 구조화**

- 수집된 원본 데이터를 카드 형태로 정리해 빠르게 파악할 수 있도록 구성
- 자동 태깅, 3줄 요약, 제목 생성, 핵심 키워드 추출 제공
- 원본 링크, 수집 시점, 출처, 관련 기술 스택 등 메타데이터 함께 저장
- 이후 검색, 추천, 리콜 과정에서 재사용 가능한 구조화 지식으로 관리

---

### 5. 하루 1회 학습 리콜

> **복습 자동화와 학습 흐름 유지**

- 전날 수집하거나 학습한 내용을 요약해 하루 1회 제공
- 과거 데이터와 연결해 흐름이 이어지는 복습 경험 지원
- 관련 개념, 다음 학습 키워드, 확장 자료 방향 제안
- 단발성 저장이 아닌 지속적인 학습 루틴으로 이어질 수 있도록 구성

---

## 🔁 서비스 흐름

<pre>
사용자 지식 수집
        ↓
원본 데이터 저장
        ↓
AI 지식 카드 생성
        ↓
태깅 · 요약 · 메타데이터 구조화
        ↓
검색/추천을 위한 컨텍스트 인덱싱
        ↓
현재 맥락 기반 추천 및 하루 1회 리콜
</pre>

---

## 📁 SAN 프로젝트 폴더 구조

<details open>
<summary><b>📦 Scrap-Notify Root</b></summary>

<pre>
├── 📁 .github/       
├── 📁 san-ai/         
├── 📁 san-backend/    
├── 📁 san-frontend/   
└── 📁 docs/
</pre>

</details>

<details>
<summary><b>📂 san-ai</b> - AI 지식 처리 모듈</summary>

- 수집 데이터 전처리
- AI 지식 카드 생성
- 자동 태깅 및 3줄 요약
- 컨텍스트 기반 추천 로직
- 하루 1회 리콜 생성
- 프롬프트 및 모델 응답 관리

</details>

<details>
<summary><b>📂 san-backend</b> - 백엔드 API 서버</summary>

- 사용자 인증 및 계정 관리
- 지식 수집 데이터 저장 및 조회
- GitHub 레포지토리 연동
- 지식 카드, 태그, 메타데이터 관리
- 추천/리콜 결과 제공 API
- 프론트엔드와 AI 모듈 간 데이터 흐름 제어

</details>

<details>
<summary><b>📂 san-frontend</b> - 프론트엔드 클라이언트</summary>

- 원탭 지식 수집 인터페이스
- 링크/캡처/텍스트 저장 화면
- AI 지식 카드 목록 및 상세 화면
- 현재 컨텍스트 기반 추천 화면
- 하루 1회 리콜 화면
- GitHub 연동 및 학습 기록 확인 화면

</details>

---

## 🛠️ 기술 스택


| 영역 | 내용 |
| :--- | :--- |
| Frontend | React + TypeScript 기반 대시보드 및 Chrome Extension 구현, 지식 수집/아카이브/카드 상세/추천/리콜 UI 개발, TanStack Query 기반 API 연동, Zustand 상태 관리, Tailwind CSS 기반 반응형 UI 및 디자인 시스템 적용 |
| Backend | Spring Boot 기반 REST API, 사용자 인증/JWT, 지식 데이터 관리, GitHub OAuth 연동, 추천/리콜 API 및 비동기 작업 처리 |
| AI | 요약, 태깅, 지식 카드 생성, 컨텍스트 추천, 학습 리콜 |
| Infra | 배포, CI/CD, 서버 운영, 문서/이미지 자산 관리 |
| Collaboration | Git, GitLab, Jira, Notion, Mattermost |

---

## 👥 팀원 소개

<table>
  <tr>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/유다현.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>유다현</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/김다희.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>김다희</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/박준아.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>박준아</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/권예지.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>권예지</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/이강희.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>이강희</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/방승재.jpg" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>방승재</b>
    </td>
    <td align="center" width="130">
      <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/members/이준영.png" width="100" height="100" style="width:100px; height:100px; object-fit:cover; border-radius:50%;" /><br />
      <b>이준영</b>
    </td>
  </tr>
  <tr>
    <td align="center">Fullstack</td>
    <td align="center">Backend</td>
    <td align="center">Backend</td>
    <td align="center">Fullstack</td>
    <td align="center">AI</td>
    <td align="center">AI</td>
    <td align="center">Infra</td>
  </tr>
</table>

## 🫧 협업 방식

### 1. Git / GitLab

- GitLab 기반 Issue, Branch, Merge Request 관리
- 기능 단위 브랜치 전략 적용
- Merge Request 기반 코드 리뷰 진행
- 커밋 메시지와 브랜치 네이밍 컨벤션 관리

### 2. Jira

- 작업 단위를 `Epic → Story → Task` 흐름으로 분류
- Sprint 단위로 목표를 설정하고 진행 상황 추적
- Story Point 기반으로 작업량 산정
- 진행 상태를 `To Do → In Progress → Done` 흐름으로 관리

### 3. Notion

- 회의록, 기획 문서, 컨벤션 문서 관리
- 기능 정의서, PRD, API 정책 등 산출물 정리
- 트러블 슈팅과 의사결정 내역 기록
- 프로젝트 일정 및 진행 상황 공유

### 4. Mattermost 및 커뮤니케이션

- 데일리 스크럼으로 진행 상황과 당일 목표 공유
- 파트별 PR 생성/머지 알림을 Mattermost 웹훅으로 연동
- 서비스 피드백 제출 알림을 Mattermost 웹훅으로 연동
- 이슈 발생 시 채널 기반으로 빠르게 공유 및 대응

---

## 📌 산출물

- [PRD](https://dahyeonii.notion.site/PRD-348b91841cc5801ca2f4f4e8fc9ddca1?source=copy_link)
- [API 명세서](https://dahyeonii.notion.site/API-348b91841cc58016926ffde539036052?source=copy_link)
- [ERD](https://www.erdcloud.com/d/9Sa6FqcxLBhJczpMp)
- [Git Convention](https://www.notion.so/dahyeonii/Git-Convention-33ab91841cc5816090f5e4927c669849?source=copy_link)
- [Front Convention](https://www.notion.so/dahyeonii/Frontend-Convention-33ab91841cc581a4bdcad85a505817a5?source=copy_link)
- [Back Convention](https://www.notion.so/dahyeonii/Backend-Convention-33ab91841cc5817598d7d0fe8016ae19?source=copy_link)
- [AI Convention](https://www.notion.so/dahyeonii/AI-Convention-344b91841cc5806f83b5ea30e2e1dfe3?source=copy_link)
---

## 📦 결과물

- [포팅 메뉴얼](https://raw.githubusercontent.com/Scrap-Notify/docs/main/result/포팅메뉴얼.docx)
- [최종 발표 자료](https://raw.githubusercontent.com/Scrap-Notify/docs/main/result/최종발표.pptx)
---

## 🖥️ 화면 구성

### 로그인

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/extension_guest_tutorial.gif" width="180" /> | **익스텐션 비회원 튜토리얼**<br/>비회원 사용자가 익스텐션 사용 흐름을 이해할 수 있도록 안내합니다. |
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/extension_first_user_tutorial.gif" width="180" /> | **익스텐션 첫 회원 튜토리얼**<br/>첫 로그인 사용자가 지식 수집과 저장 흐름을 자연스럽게 시작할 수 있도록 안내합니다. |

---

### 지식 숲

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/main.png" width="360" /> | **메인 대시보드**<br/>수집한 지식 카드와 학습 흐름을 한눈에 확인할 수 있는 메인 홈입니다. |
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/archive.png" width="360" /> | **아카이브**<br/>저장된 지식 카드를 모아보고 다시 탐색할 수 있는 공간입니다. |
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/detail.gif" width="360" /> | **지식 카드 상세보기**<br/>AI가 요약·태깅한 지식 카드의 상세 내용을 확인할 수 있습니다. |

---

### 익스텐션 기반 지식 수집

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/sidepanel_scrap.gif" width="360" /> | **사이드패널 스크랩**<br/>브라우저에서 드래그한 텍스트, 현재 페이지 링크, 화면 캡처를 확장 프로그램으로 바로 저장합니다. |

---

### GitHub 기반 학습 컨텍스트

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/github.png" width="360" /> | **GitHub 연동**<br/>GitHub 계정과 연결해 커밋 기반 학습 기록을 불러옵니다. |
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/star.png" width="360" /> | **GitHub Star 분석**<br/>사용자의 GitHub Star 레포지토리를 분석해 관심 기술 스택과 학습 컨텍스트를 불러옵니다. |

---

### TIL 학습 기록

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/TIL.png" width="360" /> | **TIL 자동 생성**<br/>오늘 학습한 내용을 AI가 자동으로 TIL 형태로 정리하고 Markdown 기록으로 남깁니다. |

---

### 학습 리콜 / 퀴즈

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/quiz.png" width="360" /> | **학습 리콜 퀴즈**<br/>이전에 학습한 내용을 퀴즈 형태로 복습하며 기억을 강화합니다. |

---

### 마이페이지

| 화면 | 설명 |
|---|---|
| <img src="https://raw.githubusercontent.com/Scrap-Notify/docs/main/assets/screenshots/profile.png" width="360" /> | **마이 프로필**<br/>사용자의 학습 기록, 단축키 설정, 리콜 알림 설정, GitHub 연동 정보를 확인할 수 있습니다. |


---

## ✅ MVP 목표

- 개발 지식의 저장 장벽을 낮추는 원탭 수집 경험 제공
- GitHub 기반 초기 컨텍스트 확보로 콜드 스타트 완화
- 수집된 비정형 정보를 AI 지식 카드로 구조화
- 현재 작업 맥락에 맞는 과거 지식 추천 제공
- 하루 1회 리콜을 통해 학습 지속성과 재활용성 강화

---

## 🧭 SAN이 해결하려는 문제

> 개발자는 이미 많은 지식을 쌓고 있지만, 그 지식은 필요한 순간에 다시 연결되지 못합니다.

SAN은 개발자가 저장한 지식이 단순한 기록으로 끝나지 않고, 현재의 문제 해결과 다음 학습으로 이어지도록 돕는 것을 목표로 합니다.

