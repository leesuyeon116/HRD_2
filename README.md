## DB

```sql
-- course_tbl 테이블 생성
CREATE TABLE course_tbl(
    id VARCHAR2(5) NOT NULL,
    name VARCHAR2(40),
    credit NUMBER(6),
    lecturer VARCHAR2(10),
    week NUMBER(2),
    start_hour NUMBER(4),
    end_hour NUMBER(4),
    PRIMARY KEY(id)
);

-- lecturer_tbl 테이블 생성
CREATE TABLE lecturer_tbl(
    idx NUMBER(6) NOT NULL,
    name VARCHAR2(10),
    major VARCHAR2(40),
    PRIMARY KEY(idx)
);

-- course_tbl 데이터 삽입
INSERT INTO course_tbl VALUES('10001', '애플리케이션 배포', 2, '1', 1, 0900, 1100);
INSERT INTO course_tbl VALUES('10002', '프로그래밍 언어 활용', 2, '2', 2, 0900, 1200);
INSERT INTO course_tbl VALUES('10003', '응용SW기초기술 활용', 3, '6', 3, 0900, 1200);
INSERT INTO course_tbl VALUES('10004', '화면구현', 3, '4', 4, 0900, 1200);
INSERT INTO course_tbl VALUES('20001', '애플리케이션 태스트 수행', 2, '5', 1, 1300, 1600);
INSERT INTO course_tbl VALUES('20002', 'SQL 활용', 3, '5', 2, 1500, 1800);
INSERT INTO course_tbl VALUES('20003', 'UI 테스트', 3, '6', 3, 1330, 1530);
INSERT INTO course_tbl VALUES('30001', '화면 설계', 2, '3', 4, 1330, 1530);
INSERT INTO course_tbl VALUES('30002', '네트워크 프로그래밍 구현', 3, '3', 5, 0900, 1200);
INSERT INTO course_tbl VALUES('40001', '스마트문화앱구현', 3, '2', 5, 1300, 1600);

-- lecturer_tbl 데이터 삽입
INSERT INTO lecturer_tbl VALUES(1, '김교수', '소프트웨어공학');
INSERT INTO lecturer_tbl VALUES(2, '이교수', '프로그래밍');
INSERT INTO lecturer_tbl VALUES(3, '박교수', '네트워크');
INSERT INTO lecturer_tbl VALUES(4, '우교수', '운영체제');
INSERT INTO lecturer_tbl VALUES(5, '최교수', '자료구조');
INSERT INTO lecturer_tbl VALUES(6, '임교수', '인공지능');
