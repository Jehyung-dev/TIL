## Day3 : 함수

- 함수(Function) : 특정 명령을 수행하는 함수 묶음

- 모듈(Module) : 함수 / 클래스의 모음 단위 

- 패키지(Package) : 프로그램과 모듈의 묶음

- 라이브러리(Library) : 패키지의 모음

- 함수의 사용 이유 : 가독성, 재사용성, 유지보수

- def : 함수의 선언

- parameter : 함수는 매개변수를 줄 수 있음

- return : 함수는 동작 후 결과 값을 반환
  
  - 한 개의 객체만 반환

- 함수의 호출 : 함수명() 의 형태

- 함수의 출력(Output) : return(a, b) 하여 2개 출력가능

- 함수의 입력(Input)
  
  - 매개변수(parameter) : def func(x)에서 x
    
    - 입력을 받아 함수 내부에서 활용되는 변수
    
    - 함수를 정의하는 부분에서 확인
  
  - 전달인자(argument) : func(50)에서 50
    
    - 실제로 전달되는 값
    
    - 함수를 호출하는 부분에서 사용
  
  - 위치 인자(Positional Arguments) : 인자의 위치에 따라 함수에 전달된다.(ex : func(a, b) <=> func(5, 100))
  
  - 키워드 인자(Keyword Arguments) : 직접 변수의 이름으로 특정 인자를 전달(ex : func(a, b) <=> func(b = 100, a = 5))
    
    - 단, func(5, b = 100) 가능 / func(a = 5, 100) 불가능
  
  - 기본 인자 값(Default Argument Values) : 함수 정의 시 기본값을 지정하여 보다 적은 인자로 함수를 호출
    
    - func(a = 10) return a
    - 기본 인자 값(b = 0) 외에 함수 내 값(b = 3)이 있다면 그대도 계산(b = 3)

- Scope : Python의 범위
  
  - 전역 스코프(global scope) : 어디든 코드가 참조 가능
  
  - 지역 스코프(local scope) : 함수 내부에서만 참조 가능
  
  - 전역 변수(global variable) : 전역 스코프에 정의된 변수
  
  - 지역 변수(local variable) : 로컬 스코프에 정의된 변수
    
    - 지역 스코프에서 전역 스코프의 변수는 참조 가능(연예인 -> 시민 집O)
    
    - 전역 스코프에서 지역 스코프의 변수는 참조 불가능(시민 -> 연예인 집X)

- 변수의 수명주기(Lifecycle)
  
  - 빌트인 스코프(built_in scope) : 파이썬이 실행된 후 영원히 유지
  
  - 전역 스코프(global scope) : 이름 선언 이후 인터프리터 끝까지
  
  - 지역 스코프(local scope) : 함수가 호출되고 종료될 때까지

- 이름 검색 규칙 : 파이썬에서 식별자들은 이름공간(namespace)에 저장됨
  
  - LEGB Rule : 이름을 찾아가는 순서
    
    - Local scope : 로컬 함수
    
    - Enclosed scope : 특정 함수의 상위 함수
    
    - Global scope : 함수 밖의 변수 or import 모듈
    
    - Built-in scope : 파이썬 안에 내장된 함수 or 속성
      
      - ex : global 선언 변수면 전역 변수 값으로 나옴
