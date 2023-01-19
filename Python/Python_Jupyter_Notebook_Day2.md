## DAY2 : 제어문

- 조건문(Conditional Statement) : if문
  
  - if 조건 :    elif 조건 :     else:
    
    - if 조건 중첩 가능
  
  - 조건 표현식(Conditional Expression) : 조건에 따라 값을 정할 때
    
    - ex : print('짝수입니다.') if num%2 == 0 else print('홀수입니다.')

- 반복문(Loop Statement) : for, while
  
  - while : 조건이 참인 경우 반복적으로 실행
  - for : 순회가능한 객체의 요소를 순회
    - for i in 리스트/문자 -> print(i) 요소가 하나씩 나옴
  - 딕셔너리 순회 : for i in dict -> dict.key값이 나옴
  - enumerate() : index와 value를 같이 반환
  - List Comprehension : [expression for i in range(,)]
    - 초기화 할 때도 사용([[0]*5]로 하면 리스트 요소 변경시 다 바뀜)
  - Dictionary comprehension : {key: value for i in range( , )}
- 반복제어 : break, continue, for-else
  - break : 반복문을 종료
  - continue : continue 이후의 코드는 수행하지 않고, 다음 요소부터 반복을 수행
  - pass : 아무것도 하지 않음


