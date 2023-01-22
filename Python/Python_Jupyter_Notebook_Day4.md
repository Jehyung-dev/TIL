# Day4 : 함수 응용

- map(func, iterable) : 순회가능한(시퀀스) 데이터 구조의 모든 요소에 func을 적용해 결과를 돌려줌
  - 리스트 -> 문자열 : ''.join(map(str, 리스트 이름))
  - 리스트 안 문자 -> 리스트 안 정수 : list(map(int, 리스트 이름))
  - 같은 줄 숫자 입력 : map(int, input().split())
- filter(func, iterable) : func의 결과가 True인 것만 반환
  - list conprehension(ex) : [n*n for n in lst if n%1==1]
- zip(*iterables) : 복수의 iterable 객체를 모아 튜프로 반환
  - zip(a, b) -> (a1, b1), (a2, b2) 등 출력
- lambda : 계산한 결과를 반환하는 함수(return이 없음)
  - ex : list(map(lambda n : n%2, [1, 2, 3]) -> [1, 0, 1]
- 재귀 함수(recursive function) : 
