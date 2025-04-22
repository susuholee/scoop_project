# 🎯 Node.js-Project_Scoop

<p align="center">
  <img src="./public/images/logo.png" width="300px"/>
</p>
<h1 align="center">Scoop</h1>
<p align="center">
"Scoop은 '한 스푼 퍼올리다'는 의미를 담아, 사용자 지역 커뮤니티 정보를 손쉽게 접근하고 활용할 수 있도록 설계된 플랫폼입니다."
</p>

## 📖 목차
- [📺 프로젝트 소개](#-프로젝트-소개)
- [💬 프로젝트 개요](#️-개발-기간)
- [🔗 배포 주소](#️-개발-기간)
- [💁‍♂️ 팀원소개 및 역할](#️-팀원소개)
- [🖥 화면 구성 및 기능](#-화면-구성)
  - [📌 전체 카테고리 페이지](#-카테고리-페이지)
  - [📌 상세 카테고리 페이지](#-카테고리-페이지)
  - [📌 동호회 상세 페이지](#-카테고리-페이지)
  - [📌 동호회 추가/관리 페이지](#-카테고리-페이지)
- [🏷️ 주요 기능](#️주요-기능)
- [🛠 기술 스택](#-기술-스택)
- [👥 협업 도구](#-협업-도구)
- [📁 프로젝트 폴더 구조 ](#-프로젝트-폴더-구조)
---
## 📺 프로젝트 소개
"Scoop"은 관심사 기반 동호회를 누구나 쉽게 찾고 참여할 수 있도록 도와주는 웹 서비스입니다.  
사용자는 카테고리 또는 위치 기반으로 동호회를 탐색하고, 활동에 참여하거나 후기를 남길 수 있습니다.  
동호회 운영자는 활동 일정을 등록하고, 참여자 정보를 관리하며 리뷰 및 인증 시스템을 통해 활발한 커뮤니케이션을 유도할 수 있습니다.  
웹 기반으로 기획되었으며, 반응형 UI를 제공하여 모바일과 데스크탑 모두 대응합니다.

## 🖥 화면 구성

### 📌 메인 페이지
#### 담당 : 이수호
- 사용자는 지역 기반 또는 광역 기반으로 동호회를 선택해 지도를 통해  시각적으로 확인할 수 있습니다.

- 지도에서 지역 또는 광역 단위로 생성된 동호회를 클릭하면 해당 동호회의 상세 정보를 확인할 수 있습니다.

- 로그인하지 않은 비회원도 생성된 동호회를 조회할 수 있으며, 필터 기능도 사용할 수 있습니다.

![메인페이지](./public/images/main.jpg)
---

 ## 🏷️주요 기능
* 지역 및 지하철역 기반 동호회 추천

* 카카오맵 API를 활용한 동호회 위치 시각화

* 카카오 로그인 (카카오 Auth 연동)

* 동호회 상세 정보 열람 기능

* 동호회 등록, 수정 및 필터링 기능

* 카테고리별 동호회 목록 조회

* 동호회 좋아요(찜) 및 리뷰 작성 기능

* 캘린더를 통한 동호회 일정 등록

* 비회원 일일 게스트 참가 기능

* 동호회 활동에 따른 포인트 적립 시스템


## 🗓️ 개발 기간
* 2025.04.02(수) ~ 2025.04.18(금)

### 💁‍♂️ 팀원소개
---
<div style="text-align: center;">
  <div style="display: inline-block; margin: 0 20px; float :left;"> 
    <img src="https://github.com/susuholee.png" width="120"><br>
    <a href="https://github.com/susuholee"> 팀장 : 이수호</a>
  </div>
  <div style="display: inline-block; margin: 0 60px; float:left">
    <img src="https://github.com/zzeen2.png" width="120"><br>
    <a href="https://github.com/zzeen2">팀원 : 김지은</a>
  </div>

  <div style="display: inline-block; margin: 0 10px; ">
    <img src="https://github.com/Mr-Binod.png" width="120"><br>
    <a href="https://github.com/Mr-Binod">팀원 : 비노드</a>
  </div>
</div>

---
## 📡 API 문서

### 🔹 메인 페이지
- **`GET /`**
  - 메인 페이지를 반환합니다.

### 🔹 오른쪽 잉어영역 필터링
- **`GET /filter`**
  - 필터링된 동호회 목록 데이터를 반환합니다.

### 🔹 광역 기반 시/군구 데이터
- **`GET /api/area`**
  - 광역시도 기반의 시/군/구 GeoJSON 데이터를 json 형식으로 반환합니다.
  - **Response:** `application/json`

### 🔹 지하철 정보 데이터
- **`GET /api/station`**
  - 지하철 역사명, 위도, 경도 정보 GeoJSON 데이터를  json 형식으로 반환합니다.
  - **Response:** `application/json`

### 🔹 지하철역 마커 클릭 시
- **`GET /station`**
  - 사용자가 지하철 마커를 클릭했을 때 해당 역 관련 데이터를 반환합니다.

### 🔹 등록된 동호회 지역 데이터
- **`GET /area`**
  - 동호회가 등록된 시/군/구 데이터를 반환합니다.

---
## 🛠 기술 스택

- Frontend </br>

<img src="./public/images/html.png" alt="HTML5" width="80"/> 
<img src="./public/images/CSS3.png" alt="CSS3" width="80"/>
<img src="./public/images/JavaScript.png" alt="js" width="80"/>

- Backend </br>

<img src="./public/images/Node.js.png" alt="node.js" width="80"/> 
<img src="./public/images/Express.png" alt="CSS3" width="80"/>
<img src="./public/images/JavaScript.png" alt="js" width="80"/>

- Database </br>

<img src="./public/images/MySQL.png" alt="mysql" width="80"/> 
<img src="./public/images/Sequelize.png" alt="CSS3" width="80"/>

- 지도 API </br>

<img src="./public/images/kakaomaps.png" alt="mysql" width="120"/> 

## 🛠 협업 도구
---
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Github.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Notion.png?raw=true" width="80">
</div>

---

## 🛠 프로젝트 폴더 구조

📦scoopproject

 ┣ 📂controllers
 
 ┣ 📂json

 ┣ 📂lib

 ┣ 📂routers

 ┣ 📂views

 ┣ 📂public

 ┃ ┣ 📂css

 ┃ ┣ 📂js

 ┃ ┣ 📂js

 ┣ 📜server.js

 ┣ 📜README.md