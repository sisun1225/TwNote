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