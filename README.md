# 오라클 활용 console 게시판 만들기

## 순수 자바를 사용하고 JDBC를 통해서 오라클 DB와 연동하는 콘솔형 게시판 형성

## 1. 목표
* 글쓰기, 내용보기, 수정, 삭제 기능 구현
* 댓글쓰기, 답글쓰기 는 다음에 구현한다.


## JAVA에서 DB 어플리케이션 구현 순서
1. VO 생성
- TABLE과 같은 구조로 생성을 하고
-- member 변수 이름도 TABLE의 칼럼과 일치 시킨다.

2. DAO 생성
-- DAO는 DB로부터 데이터를 읽고, 쓰고, 수정하고, 삭제할 때 사용할 class
- 실제적으로 DB에 연결하고 , CRUD를 구현하는 부분
- 클래스를 생성하기 앞서 interface를 작성을 하고
- interface를 implement해서 클래스를 구현한다.

3. Service 생성
- Dao와 사용자 UI 사이에서 데이터를 선 가공하는 여러 method를 구현한다.
