# 에레메세지 메모

### the password has expired
비밀 번호 만료 되었다는 것  
hr 계정 비밀번호를 동일하게 한번 더 변경해주면된다.  
sqlplus 로 접속할경우 자동적으로 비밀번호 바꿔라고 나옴  


### Column count doesn't match value count at row 1
지정된 컬럼과 Value가 맞지 않을 경우에 발생  

### every derived table must have its own alias 에러

select count(*) from (select ~~~~~) 형식으로 조회할경우  
서브쿼리를 지정하지 않아서 에러가 생긴다  
서브쿼리 뒤에 명시적으로 워낳는 이름을 지정해주면 간단히 해결된다  
