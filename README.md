# nextwebback
nextweb backend

# post

app.get -> 가져오다
app.post -> 생성하다
app.put -> 전체수정
app.delete -> 제거
app.patch -> 부분수정
app.options -> 찔러보기 (요청보낼수 있는지?)
app.head -> 헤더만 가져오기

# MySQL 설치

- MySQL 설치
https://dev.mysql.com/downloads/mysql/

DMG Archive 버전으로 다운로드

- MySQL 경로가기 및 접속
/usr/local/mysql/bin

mysql -u root -p

초기 비밀번호는 MAC 비밀번호
그뒤 Enter Password라고 뜨는 문구에서 MYSQL 비밀번호를 입력

- Database 생성
 CREATE DATABASE [DB명];
 show databases;

- 사용하기
 use [DB명];

- 테이블 생성
create table [테이블명] (
    [컬럼명] [type],
    [컬럼명] [type],
)

- root계정 비밀번호 변경

 alter user 'root'@'localhost' identified with mysql_native_password by '[password]';

# sequelize sequelize-cli mysql2

npm i sequelize sequelize-cli mysql2
npx sequelize init
    -> sequelize 세팅

mysql2는 node랑 mysql을 연결해주는 드라이버
sequelize는 자바스크립트로 sql을 조작할 수 있게 해준다

npx sequelize db:create   
    -> sequelize로 db생성