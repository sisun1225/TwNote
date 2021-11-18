# jquery

### .val()
* 밸류값 가져와라~  
var jb = $( '#abcd' ).val();  
* 밸류값 넣어라~  
$( '#abcd' ).val( 'ABCDE' );  

### 밸류값 가져오기  
* id 값 기준 가져오기  
$('#abcd').val();   
* class 값 기준 가져오기  
$('.abcd').val();  
* name 값 기준 가져오기  
$('input[name=abcd]').val();  


###메모

<script>  
    function fnGetdata(){  
        var obj = $("[name=SEQ_CHK]");  
        var chkArray = new Array(); // 배열 선언  
 
        $('input:checkbox[name=SEQ_CHK]:checked').each(function() { // 체크된 체크박스의 value 값을 가지고 온다.  
            chkArray.push(this.value);  
        });  
        $('#hiddenValue').val(chkArray);  
        
        alert($('#hiddenValue').val()); // 아래 체크박스가 모두 체크되어 있다면 1,2,3,4 가 출력 된다.  
          
    }  
  
</script>  


### 속성값 
attr  
속성을 조회하거나 변경할 수 있는 메소드  

prop  
attr과 유사하지만 true/false 값을 가지는 속성들만을 위한 메소드  
예를들어 hidden. readonly, checked  

### if문
조건에 변수만 들어간다면 변수에 값이 있는지 없는지 확인 후 실행  



###each를 통하여 doc 부분의 텍스트를 가져와야한다면...
<문서>
    <doc>1</doc>
    <doc>2</doc>
    <doc>3</doc>
    <doc>4</doc>
    <doc>5</doc>
    <doc>6</doc>
    <doc>7</doc>
    <doc>8</doc>
</문서>
$(xml).find('문서').find('doc').each(function(index, item){  
    console.log($(this).text());
});
index 키값
item  키의 값 


#### .load()
페이지를 동적으로 교체할때 사용


### 아이디에 동적으로 페이지 넣기
$(document).ready(function(){  
$("#test").load("test.html");  
});  
