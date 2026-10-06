<div align="center">

# 👋 Backend Developer | 최주영

### Java/Spring 기반의 백엔드 개발 역량과 개발·유지보수 실무경험을 갖춘 개발자입니다.

기존 시스템의 구조와 데이터 흐름을 이해하고,  
요구사항을 안정적으로 구현하는 백엔드 개발자를 지향합니다.

</div>

---

## 👨‍💻 About Me

- 약 2년간 **ERP 및 업무 시스템 개발·유지보수** 업무를 경험했습니다.
- **Java / Spring Boot / JPA / MySQL**을 기반으로 웹 서비스를 개발하고 있습니다.
- 기존 시스템의 구조를 파악하고 요구사항과 영향 범위를 확인한 뒤 기능을 개선하는 과정을 중요하게 생각합니다.
- Python을 활용한 **데이터 수집·전처리·검증 및 데이터 파이프라인 구축 경험**이 있습니다.
- 팀 프로젝트를 통해 Git 기반 협업과 배포 환경을 경험했습니다.

---

## 🛠 Tech Stack

### Backend

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?style=flat-square&logo=thymeleaf&logoColor=white)

### Data & Database

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![MSSQL](https://img.shields.io/badge/MSSQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)

### Collaboration & Tools

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

> Docker, GCP 등은 프로젝트의 개발·배포 환경에서 활용한 경험이 있습니다.

---

# 🚀 Projects

## 🐕 멍자국
### 반려견 산책 코스 추천 및 산책 기록 웹 서비스

**4인 Team Project · 2026.09.21 ~ 2026.10.02**

반려견과 함께하는 산책을 중심으로 **산책 코스 추천, GPS 산책 기록, 동행 모집 및 커뮤니티 기능**을 하나의 서비스로 구성한 팀 프로젝트입니다.

**Tech**

`Java 21` `Spring Boot` `Spring Security` `JPA` `MySQL` `Thymeleaf` `JavaScript` `Kakao Maps` `Docker`

**주요 기능**
- 반려견 산책 코스 조회 및 추천
- GPS 기반 산책 경로·거리·시간 기록
- 반려견 프로필 등록 및 관리
- 산책 동행 모집 및 신청 관리
- 산책 기록 및 활동 내역 조회
- 사용자 인증 및 데이터 접근 권한 처리

**담당 기능**
- 마이페이지 및 반려견 정보 연동
- 반려견 프로필 수정·삭제 및 소유자 권한 검증
- 개인/동행 산책 기록 조회 및 활동 상세 기능
- 동행 신청 관리 및 수락·거절 상태 처리
- 로그인 사용자를 기준으로 한 데이터 접근 제어
- 공용 Entity·Repository 변경 과정에서 기존 기능과의 충돌을 조정하고 통합

**Collaboration & Deployment**
- Git Feature Branch 기반 4인 협업
- 공용 Entity / Repository 변경에 따른 충돌 해결 및 통합
- Docker 기반 애플리케이션·MySQL·AI 서버 통합 실행
- HTTPS 환경으로 실제 서비스 배포 경험

**Troubleshooting**

최신 `dev` 브랜치를 병합하는 과정에서 Git LFS로 관리되는 약 1GB의 AI 도로망 데이터로 인해 병합이 장시간 정체된 것처럼 보이는 문제가 발생했습니다.

Git LFS 상태를 확인한 뒤 필요한 데이터를 정상적으로 내려받고, 이후 발생한 Entity·Repository·Service 및 공통 스타일 충돌을 최신 공용 구조를 기준으로 수동 통합했습니다. 이 과정에서 중복 Repository와 ID 타입도 함께 점검하고 기능을 다시 테스트하여 최종 통합 및 배포가 가능한 상태로 정리했습니다.

🔗 **Repository**  
https://github.com/dydwp/meongjaguk

---

## 🍽️ DiningCode Dynamic Crawling Pipeline
### 동적 웹 데이터 수집·전처리·검증 및 적재 파이프라인

**Personal Project · 2026.08.14 ~ 2026.09.13**

Selenium을 활용하여 동적 웹페이지의 음식점 데이터를 제한적으로 수집하고, **Raw → Interim → Processed → MySQL** 단계로 데이터를 처리하도록 구성한 개인 데이터 파이프라인 프로젝트입니다.

**Tech**

`Python` `Selenium` `BeautifulSoup` `pandas` `MySQL` `pytest` `Ruff` `GitHub Actions` `GCE`

**Pipeline**

`Selenium → Raw HTML → Extract → Interim → Preprocess & Validation → Processed → MySQL UPSERT`

**주요 구현**
- Selenium 기반 동적 음식점 데이터 수집
- Raw / Interim / Processed 데이터 계층 분리
- URL 기준 중복 제거 및 데이터 전처리·검증
- MySQL PK / UNIQUE 기반 UPSERT
- pytest 기반 단위 테스트 및 Ruff 정적 검사
- GitHub Actions를 이용한 CI 구성
- GCE 인스턴스 자동 시작 → 수집·처리 → DB 저장·검증 → 자동 종료 흐름 구성

**Result**
- 75개 수집 후보에서 URL 중복 제거
- **72개 음식점 × 16개 컬럼 데이터 구성**
- `restaurant_id`, `source_url` 중복 **0건**
- Processed CSV **72건 / MySQL DB 72건**
- 최종 상세 HTML **72건 / 수집 실패 0건**
- pytest **56개 테스트** 구성

**Troubleshooting**

GCE 환경에서 음식점 상세 페이지 응답이 지연되면서 Selenium Timeout이 발생했습니다.

페이지 로딩 전략을 조정하고 최대 대기시간과 재시도 로직을 적용했으며, 특정 음식점의 실패가 전체 Batch 중단으로 이어지지 않도록 개별 작업 단위의 예외 처리와 실패 로그를 구성했습니다. 이후 테스트와 정적 검사를 거쳐 재실행하여 최종 72건을 정상 수집했습니다.

🔗 **Repository**  
https://github.com/jy-0202/diningcode-dynamic-crawling-pipeline

---

## 🍴 Today Pick
### 조건 기반 맛집 탐색 및 추천 웹 서비스

**Personal Project · 2026.07 ~ 2026.09**

사용자의 지역·카테고리·가격·태그 조건을 기반으로 음식점을 탐색하고, 상세 정보와 지도 위치를 확인할 수 있도록 구현한 Spring Boot 기반 개인 웹 프로젝트입니다.

**Tech**

`Java 21` `Spring Boot 3.5` `JPA` `MySQL` `Thymeleaf` `JavaScript` `Kakao Maps`

**주요 구현**
- 지역·카테고리·가격대·태그 기반 조건 검색
- 음식점명 및 메뉴명 통합 검색
- 음식점 상세 정보 및 메뉴 조회
- 리뷰 및 평균 평점 조회
- Kakao Maps 기반 음식점 위치 표시
- Controller - Service - Repository 계층 구조로 기능 분리
- 지도 이동 범위에 따라 사이드바 음식점 목록과 결과 개수 동기화
- 자연어 추천 기능 확장을 위한 AI 추천 화면 및 Service·DTO 기본 구조 구성

**Troubleshooting**

지도 이동 시 현재 지도 영역의 음식점 개수는 변경되지만 사이드바에는 전체 음식점이 계속 표시되는 문제가 있었습니다.

Kakao Map의 `idle` 이벤트에서 현재 지도 영역을 가져오고 음식점 좌표가 영역 안에 포함되는지 확인하도록 처리했습니다. 동일한 기준으로 카드 표시 여부와 결과 개수를 갱신하여 지도와 사이드바가 일관된 데이터를 보여주도록 개선했습니다.

**Next**
- 현재 위치 기반 주변 음식점 조회 및 거리순 정렬
- 지도 이동 범위와 검색 조건을 결합한 탐색 기능
- 음식점·메뉴·리뷰 데이터를 활용한 추천 모델 검토
- 자연어에서 추천 조건을 추출하여 기존 조건 검색과 연계하는 AI 추천 기능 확장

🔗 **Repository**  
https://github.com/jy-0202/today-pick

---

## 💼 Experience

### (주)아이씨엔아이티
**ERP 개발·유지보수 | 2015.02 ~ 2017.02**

- 고객사 ERP 및 업무·웹 시스템 개발·유지보수
- 업무 화면, 출력 양식 및 데이터 표시 기능 수정
- 브랜드별 출력 양식, 바코드 라벨 및 행택 개발·수정
- 화면·Query·출력 오류 원인 분석 및 대응
- MSSQL 기반 운영 데이터 조회 및 기준정보 관리
- 개발 서버 반영 → 고객사 확인 → 운영 서버 적용 과정 수행
- 9개 브랜드별 ERP 출력 양식 및 가격·Lead Time 조건별 출력 로직 구현

---

## 🎓 Education & Certification

### 경기대학교
**컴퓨터과학과 | 2010.03 ~ 2015.02**

### 더조은컴퓨터아카데미 종로
**자바, 파이썬 활용 빅데이터분석과 AI SW개발자 양성과정**  
2026.03.30 ~ 2026.10.12 · 1,050시간

### Certification

- **정보처리기사** · 한국산업인력공단 · 2014.05

---

<div align="center">

### 📫 Contact

**GitHub** · https://github.com/jy-0202

</div>
