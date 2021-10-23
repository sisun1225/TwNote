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


### 
attr  
속성을 조회하거나 변경할 수 있는 메소드  

prop  
attr과 유사하지만 true/false 값을 가지는 속성들만을 위한 메소드  
예를들어 hidden. readonly, checked  
