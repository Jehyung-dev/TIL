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
  
  - 




