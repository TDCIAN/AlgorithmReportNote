# AlgorithmReportNote
Algorithm Report Note

### Quiz 1 (2021/03/18 ~ 2021/03/21)
Q1. 다음 중 여러개의 데이터를 나열하는 데에 쓰이며, 한 번 정의된 후 데이터를 변경할 수 없는 자료형을 고르시오.
(1) 리스트
(2) 튜플 
(3) 숫자형
(4) 람다

Q2. 다음 중 딕셔너리 자료형에 대한 설명으로 옳지 않은 것을 고르시오.
(1) Key와 Value의 쌍으로 이루어지는 자료형이다.
(2) 딕셔너리에는 여러 개의 자료를 삽입할 수 있다.
(3) 딕셔너리에서는 동일한 Value를 가진 자료가 존재할 수 없다. 
(4) 딕셔너리 자료형은 Key를 이용해 매우 빠르게 자료를 검색할 수 있다.

Q3. 메모리에 할당되지 않고, 즉시 실행하는 형식의 함수는 어떤 함수인가?

Q4. 다음 중 파이썬의 가상환경을 구성하는 이유로 옳지 않은 것을 고르시오
(1) 원하는 패키지만을 설치하여, 깔끔한 환경을 구성할 수 있다.
(2) 가상환경 별로 미리 작성된 코드를 활용하여 빠르게 프로토타이핑 할 수 있다.
(3) 프로젝트 별로 프로그램이 실제로 실행될 환경에서 개발/테스트할 수 있다.
(4) 특정 버전의 패키지를 설치하여 테스트해 볼 수 있다.

Q5. 다음 중 조건문에 대한 설명으로 옳은 것을 고르시오
(1) 파이썬의 조건문은 if문 계열 (if, if ~ else, if elif ~ else)이 유일하다.
(2) 조건문에는 반드시 bool 타입만이 사용될 수 있다.
(3) [조건문 1] and [조건문 2] 형식으로 작성된 경우, 두 조건문이 반드시 모두 실행된다.
(4) 조건문 내부에서 새로운 변수를 선언하더라도 조건문 외부에서 참조하는 데에 문제가 없다.

Q6. 다음과 같은 출력이 나오도록 코드의 빈 공간을 작성하시오
a = ['파','이','썬','썬','썬','썬','즐','즐','즐','거','운']
last = None
for elem in a:
  if elem == last:
    <이곳에 들어갈 코드를 작성하세요>
  print(elem, end="")
  last = elem
  
출력: 파이썬즐거운

Q7. 다음과 같은 출력이 나오도록 코드의 빈 공간을 파이썬의 lambda를 이용하여 한 줄로 작성하시오
(lambda를 사용하지 않을 시 오답으로 간주됩니다.)
a = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
b = <이곳에 들어갈 코드를 작성하세요>
c = list()
for elem in a:
  c.append(b(elem))
print(c)

출력: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

Q8. a와 b를 이용하여 아래와 같은 출력이 나오도록 코드의 A, B에 들어갈 구문으로 알맞게 짝지어진 것을 고르시오
data1 = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
data2 = [10, 11, 12, 13, 14, 15, 16, 17, 18, 19]
result = list(data1)A + data2B
print(result)

출력: [0, 1, 2, 3, 4, 5, 10, 12, 14, 16, 18]
(1) 3
(2) A: [::6], B: [:2]
(3) A: [:6], B: [::2]
(4) A: [:6], B: [:2]

Q9. a와 b를 이용하여 아래와 같은 출력이 나오도록 코드의 빈칸을 작성하시오 (set 자료형의 특성을 이용하시오)
a = [1, 2, 3, 4]
b = [3, 4, 5, 6]
c = list(set(a)._(set(b)))
print(c)

출력: [3,4]

Q10. a를 이용하여 아래와 같은 출력이 나오도록 빈칸에 들어갈 코드를 아래 보기 중 고르시오
a = [['패스트', '완주', '반'], '코딩',['캠','스','퍼'], '+', '알고리즘']
res = <이곳에 들어갈 코드를 작성하세요>
print(res)

출력: 패스트캠퍼스코딩 + 알고리즘

(1) a[0][] + a[2] + a[2][-1] + a[2][1] + a[1] + a[-2] + a[0]
(2) a[0] + a[2] + a[2][-1] + a[2][0] + a[1] + a[-2] + a[-1]
(3) a[0][0] + a[2][0] + a[2][-1] + a[2][0] + a[1] + a[-2] + a[0]
(4) a[0][0] + a[2][0] + a[2][-1] + a[2][1] + a[1] + a[-2] + a[-1]

### Report 1 (2021/03/18 ~ 2021/03/21)
과제 1.
반복문과 조건문을 이용하여, 다음과 같은 출력물이 나오도록 프로그램을 작성하시오.

<pre>
<code>
출력:
* (1)
** (2)
**** (4)
***** (5)
******* (7)
******** (8)
</code>
</pre>

