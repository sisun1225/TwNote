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



rownum  
rowid  


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
