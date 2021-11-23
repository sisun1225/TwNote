## meta og 태그
오픈 그래프는 어떤 html의 메타정보를 쉽게 표시하기 위해서   
메타정보에 해당하는 제목,설명 , 문서의 타입, 대표 url등 다양한 요소들에 대해서  
사람들이 통일해서 쓸수있도록 정의해놓은 프로토콜...  
(카카오에서 주소 보내면 이미지 제목 짧은 내용이 뜨는데 이런것이 og:image, og:title, og:description 이다)  

<meta property="og:type" content="website">  
<meta property="og:title" content="여기는 og title | 타이틀, 사이트 제목">  
<meta property="og:description" content="여기는 og description | 사이트에 대한 설명">  
<meta property="og:image" content="여기는 대표 이미지 URL">  
<meta property="og:url" content="여기는 사이트 URL">  

페이지 호출 시 동적으로 meta태그 추가 방법  
<script>  
    $("meta[property='og\\:title']").attr("content", '타이틀넣기' );  
    $("meta[property='og\\:url']").attr("content", '주소넣기' );                      
    $("meta[property='og\\:description']").attr("content", '페이지설명넣기' );  
    $("meta[property='og\\:image']").attr("content", '이미지주소넣기' );  
 
    // 동적으로 페이지 타이틀 수정하기  
    $(document).ready(function() {  
        document.title = '타이틀 변경하기';  
    });  
</script>   
