# vs

### 모든 파일 한글 안깨지도록
TOOLS - Options - Enviroment - Documents 에서  
Save documents as Unicode when data cannot be saved in codepage 체크  
TOOLS - Options - Enviroment - Find and Replace 에서  
Display warning messages 체크  


### 특정 파일 한글 깨질때
다른이름으로 저장->save with encoding-> unicode(utf-8 with signature)........... 로 저장


### pm2 : 이 시스템에서 스크립트를 실행할 수 없으므로 ~~
windows PowerShell을 관리자 권한으로 실행  
Get-ExecutionPolicy 명령어로 확인  
Restricted 라고 뜬다면  
set-executionpolicy remotesigned 명령어 치고 y  
