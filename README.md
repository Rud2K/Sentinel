<img src="https://github.com/Rud2K/Sentinel/raw/master/Sentinel/src/main/resources/static/Team_Logo.png" alt="팀 로고" width="100"/>
<br>

### 🖥️ 프로젝트 소개
  - DBMS 실시간 공격 탐지 및 차단 시스템입니다.

### ⏰ 개발 기간
  - 2023.11.07 ~ 2024.01.02

### 🧑‍🤝‍🧑 멤버구성
```java
Sentinel<Leader> 박희승 = new Sentinel<Leader>("프로젝트 관리", "탐지 엔진 개발");
Sentinel<Member> 정찬진 = new Sentinel<Member>("탐지 엔진 개발");
Sentinel<Member> 최경호 = new Sentinel<Member>("관리자 UI/UX 개발", "관리자 UI/UX 디자인");
Sentinel<Member> 한주연 = new Sentinel<Member>("관리자 UI/UX 개발", "관리자 UI/UX 디자인");
Sentinel<Member> 양주목 = new Sentinel<Member>("관리자 UI/UX 디자인");
```

### 🛠️ 개발 환경
```javascript
const Sentinel = {
  Language: "Java 17(JDK 17), C/C++, HTML5, CSS3, JavaScript",
  IDE: "Eclipse 4.29.0",
  Framework: "Spring Boot 3.1.6",
  Database: "MariaDB 10.3.39, MySQL",
  ORM: "MyBatis 3.0.3",
  Librarie: "jQuery, Chart.js",
  Server: "Rocky Linux 8.6, Apache Tomcat"
};
```

### 📌 주요기능
#### 로그인
  - DB 값 검증
  - PW 암호화
  - 로그인 시 세션(Session) 생성
#### 대시 보드
  - 가장 최근의 일, 월 단위 로깅 데이터 확인
#### 정책 관리
  - 탐지 정책의 추가, 수정, 삭제 가능
  - 정책 이름을 클릭해 해당 정책 상세 조회 가능
  - 정책 수정 및 삭제(활성화 되어있는 정책만), 활성화/비활성화 시 엔진에게 UDP 신호를 전송해 엔진이 정책을 다시 읽어옴
  - 유효기간이 만료된 정책은 Spring Boot의 @Scheduled를 사용하여 자동으로 비활성화 가능
#### 로그 조회
  - 필터링 된 로그 목록 조회 및 특정 로그 상세 조회 가능
  - 상세 조회 페이지에서는 특정 네트워크 패킷의 상세 정보 확인 및 이상 행동이나 패턴을 식별 가능
#### 설정
  - 엔진에서 읽을 conf 파일을 관리자 UI에서 수정 가능
  - 기존 PW 값 검증 후 관리자 PW 변경 가능

### 📷 실행 화면
<img src="https://github.com/Rud2K/Sentinel/blob/master/Sentinel/src/main/resources/static/img/%ED%99%94%EB%A9%B4_%EB%A1%9C%EA%B7%B8%EC%9D%B8.png" alt="로그인 화면"/><br>
<img src="https://github.com/Rud2K/Sentinel/blob/master/Sentinel/src/main/resources/static/img/%ED%99%94%EB%A9%B4_%ED%99%88.png" alt="홈 화면"/><br>
<img src="https://github.com/Rud2K/Sentinel/blob/master/Sentinel/src/main/resources/static/img/%ED%99%94%EB%A9%B4_%EC%A0%95%EC%B1%85%EB%A6%AC%EC%8A%A4%ED%8A%B8.png" alt="정책 관리 화면"/><br>
<img src="https://github.com/Rud2K/Sentinel/blob/master/Sentinel/src/main/resources/static/img/%ED%99%94%EB%A9%B4_%EB%A1%9C%EA%B7%B8%EB%A6%AC%EC%8A%A4%ED%8A%B8.png" alt="로그 조회 화면"/><br>
<img src="https://github.com/Rud2K/Sentinel/blob/master/Sentinel/src/main/resources/static/img/%ED%99%94%EB%A9%B4_%EC%83%81%EC%84%B8%EB%A1%9C%EA%B7%B8.png" alt="상세 로그 조회 화면"/>

### ⚙️ 엔진
#### 보안 엔진 Github Link: https://github.com/Salieri1126/Sentinal_C