과제2.
다음은 map 함수에 대한 설명이다. map 함수와 lambda 함수를 이용하여, 
10진수 숫자가 문자열로 작성된 리스트 a의 각 원소의 값을 1씩 증가시킨 문자열로 변경하는 프로그램을 한 줄의 코드로 작성하시오
- map(func, iter) 함수는 두 개의 입력을 받는다.
- 첫 번째 입력 func은 하나의 입력을 받는 함수이며, 반드시 출력이 존재한다.
- map 함수는 두 번째 입력 iter를 순회하면서 각 원소 elem을 func의 입력으로 하여, func(elem)을 출력하는 iterative object를 출력한다.
- map의 출력은 일회성으로 동작하는 iterative object이며, list() 또는 tuple()을 이용하여 여러번 참조할 수 있도록 변환할 수 있다.
<pre>
<code>
a = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
<이곳에 들어갈 한 줄의 코드를 작성하시오.>
print(a)

출력:
['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
</code>
</pre>

과제3.
다음 동작을 수행하는 프로그램을 작성하시오. (단, 입력 a의 내용이 아래 예시 입력과 달라져도 프로그램이 동작해야 한다.)
- 최대 인원 수가 정해진 방과후 수업에 학생들을 배정하려고 한다.
- 학생들은 각자 원하는 스포츠 종목을 적어냈고, 해당 종목들은 리스트 a에 저장되어 있다.
- 방과후 수업에는 최대 정원이 있어, 파이썬 프로그램을 이용해 자료를 처리하고자 한다. 
- 각 스포츠 종목별로 지원자의 수를 출력하는 프로그램을 작성하시오.
<pre>
<code>
a = ['base ball', 'basket ball', 'soccer', 'base ball', 'soccer', 'soccer', 'basket ball', 'base ball', 'basket ball', 'soccer', 'basket ball', 'basket ball', 'base ball', 'soccer', 'soccer', 'basket ball', 'basket ball', 'base ball', 'base ball']

출력:
bakset ball 7
base ball 6
soccer 6
</code>
</pre>

과제4.
반복문과 print()함수를 이용하여 아래와 같은 출력을 하는 프로그램을 구현하시오
<pre>
<code>
출력:
0 1 2 4 8 16 32 64 128 256 256 256
</code>
</pre>


### Quiz 2 (2021/03/25 ~ 2021/03/28)
Q1. 다음 코드의 실행 결과를 고르시오
<pre>
<code>
class Foo:
  def __init__(self, name):
    self.name = name
    
  def speak(self):
    print('I am' + self.name)
    
class Bar(Foo):
  def __init__(self, name):
    super().__init__(name)
    
  def speak(self):
    print('You are ' + self.name)
    
bar = Bar('John')
bar.speak()
</code>
</pre>
a. I am John
b. I am JohnYou are John
c. You are John - 이거
d. You are Jonhl am John

Q2. 다음 중 에러의 종류와 발생 원인을 맞게 나열한 것은?
a. AttributeError - 모듈, 클래스에 잘못된 속성에 접근했을 때 - 이거
b. ValueError - 주어진 테스트 출력과 값이 맞지 않을 때
c. FileNotFoundError - 요청한 파일이 없어, 새로운 파일을 만들어냈을 때 
d. TypeError - 함수에 자료형 힌트와 맞지 않은 것을 입력으로 사용했을 때

Q3. 다음 중 SQLite에 대한 설명 중 옳지 않은 것을 고르시오.
a. SQLite는 최신버전 파이썬에 기본 패키지 sqlite3로 포함되어 있다. 
b. 파이썬에서 존재하지 않는 데이터베이스에 연결하려 하면, 자동으로 새 데이터베이스를 생성한다. 
c. 파이썬 프로그램 내에서 데이터베이스와 테이블을 생성하여 사용할 수 있다. 
d. 새로운 항목을 입력하려 할 때, 기존의 항목과 Primary Key 값이 동일하면 자동으로 값을 변경하여 입력한다. - 이거

Q4. 다음 중 객체지향 프로그래밍의 지향점과 다른 것을 고르시오.
a. 클래스로 구현하여 재사용성이 높은 코드를 작성하였다.
b. 객체에 드러낼 부분과 드러내지 않을 부분을 구분하여 캡슐화를 하였다.
c. 비즈니스 로직에 집중하여 불필요한 코드 작성을 줄이고, 기능 구현에 충실하였다. - 이거
d. 기본이 되는 클래스를 상속하여, 필요한 추가 기능만을 구현하였다.

Q5. 다음 중 클래스 변수와 인스턴스 변수의 차이를 옳게 서술한 것을 고르시오.
a. 클래스 변수는 인스턴스를 생성하지 않아도 접근할 수 있다. -> 이거
b. 인스턴스 변수는 클래스 변수와 같은 이름을 가질 수 없다. -> 가질 수 있음
c. 클래스 변수와 인스턴스 변수는 생성 방법은 다르지만, 접근하는 방법은 동일하다. -> 접근 방법 다르다
d. 인스턴스 변수는 인스턴스를 생성한 후에 값을 변경할 수 없다. -> 변경할 수 있는데 권장되진 않음

Q6. 다음 함수에 대한 분석으로 옳은 것을 고르시오.
<pre>
<code>
def int_sum(*args):
  try:
    for n in args:
      sum += n
  except:
    print('error')
  return sum
</code>
</pre>
a. 예외처리문이 모든 예외를 처리하도록 되어 있으므로, 해당 함수는 절대 런타임 오류를 발생시키지 않는다.
b. 입력이 하나만 들어온 경우, for문이 정상 동작하지 않아 error를 출력한다.
c. 입력이 모두 문자열로 들어온 경우, 정수가 아니기 때문에 error를 출력한다.
d. 어떠한 입력이 들어와도 무조건 런타임 오류가 발생한다.

Q7. 다음 폴더 구조를 가진 작업 공간에서 main.py를 실행할 때, foo.py 파일 내에 있는 Foo 클래스를 import하는 구문을 작성하시오.
<pre>
<code>
ㅡㅡ main.py
  ㄴㅡ pkg ㅡㅡ __init__.py
           ㄴㅡ foo.py
</code>
</pre>

Q8. 아래 빈칸에 현재 날짜와 시간을 표시하는 구문을 작성하시오
<pre>
<code>
import datetime
now = <이곳에 들어갈 코드를 작성하세요>
print(now) // 결과예시: 2020-07-14 21:24:24.968242
</code>
</pre>


Q9. 클래스의 __init__ 메소드를 이용하여 생성된 객체를 무엇이라고 하는가?

Q10. 파이썬에서는 변수에 객체의 내용을 직접 저장하지 않고, 대신에 객체의 '이것'을 저장한다.
     '이것'을 사용하기 때문에 객체가 예상치 못하게 값이 변화할 수 있어, 깊은 복사를 적절히 사용해야 한다.
     '이것'은 무엇인가?


### Report 2 (2021/03/25 ~ 2021/03/28)
과제 1.
다음과 같이 작성된 csv 파일을 읽고, 읽어들인 모든 값을 더해서 출력하는 파이썬 프로그램을 작성하시오.
csv 파일의 위치는 실행 위치와 동일하다고 가정한다(a.csv).
(단, csv 파일의 내용은 달라질 수 있으며, 자료의 개수는 10000개 이하이다.)
<pre>
<code>
--------------- a.csv --------------------
10,60,20,33,55,25,64,83,523,54,87,84,56,84
------------------------------------------
</code>
</pre>

<pre>
<code>
---------- 출력 ------------
1238
----------------------------
</code>
</pre>

과제2.
아래 기반 코드를 완성하여, 입력받은 값 중 중앙값을 출력하는 클래스를 완성하시오.
입력받은 값이 짝수개이면, 중앙값 2개의 평균을 출력하시오
(단, clear 메소드는 입력받은 내역을 모두 삭제)
<pre>
<code>
class Median:
    def __init__(self):
        pass
 
    def get_item(self, item):
        pass
 
    def clear(self):
        pass
 
    def show_result(self):
        pass
 
median= Median()
for x in range(10):
    median.get_item(x)
median.show_result()
 
median.clear()
for x in [0.5, 6.2, -0.4, 9.6, 0.4]:
    median.get_item(x)
median.show_result()
</code>
</pre>

<pre>
<code>
--------- 출력 -------------------
4.5
0.5
------------------------------------
</code>
</pre>

과제3.
아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오.
단, Animal 클래스는 수정하지 않고 구현하시오.
최소한의 메소드만을 추가하여 구현하시오.
하나의 메소드는 하나의 line만을 출력하시오.

<pre>
<code>
class Animal:
    def __init__(self, name):
        self.name = name
 
    def speak(self):
        print(self.name + ' cannot speak.')
 
    def move(self):
        print(self.name + ' cannot move.')
 
 
class Dog(Animal):
    pass
 
 
class Retriever(Dog):
    pass
 
 
dog = Dog('Nancy')
dog.speak()
dog.move()
 
super_dog = Retriever('Michael')
super_dog.speak()
super_dog.move()
</code>
</pre>

<pre>
<code>
---------- 출력 -----------------
Nancy cannot speak.
Nancy moves like a jagger.
Michael is smart enough to speak.
Michael moves like a jagger.
---------------------------------
</code>
</pre>

과제4.
아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오. 단, 하나의 메소드에서는 단 하나의 line만을 출력하시오.
PEP를 준수하여 코드를 작성하시오.
<pre>
<code>
class Foo:
    pass
 
print(Foo.bar)       # A 출력
print(Foo().bar)     # B 출력
print(Foo.Bar.bar)   # C 출력
print(Foo.Bar().bar) # D 출력
</code>
</pre>

<pre>
<code>
----- 출력 -----
A
B
C
D
----------------
</code>
</pre>
