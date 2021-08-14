# Python 코딩 학습

## Python 도장

### Unit 1-7 파이썬 기본 활용법

- Unit 1 : 소프트웨어 교육과 파이썬

- Unit 2 : 파이썬 설치
- Unit 3 : "Hello, world!"로 시작
- Unit 4 : 기본 문법 알아보기
- Unit 5 : 숫자 계산하기
- Unit 6 : 변수와 입력 사용
- Unit 7 : 출력 방법

### Unit 8-12 자료형

- Unit 8 : 불과, 비교, 논리 연산자
- Unit 9 : 문자열 사용
- Unit 10: 리스트와 튜플 사용하기
- Unit 11: 시퀀스 자료형 활용
- Unit 12 : 딕셔너리 사용

#### Unit 9

"", ' '을 사용하여 문자열 입력

``` python
hello = 'Hello, world'
hello2 = "Hello, world"
```

''' ''', """ """도 사용 가능

```python
multiline = '''
Hello!
world
'''
```

' ', " ", \를 문자열에서 사용하기 위해서는 \을 추가적으로 붙이거나 외부에 따음표를 다시 씌운다.

``` python
C = 'python isn\'t difficult.'
S = 'Alice said "I love you."'
```

#### Unit 10

리스트, 튜플 모두 인수를 모아둔 개념이지만, 리스트는 수정 가능하고 튜플은 수정이 불가능한 차이가 있다.

- list

```python
a = [5, 10, 18, 20, 25, 30] # 리스트(list)
b = ['james', 17, 175.3, True] # 다양한 type의 인수 사용가능
c = list(range(10)) # list 함수로 생성 가능
```

- 튜플

```py
a = (38, 21, 41, 50)
a = tuple(range(10))
a = [1, 2, 3]
tuple(a)
```



### Unit 13-15 조건문

- Unit 13 : If 조건문
- Unit 14 : else 사용(두 방향으로 분기하기)
- Unit 15 : elif를 사용

### unit 13

if 조건문은 특정 조건일 때 코드를 실행하는 문법이다. 

```bash
x= 10
if x == 10: 
    print('Value is 10')

```

python은 들여쓰기로 조건문 내용을 구분한다. 그렇기에 띄어쓰기에 주의할 것

- 중첩 if 조건문 사용하기

```bash
x=15
if x > 10:
  print('10보다 큰 수입니다.')
  if x ==15:
    print('15입니다.')
  if x == 20:
    print('20입니다.')
```



### unit 14

- else 사용하기

if 조건문에 충족하지 않을 경우 실행되는 코드

```bash
x = 8
if x==10:
  print('It is 10')
else:
  print('It is %s' %x)
```

- 3항 연산자

```bash
# 3항 연산자의 경우 :가 안들어간다.
y = 'even' if x%2 == 0 else 'odd'
y
```



### unit 15

- elif를 사용하여 여러 방향으로 분기할 수 있다.

- ```bash
  x=20
  if x==10:
      print('It is 10.')
  elif x==20:
      print('It is 20.')
  else:
      print('It is not 10, 20')
  ```

```bash
# 숫자- 입력, 3의 배수면 Fizz 출력, 5의 배수면 Buzz, 15의 배수면 Fizzbuzz
number = int(input())
if number % 15 == 0: # 제일 엄격한 조건을 앞에 두기
    print('Fizzbuzz')
elif number % 5 ==0:
    print('Buzz')
elif number % 3 ==0:
    print('Fizz')
else:
    print('이 수는 3, 5, 15의 배수가 아닙니다.')
```



### Unit 16-19 반복문

- Unit 16 : for 반복문
- Unit 17: while 반복문
- Unit 18 : break, continue 반복문 제어
- Unit 19 : 계단식 별 출력



### Unit 22-26 리스트, 튜플, 딕셔너리, 세트

- Unit 22 : 리스트와 튜플 응용
- Unit 23 : 2차원 리스트 사용하기
- Unit 24 : 문자열 응용하기
- Unit 25 : 딕셔너리 응용
- Unit 26 : 세트 사용하기



### Unit 27-33 함수

- Unit 27 : 파일 사용하기
- Unit 29 : 함수 사용
- Unit 30 : 함수의 인수(위치 인수, 키워드 인수)
- Unit 31 : 재귀호출
- Unit 32 : 람다 표현식
- Unit 33 : 클로저 사용



### Unit 34-36 클래스

- Unit 34 : 클래스 사용
- Unit 35 : 클래스 속성, 정적, 클래스 메서드
- Unit 36 : 클래스 상속



### Unit 38-45 

- Unit 38 : 예외 처리 사용하기
- Unit 39 : 이터레이터 사용
- Unit 43 : 정규표현식 사용
- Unit 44 : 모듈과 패키지 사용
- Unit 45 : 모듈과 패키지 만들기

