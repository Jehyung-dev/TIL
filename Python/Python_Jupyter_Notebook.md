# Python

## DAY1 : 파이썬 기초

- 코드 구분 방법 : 들여쓰기 사용(Space : 4 = Tab : 1)



- 변수(Variable) : 컴퓨터 메모리의 저장된 객체를 참조하기 위한 이름
  
  - 객체(Object) : 값을 가진 것(ex : 숫자, 문자)
  
  

- 할당 연산자(Assignment Operator =) : 변수에 값을 할당( <- 방향으로 대입)
  
  - type(a) : 데이터 타입 확인
  
  - id(a) : 메모리 주소 확인

- 같은 값 동시 할당 : x = y = 10

- 다른 값 동시 할당 : x, y = '파이썬', 10

- 파이썬식 swap : a, b = b, a(값이 바뀜)



- 사용자 입력(input('입력 값 : ')) : 즉시 입력받아 문자열로 출력

- 식별자(Identifiers) : 변수, 함수 등을 식별하는 이름(ex : import, if)
  
  - 위의 이름으로 새로 만들면 기존의 동작이 실행되지 않음
  
  - 식별자에 새로 할당을 한 경우 del로 삭제하여 기존 기능을 돌릴 수 있음
  
  

- 주석(Comment) : 한 줄(#), 문단(''' 본문 ''' or """ 본문 """)



- 연산자(Operator)
  
  - 산술 연산자(Arithmetic Operator)
    
    - 덧셈 : +
    
    - 뺄셈 : -
    
    - 곱셈 : *
    
    - 나눗셈 : /(float), //(int로몫만 출력)
    
    - 나머지 : %
    
    - 거듭제곱 : **
    
    - 참고 : divmod(a, b) = (quotient(몫), 나머지(remainder))
  
  - 비교 연산자(Comparison Operator)
    
    - 미만 : <
    
    - 이하 : <=
    
    - 초과 : >
    
    - 이상 : >=
    
    - 같음 : ==
    
    - 같지 않음 : !=
    
    - 객체 아이덴티티 : is(ex : x is None -> True or False 출력)
    
    - 객체 아이덴티티가 아닌경우 : is not
      
      - 3 == 3.0(True), 'HI' == 'hi'(False)
  
  - 논리 연산자
    
    - and : a, b가 모두 True면 True
      
      - 3 and 5 경우처럼 보통 뒤의 값(5) 출력
      
      - 0 and 3 경우처럼 처음에 거짓이면 (0) 출력
    
    - or : a, b 중에 하나가 True면 True
      
      - 1 or 3 경우처럼 보통 앞의 값(1) 출력
      
      - 0 or 3 경우처럼 앞이 거짓이면 뒤의 값 확인 후 (3) 출력
    
    - not : not True -> False
    
    - 단축평가 : 첫 번째 값이 확실할 때 뒷 값은 확인하지 않아 속도 향상

- 연산자 우선순위
  
  - ()로  grouping
  
  - Slicing
  
  - Indexing
  
  - 제곱 연산자  : **
  
  - 단항 연산자 : +, -(부호)
  
  - 산술 연산자 : *, /, %
  
  - 산술 연산자 : +, -
  
  - 비트 연산자
  
  - 비교 연산자
  
  - 식별 연산자
  
  - 논리 연산자
  
  

- 자료형(Data Type)
  
  - 수치형(Numeric Type)
    
    - int(integer) : 정수, 오버플로우X(메모리가 넘어가는 상황X) -> 임의 정밀도 산술(가용 메모리로 수 표현)
    
    - float(floating point number) : 부동 소수점, 실수(2진수 표현 과정에 오류)
      
      - e지수도 사용가능(10의 몇 제곱인가)
      
      - (3.5 - 3.12) == 0.38 False ->해결법 :  round / 차이 <= 1e-10 / 
        
        차이 <= sys.float_info.epsilon / math.isclose(3.5, 3.12)
    
    
  
  - 문자열(String Type)
    
    - input()으로 입력받은 값은 str 타입
    
    - immutable : 문자열을 변경할 수 없음(ex : a[-1] = 3 추가 불가)
    
    - iterable : for과 같이 문자열 순회 가능함
    
    - 따옴표 : '' 과 "" 사용 가능
      
      - 삼중 따옴표 : """ 안에 작은 따옴표, 큰 따옴표 사용하고 개행없이 여러줄 출력 가능함"""
    
    - 이스케이프 시퀀스(Escape sequence)
      
      - \n : 줄 바꿈
      
      - \t : 탭
      
      - \r : 캐리지리턴(커서를 줄 맨 앞으로)
      
      - \0 : Null
      
      - \\\ : \
      
      - \' : 단일인용부호(')
      
      - \''' : 이중인용부호('')
    
    - String interpolation
      
      - %-formatting
        
        - %d : 정수(ex : '정수 %d' % a)
        
        - %f : 실수(ex : '실수 %f' % b)
        
        - %s : 문자열(ex : '문자열 %s' % c)
        
        - %y : 년
        
        - %m : 월
        
        - %d : 일
        
        - %A : 요일
      
      - str.format() : 다 가능(ex : 'Hello {}'.format(word))
      
      - f-string : f '문장 {변수명}'(ex : f '몇 년  {today : %y}' <- 출력형식 지정)
  
  
  
  - None Type : 값이 없음을 표현
  
  - 불린형(Boolean Type) : True와 False로 이뤄짐
    
    - bool() : T/F를 검증하는 함수(ex : '' False, [] False, [1,2,3] True)



- 컨테이너(Container) : 여러 개의 서로 다른 자료형 값을 저장할 수 있음
  
  - 시퀀스형 : 순서가 있는 데이터(ex : 리스트, 튜플, 레인지)
    
    - 순서가 있음
    
    - 특정 위치 데이터를 가르킬 수 있음
    
    - 리스트(List) : [] or list()로 생성
      
      - index : 0으로 시작, Negative Index는 뒤에서 -1부터 시작
    
    - 튜플(Tuple) : 리스트와 유사하지만 ()로 묶어 표현
      
      - 수정이 불가능
      
      - 단일 항목으로 만들 때는 쉼표가 필수(ex : t1 = 1,)
    
    - 레인지(range) : range(start, end, step)
      
      - range(m, n) : m부터 n-1까지 값을 가짐
    
    - 인덱싱(indexing) : 시퀀스 특정 인덱스 값에 접근할 수 있음
    
    - 슬라이싱 : 시퀀스를 특정 단위로 슬라이싱(ex : lst[start : end : step])
      
      - lst[::-1] : 값을 리버스로 출력
  
  - 비시퀀스형 : 순서가 없는 데이터(ex : 딕셔너리, 세트)
    
    - 딕셔너리(dictionary) : key와 value로 구성
      
      - dic = {Key1 : Value1, Key2 : Value2 ...}
      
      - 변경 불가능한 데이터만 가능
      
      - Key는 중복이 허용되지 않음
      
      - dict.keys() : key들 확인
      
      - dict.values() : values들 확인
      - dict.items() : key와 value들 확인
      
      

- 형변환(Type conversion, Typecasting) : 암시적 형변환, 명시적 형변환
  
  - 암시적 형변환(Implicit Typecasting) : 파이썬 내부적으로 자동 형변환
    
    - int + bool = int
    
    - int + float = float
  
  - 명시적 형변환(Explicit Typecasting)
    
    - string(정수 숫자) -> int
      
      - float(3.5) -> int(3) 가능 <-> str(3.5) -> int(3) 불가능
    
    - int -> string(모두 가능)
  
  - 컨테이너형 형변환 : 컨테이너형 -> range와 dictionary는 불가능
    
    - dictionary -> list, tuple, set의 경우 dict.keys()만 가능







## DAY2 : 제어문

- 조건문(Conditional Statement) : if문
  
  - if 조건 :    elif 조건 :     else:
    
    - if 조건 중첩 가능
  
  - 조건 표현식(Conditional Expression) : 조건에 따라 값을 정할 때
    
    - ex : print('짝수입니다.') if num%2 == 0 else print('홀수입니다.')



- 반복문(Loop Statement) : for, while
  
  - while : 조건이 참인 경우 반복적으로 실행
  
  - 
