# JS

### 콤보(select)박스
<script>  
function handleOnChange(e) {  
  // 선택된 데이터 가져오기  
  const value = e.value;  
  
  // 데이터 출력  
  document.getElementById('result').innerText  
    = value;  
}  
</script>  
<select name="language" onchange="handleOnChange(this)">  
  <option value="korean">한국어</option>  
  <option value="english">영어</option>  
</select>  
<div id='result'></div>  

### 라디오버튼
<input type="radio" name="chk_info" value="HTML">HTML  
<input type="radio" name="chk_info" value="CSS" checked="checked">CSS  
<input type="radio" name="chk_info" value="웹디자인">웹디자인  


### 체크박스
<input type="checkbox" name="chk_info" value="HTML">HTML  
<input type="checkbox" name="chk_info" value="CSS" checked="checked">CSS  
<input type="checkbox" name="chk_info" value="웹디자인">웹디자인  

