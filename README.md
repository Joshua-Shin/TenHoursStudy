TenHoursStudy : 개인 웹 애플리케이션 개발 프로젝트
--------------
- 현재 배포중인 Static 웹 사이트
    - https://joshua-shin.github.io/TenHoursStudyHtml
    - [저장소](https://github.com/Joshua-Shin/TenHoursStudyHtml)

-------------------
### 목차
- [프로젝트 목적](#프로젝트-목적)
- [개발 환경](#개발-환경)
- [진행 상황](#진행-상황)

-------------------

### 프로젝트 목적
- 기획부터 배포 및 유지 보수까지 웹 개발의 전체 라이프 사이클을 경험해본다.
- 웹 애플리케이션를 개발에 필요한 지식들을 순차적으로 학습하고 이를 곧바로 적용함으로서 학습 효과를 높인다.
- TenHoursStudy 사이트의 목적
    - 하루 10시간 공부 챌린지를 성공하기 위한 가이드를 제시해준다.

-------------------

### 개발 환경
#### Backend
- Gradle - Groovy
- Java 11, Spring Boot(2.7.8)
- H2, Jpa, Web, Lombok, Thymeleaf, DevTools

#### Frontend
- HTML5, CSS3

#### Tools
- IntelliJ, GitHub, VSCode,

-------------------

### 진행 상황
- [x] 순수 html, css로만 static 웹 사이트 구현
- [ ] 스프링 부트, JPA로 crud 게시판 페이지 구현
- [ ] 스프링 부트 프로젝트에 순수 html 파일도 통합
- [ ] AWS에 스프링부트 프로젝트 올리기
    - [ ] aws 요금 폭탄을 맞지 않기 위해 무엇을 유의해야하는지 학습
    - [ ] Elastic Beanstalk 학습
        -  아마 additional resource로 db를 붙이는 기능이 있을거야. 아니면 Amazon RDB랑 연동하거나.
- [ ] CI/CD 구성
- [ ] spring 스큐리티, Oauth로 로그인 기능 구현
- [ ] contact 페이지 구현
    - [ ] form 페이지 만들기. name, email, comment 적어서 submit 하면 내 메일로 보내지게.

-------------------
### 고민중...
- 결국 내가 원하는 형태까지 가려면 스프링부트 프로젝트는 EC2에 넣어야 되고, DB는 RDS로 해야되고, github의 Travis CI와 AWS의 CodeDeploy로 배포해야된다는거네.
  thymeleaf랑 웹MVC 익혀서 일단 로컬에서 돌아가는 게시판 만들어. 그리고 그걸 AWS로 올리고, 후에 static.html을 스프링부트 프로젝트에 통합시키면 되잖아.
- 아.. 이래서 CI/CD가 필요한거네.
  로그인 기능 하나 개발한다음에 다시 클라우드에 새로 서버 올리고, 뭐 하나 개발한다음에 다시 또 클라우드에 새로 올리고 하는게 아니라.
  개발한거 바로바로 통합시키고 배포시키기 위해서 하는거구나..


