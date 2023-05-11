# camagru (2023.05.08 ~ )
웹캠과 기존 사진을 활용하여 합성 사진을 생성하고 게시하는 웹 어플리케이션

## 개발 과정
### 요구사항 정리
1. 일반 요구사항
    - image alpha channel, superposition
    - public, likable, commentable
    - server-side : 언어 자유(but, PHP Standard Library 내에서 동일한 기능이 존재해야 함)
    - client-side : HTML, CSS(CSS framework 사용 가능), JavaScript만 사용 가능
    - 최신 container 사용
    - web server : 자유
    - 호환성 : Firefox (>= 41), Chrome (>= 46)
2. 공통 요구사항
    - MVC pattern
    - page layout, Responsive design
    - 유효성 검사
    - 보안 취약점 최소화
      - 비밀번호 암호화
      - XSS(Cross Site Scripting)
      - content 유효성 검사
      - SQL Injection
      
3. 유저 요구사항
    - 이메일 회원가입 유효성 검사
    - 가입 확인 메일
    - 비밀번호 찾기(재등록)
    - 로그아웃(모든 페이지에서)
    - 이름, 비밀번호, 메일 변경
4. 갤러리 요구사항
    - 사진 나열(생성순)
    - like, comment(연결된 유저만)
    - 알림 기능(on/off)
    - pagination
5. 편집 요구사항
    - 인증(본인만. 본인이 아닌 경우 거절 화면 제공)
    - main : preview, capture
    - sub : 이전 사진들
    - 중첩 이미지 확인
    - webcam, image
    - 사진 삭제 기능(인증)
6. Bonus
    - AJAX
    - Preview
    - 무한 scroll
    - SNS 공유
    - animated GIF render
  
### 개발 환경 구축
nginx, tomcat, postgreSQL

1. docker file
2. docker compose file
3. configuration file

### 디자인, DB 설계
### 개발
### 테스트 / 요구사항 충족 여부 확인
### 평가
