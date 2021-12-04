# 간단정리

### SELECT
SELECT 칼럼명(*) FROM 테이블   

COUNT(칼럼명)  
LIMIT - 상위 몇개만나오도록 제한가능  
ORDERBY DESC  
ORDERBY ASC  
DISTINCT 칼럼명 - 셀렉트 부분에사용 중복제거  
NVL(SALARY, 0)

### WHERE

IN('1', '2') - 1이거나 2이거나  
NOT IN('1', '2') - 1과 2가 아닌거  
LIKE '%BOX%' -포함된단어 검색  
AND   
OR  

### GROUP BY 칼럼명
HAVING -그룹바이한 결과에 조건을 붙일때  

### JOIN

INNER JOIN(교집합)- 테이블 모두 공통으로 가지는 데이터  
INNER JOIN 테이블명  
ON 테이블A.칼럼명 = 테이블B.칼럼명  
alias(별명) 사용해서 테이블명을 줄여주는 것 가능  
from과 조인 테이블명에 AS 별명 사용  
LEFT JOIN


### SUBQUERY
select 안에 또다른 select가 들어가있는 것


### 테이블 생성
create table 테이블명  

create table tw_table(  
id number(7) primary key,  
name varchar2(25) not null );  

not null   
unique 중복데이터 입력 막는다  
primary key 자동으로 unique 부여 null허용 안함  
foreign key   
check  

### 테이블 구조 변경  
alter table 테이블명  
add~~~~  
modify ~~~~~  
MODIFY (phone varchar2(20) );  
drop ~~~~    
DROP COLUMN phone;  
set unused ~~~~  
SET UNUSED  COLUMN phone;  
rename ~~~~  
truncate ~~~~  
comment ~~~~  

### 트리거
SELECT * FROM ALL_TRIGGERS;  
DROP TRIGGER 트리거_이름


### ansi sql
미국 표준협회에서 표준 sql문을 정립 시켜 놓은 것...



### 오라클 계정 관련
계정 비밀번호 변경 - alter user 계정명 identified by 변경할 비밀번호;  
현재 접속중 - show user  
sys as sysdba  

sys  
오라클 시스템 총 관리자, db생성과 삭제도 가능하다  
sysdba 권한을 갖는다.  
유지,관리 생성하기위한 모든 권한을 갖는 계정  

system  
sys와 유사하지만 db생성과 삭제가 불가능하다  
생성된 db를 운영 관리하기 위한 관리자계정이다  

sysdba  
sysoper의 권한 뿐 아니라 데이터베이스 생성과 삭제, 오라클의 모든 권한을 갖는다.  


### INSTR
INSTR(문자열, 검색할 문자, 시작지점, n번째 검색단어) 함수는 찾는 문자의 위치를 반환
찾는 문자가 없으면 0을 반환
찾는 단어 앞글자의 인덱스를 반환


### SELECT IFNULL(Column명, "Null일 경우 대체 값") FROM 테이블명; 

