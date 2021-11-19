# JS

### ajax
자바스크립트를 이용해 서버와 브라우저가 비동기 방식(웹페이지를 새로 고침하지 않고 데이터를 불러오는 방식)으로 데이터를 교환할 수 있는 통신 기능
XMLHttpRequest 객체를 이용해서 페이지를 새로 고치지 않고 일부만 불러온 데이터를 보여줄 수 있음

### DOM
브라우저 화면에 보이는 요소를 조작하기 위한 기능들이 포함된 라이브러리 <br>
(document.getElementById, innerHTML 등등..)


### template literal
ES6에서는 백틱(back-tick)이라는 기호(`)를 사용하여 정의    
여러 줄에 걸쳐 문자열을 정의할 수도 있고, 자바스크립트의 변수를 문자열 안에 바로 연결할 수 있음  
\n 사용 할필요없이 바로 엔터쳐도 되고 변수의 경우 ${......}형식으로 바로 보여줄수있음  



### 변수
* var
변수 선언을 여러 번 해도 에러가 발생하지 않음  
그래서 보완하기 위해 es6부터 let, const가 추가됨  

* let
ES6에서 추가됨  
변수 재선언 불가능, 재할당 가능  

* const
ES6에서 추가됨  
변수 재선언 불가능, 변수 재할당 불가능  
의도치 않은 재할당 안전  

기본적으로 const를 사용하고 재할당이 필요한 경우에 한정적으로 let을 사용  


### 백틱
템플릿 리터럴 기능  
템플릿 리터럴은 여러 줄 문자열을 나타낼 수 있고  
변수를 삽입할 수 있음   
\n 과 "" + "" 등이 필요없이 다음줄로 변경하고 변수를 넣는 것이 자유로움  

### this
객체의 프로퍼티가 함수일 경우, 이 함수를 메서드라고 부른다. 메서드 내부 코드에서 사용된 this는해당 메서드를 호출한 객체로 바인딩 된다.

### window.onload  
페이지가 모두 로드되는 시점 실행  
window.onload = function () { ... }  

### $(document).ready()  
외부 리소스 및 이미지 로딩과 상관없이 DOM만 로드되면 바로 실행  
$(document).ready(function(){ … });    
$().ready(function(){ … });  
$(function(){ … });  


### json 데이터 형태 
{  
    "name": "철수",  
    "family": "가족1",  
    "age": 1,  
    "weight": 45  
}  

또는   

human이 배열의 이름   
"human": [  
    {"name": "철수", "family": "가족1", "age": 1, "weight": 45},  
    {"name": "영미", "family": "가족2", "age": 3, "weight": 45},  
    {"name": "철민", "family": "가족3", "age": 7, "weight": 45}  
]  



### 자바스크립트  
setTimeout(function() {  
  console.log('Works!');  
}, 3000);  
3초후에 코드를 실행해라!  

### document.body.appendChild
바디에 자식 요소로 넣어라


### 문자열을 배열로 변환
str.split();

str.split(" "); 단어별로  
str.split("");  글자별로
str.split(","); 특정 구분자로  