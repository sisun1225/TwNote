# 알고리즘


### 선형검색
처음부터 하나하나 다 찾아봐야함   

### 이진탐색
임의로 고른 중간값의 반을 제거하며 큰지 작은지를 통해서 찾아가는것   
정렬된 리스트에서 원하는 항목을 찾기에 효율적임   
원리는 범위를 계속 파악해가는 것   
[참고](https://github.com/sisun1225/AlgorithmPractice/blob/master/src/algorithm/Pra0000.java)

### 스왑함수
두 변수의 값으로 서로 교환하는 동작을 수행  
java에서는 구현 불가능
* Call by value(값에 의한 호출)  
인자로 받은 값을 복사하여 처리  
[참고](https://github.com/sisun1225/AlgorithmPractice/blob/master/src/algorithm/Pra0001.java)
* Call by reference(참조에 의한 호출)  
인자로 받은 값의 주소를 참조하여 직접 값에 영향을 줌  
* 값을 복사하여 처리하느냐, 직접 참조하느냐의 차이  
[참고](https://github.com/sisun1225/AlgorithmPractice/blob/master/src/algorithm/Pra0002.java)

### 선택 정렬
가장 작은 카드를 찾아서 첫번째 카드와 바꾸고  
두번째 작은 카드를 찾아서 두번째 카드와 바꾸고  
세번째 작은 카드를 찾아서 세번째 카드와 바꾸는 과정을 계속 반복하면서 정렬한다.  
[참고](https://github.com/sisun1225/AlgorithmPractice/blob/master/src/algorithm/Pra0003.java)

### 삽입정렬
자료 배열의 모든 요소를 앞에서부터 차례대로 이미 정렬된 배열 부분과 비교하며 정렬을 완성해가는 알고리즘  
카드를 예로 들면 선택된 카드를 앞에서부터 차례대로 비교해서 알맞은 위치에 삽입한다. 

### 재귀
알고리즘을 설계할때 동일한 문제의 조금 더 작은 경우를 해결함으로써 문제를 해결하는 것  
컴퓨터 과학에서는 자신을 정의할때 자기 자신을 재 참조 하는 방법을 뜻한다고 한다    
*팩토리얼  
사물의 순서를 정할때 얼마나 많은 방법이 있는지 구할때 유용  
[참고](https://github.com/sisun1225/AlgorithmPractice/blob/master/src/algorithm/factorial.java)

### 유클리드 호제법 
2개의 자연수 또는 정식의 최대공약수를 구하는 알고리즘  
호제법이란 두 수가 서로 상대방 수를 나누어서 결국 원하는 수를 얻는 알고리즘
