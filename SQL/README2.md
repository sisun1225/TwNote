# 노트2

### NoSql
관계형 데이터베이스가 아닌 sql  
관계형 데이터베이스는 데이터의 중복을 제거하고 무결성을 보장하가위해 정규화하는데  
이러한 정규화가 과도한 join으로 성능 저하(상황에 따라 다름)  
초고용량 데이터 처리 등 성능에 특화된 목적을 위해, 비관계형 데이터 저장소에, 비구조적인 데이터를 저장하기 위한 분산 저장 시스템   
* 장점...  
불필요한 join의 최소화  
유연성 있는 서버 구조 제공  
비정형 데이터 구조로 설계비용 감소  
읽고 쓰기가 빠르고 빅데이터 처리가 가능  
비용이 적고 분산 처리 병렬처리가 가능 



### Document DB
JSON, XML과 같은 Collection 데이터 모델 구조를 채택  

### node.js
크롬 v8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임  
node.js는 이벤트 기반, 논 블로킹 i/o 모델을 사용해 가볍고 효율적  
node.js의 패키지 생태계인 npm은 세계에서 가장 큰 오픈 소스 라이브러리 생태계  

## mongodb
특징  
document  
base  
open source  

RDBMS가 database>tables>rows>columns로 구성되어있는데 documents는 row에 해당  
계층은 database>collections>documents>field로 비슷  

document 기반 데이터베이스는 rdbms와 다르게 자유롭게 데이터 구조를 잡을 수 있음  
BSON으로 데이터가 쌓이기때문에 array나 nested로 데이터를 쉽게 넣을 수 있음  

objectId는 pk와 같이 고유한 키를 의미  

mongodb는 sql이 아니라 별도로 제공하는 api(SpiderMonkey 자바스크립트 엔진)를 통해 데이터를 조작  

### bson
json 형태의 문서를 바이너리 형태로 인코딩한 바이트 문자열  
c언어의 데이터 형태를 사용  
