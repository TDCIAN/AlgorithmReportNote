# AlgorithmReportNote
Algorithm Report Note

### Quiz 1 (2021/03/18 ~ 2021/03/21)
Q1. 다음 중 여러개의 데이터를 나열하는 데에 쓰이며, 한 번 정의된 후 데이터를 변경할 수 없는 자료형을 고르시오.
1. 리스트
2. 튜플 
3. 숫자형
4. 람다

Q2. 다음 중 딕셔너리 자료형에 대한 설명으로 옳지 않은 것을 고르시오.
1. Key와 Value의 쌍으로 이루어지는 자료형이다.
2. 딕셔너리에는 여러 개의 자료를 삽입할 수 있다.
3. 딕셔너리에서는 동일한 Value를 가진 자료가 존재할 수 없다. 
4. 딕셔너리 자료형은 Key를 이용해 매우 빠르게 자료를 검색할 수 있다.

Q3. 메모리에 할당되지 않고, 즉시 실행하는 형식의 함수는 어떤 함수인가?

Q4. 다음 중 파이썬의 가상환경을 구성하는 이유로 옳지 않은 것을 고르시오
1. 원하는 패키지만을 설치하여, 깔끔한 환경을 구성할 수 있다.
2. 가상환경 별로 미리 작성된 코드를 활용하여 빠르게 프로토타이핑 할 수 있다.
3. 프로젝트 별로 프로그램이 실제로 실행될 환경에서 개발/테스트할 수 있다.
4. 특정 버전의 패키지를 설치하여 테스트해 볼 수 있다.

Q5. 다음 중 조건문에 대한 설명으로 옳은 것을 고르시오
1. 파이썬의 조건문은 if문 계열 (if, if ~ else, if elif ~ else)이 유일하다.
2. 조건문에는 반드시 bool 타입만이 사용될 수 있다.
3. [조건문 1] and [조건문 2] 형식으로 작성된 경우, 두 조건문이 반드시 모두 실행된다.
4. 조건문 내부에서 새로운 변수를 선언하더라도 조건문 외부에서 참조하는 데에 문제가 없다.

Q6. 다음과 같은 출력이 나오도록 코드의 빈 공간을 작성하시오
```python
a = ['파','이','썬','썬','썬','썬','즐','즐','즐','거','운']
last = None
for elem in a:
  if elem == last:
    <이곳에 들어갈 코드를 작성하세요>
  print(elem, end="")
  last = elem

출력: 파이썬즐거운
```


Q7. 다음과 같은 출력이 나오도록 코드의 빈 공간을 파이썬의 lambda를 이용하여 한 줄로 작성하시오
(lambda를 사용하지 않을 시 오답으로 간주됩니다.)
```python
a = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
b = <이곳에 들어갈 코드를 작성하세요>
c = list()
for elem in a:
  c.append(b(elem))
print(c)

출력: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

Q8. a와 b를 이용하여 아래와 같은 출력이 나오도록 코드의 A, B에 들어갈 구문으로 알맞게 짝지어진 것을 고르시오
```python
data1 = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
data2 = [10, 11, 12, 13, 14, 15, 16, 17, 18, 19]
result = list(data1)A + data2B
print(result)

출력: [0, 1, 2, 3, 4, 5, 10, 12, 14, 16, 18]
```
1. 3
2. A: [::6], B: [:2]
3. A: [:6], B: [::2]
4. A: [:6], B: [:2]

Q9. a와 b를 이용하여 아래와 같은 출력이 나오도록 코드의 빈칸을 작성하시오 (set 자료형의 특성을 이용하시오)
```python
a = [1, 2, 3, 4]
b = [3, 4, 5, 6]
c = list(set(a)._(set(b)))
print(c)

출력: [3,4]
```
Q10. a를 이용하여 아래와 같은 출력이 나오도록 빈칸에 들어갈 코드를 아래 보기 중 고르시오
```python
a = [['패스트', '완주', '반'], '코딩',['캠','스','퍼'], '+', '알고리즘']
res = <이곳에 들어갈 코드를 작성하세요>
print(res)

출력: 패스트캠퍼스코딩 + 알고리즘
```
1. a[0][] + a[2] + a[2][-1] + a[2][1] + a[1] + a[-2] + a[0]
2. a[0] + a[2] + a[2][-1] + a[2][0] + a[1] + a[-2] + a[-1]
3. a[0][0] + a[2][0] + a[2][-1] + a[2][0] + a[1] + a[-2] + a[0]
4. a[0][0] + a[2][0] + a[2][-1] + a[2][1] + a[1] + a[-2] + a[-1]

### Report 1 (2021/03/18 ~ 2021/03/21)
과제 1.
반복문과 조건문을 이용하여, 다음과 같은 출력물이 나오도록 프로그램을 작성하시오.
```python
출력:
* (1)
** (2)
**** (4)
***** (5)
******* (7)
******** (8)
```

과제2.
다음은 map 함수에 대한 설명이다. map 함수와 lambda 함수를 이용하여, 
10진수 숫자가 문자열로 작성된 리스트 a의 각 원소의 값을 1씩 증가시킨 문자열로 변경하는 프로그램을 한 줄의 코드로 작성하시오
- map(func, iter) 함수는 두 개의 입력을 받는다.
- 첫 번째 입력 func은 하나의 입력을 받는 함수이며, 반드시 출력이 존재한다.
- map 함수는 두 번째 입력 iter를 순회하면서 각 원소 elem을 func의 입력으로 하여, func(elem)을 출력하는 iterative object를 출력한다.
- map의 출력은 일회성으로 동작하는 iterative object이며, list() 또는 tuple()을 이용하여 여러번 참조할 수 있도록 변환할 수 있다.
```python
a = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
<이곳에 들어갈 한 줄의 코드를 작성하시오.>
print(a)

출력:
['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
```

과제3.
다음 동작을 수행하는 프로그램을 작성하시오. (단, 입력 a의 내용이 아래 예시 입력과 달라져도 프로그램이 동작해야 한다.)
- 최대 인원 수가 정해진 방과후 수업에 학생들을 배정하려고 한다.
- 학생들은 각자 원하는 스포츠 종목을 적어냈고, 해당 종목들은 리스트 a에 저장되어 있다.
- 방과후 수업에는 최대 정원이 있어, 파이썬 프로그램을 이용해 자료를 처리하고자 한다. 
- 각 스포츠 종목별로 지원자의 수를 출력하는 프로그램을 작성하시오.
```python
a = ['base ball', 'basket ball', 'soccer', 'base ball', 'soccer', 'soccer', 'basket ball', 'base ball', 'basket ball', 'soccer', 'basket ball', 'basket ball', 'base ball', 'soccer', 'soccer', 'basket ball', 'basket ball', 'base ball', 'base ball']

출력:
bakset ball 7
base ball 6
soccer 6
```

과제4.
반복문과 print()함수를 이용하여 아래와 같은 출력을 하는 프로그램을 구현하시오
```python
출력:
0 1 2 4 8 16 32 64 128 256 256 256
```

### Quiz 2 (2021/03/25 ~ 2021/03/28)
Q1. 다음 코드의 실행 결과를 고르시오
```py
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
```
1. I am John
1. I am JohnYou are John
1. You are John - 이거
1. You are Jonhl am John

Q2. 다음 중 에러의 종류와 발생 원인을 맞게 나열한 것은?
1. AttributeError - 모듈, 클래스에 잘못된 속성에 접근했을 때 - 이거
1. ValueError - 주어진 테스트 출력과 값이 맞지 않을 때
1. FileNotFoundError - 요청한 파일이 없어, 새로운 파일을 만들어냈을 때 
1. TypeError - 함수에 자료형 힌트와 맞지 않은 것을 입력으로 사용했을 때

Q3. 다음 중 SQLite에 대한 설명 중 옳지 않은 것을 고르시오.
1. SQLite는 최신버전 파이썬에 기본 패키지 sqlite3로 포함되어 있다. 
1. 파이썬에서 존재하지 않는 데이터베이스에 연결하려 하면, 자동으로 새 데이터베이스를 생성한다. 
1. 파이썬 프로그램 내에서 데이터베이스와 테이블을 생성하여 사용할 수 있다. 
1. 새로운 항목을 입력하려 할 때, 기존의 항목과 Primary Key 값이 동일하면 자동으로 값을 변경하여 입력한다. - 이거

Q4. 다음 중 객체지향 프로그래밍의 지향점과 다른 것을 고르시오.
1. 클래스로 구현하여 재사용성이 높은 코드를 작성하였다.
1. 객체에 드러낼 부분과 드러내지 않을 부분을 구분하여 캡슐화를 하였다.
1. 비즈니스 로직에 집중하여 불필요한 코드 작성을 줄이고, 기능 구현에 충실하였다. - 이거
1. 기본이 되는 클래스를 상속하여, 필요한 추가 기능만을 구현하였다.

Q5. 다음 중 클래스 변수와 인스턴스 변수의 차이를 옳게 서술한 것을 고르시오.
1. 클래스 변수는 인스턴스를 생성하지 않아도 접근할 수 있다. -> 이거
1. 인스턴스 변수는 클래스 변수와 같은 이름을 가질 수 없다.
1. 클래스 변수와 인스턴스 변수는 생성 방법은 다르지만, 접근하는 방법은 동일하다.
1. 인스턴스 변수는 인스턴스를 생성한 후에 값을 변경할 수 없다.

Q6. 다음 함수에 대한 분석으로 옳은 것을 고르시오.

```py
def int_sum(*args):
  try:
    for n in args:
      sum += n
  except:
    print('error')
  return sum
  ```
1. 예외처리문이 모든 예외를 처리하도록 되어 있으므로, 해당 함수는 절대 런타임 오류를 발생시키지 않는다.
1. 입력이 하나만 들어온 경우, for문이 정상 동작하지 않아 error를 출력한다.
1. 입력이 모두 문자열로 들어온 경우, 정수가 아니기 때문에 error를 출력한다.
1. 어떠한 입력이 들어와도 무조건 런타임 오류가 발생한다. - 이거

Q7. 다음 폴더 구조를 가진 작업 공간에서 main.py를 실행할 때, foo.py 파일 내에 있는 Foo 클래스를 import하는 구문을 작성하시오.
<pre>
<code>
ㅡㅡ main.py
  ㄴㅡ pkg ㅡㅡ __init__.py
           ㄴㅡ foo.py
</code>
</pre>

answer: from pkg.foo import Foo


Q8. 아래 빈칸에 현재 날짜와 시간을 표시하는 구문을 작성하시오

```py
import datetime
now = <이곳에 들어갈 코드를 작성하세요>
print(now) // 결과예시: 2020-07-14 21:24:24.968242
```

answer: datetime.datetime.now()

Q9. 클래스의 __init__ 메소드를 이용하여 생성된 객체를 무엇이라고 하는가?

answer: 인스턴스

Q10. 파이썬에서는 변수에 객체의 내용을 직접 저장하지 않고, 대신에 객체의 '이것'을 저장한다.
     '이것'을 사용하기 때문에 객체가 예상치 못하게 값이 변화할 수 있어, 깊은 복사를 적절히 사용해야 한다.
     '이것'은 무엇인가?

answer: 참조, reference


### Report 2 (2021/03/25 ~ 2021/03/28)
과제 1.
다음과 같이 작성된 csv 파일을 읽고, 읽어들인 모든 값을 더해서 출력하는 파이썬 프로그램을 작성하시오.
csv 파일의 위치는 실행 위치와 동일하다고 가정한다(a.csv).
(단, csv 파일의 내용은 달라질 수 있으며, 자료의 개수는 10000개 이하이다.)

```p
--------------- a.csv --------------------
10,60,20,33,55,25,64,83,523,54,87,84,56,84
------------------------------------------
```
```
---------- 출력 ------------
1238
----------------------------
```

답안

```p
import csv
with open('./a.csv', 'r') as f:
    reader = csv.reader(f)
    sum = 0    
    for n in reader:
        for i in n:
            sum += int(i)

print(sum)

```

과제2.
아래 기반 코드를 완성하여, 입력받은 값 중 중앙값을 출력하는 클래스를 완성하시오.
입력받은 값이 짝수개이면, 중앙값 2개의 평균을 출력하시오
(단, clear 메소드는 입력받은 내역을 모두 삭제)

```py
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
```


```
--------- 출력 -------------------
4.5
0.5
------------------------------------
```

답안

```py
class Median:
    list_of_num = []

    def __init__(self):
        self.list_of_num = []
 
    def get_item(self, item):
        self.list_of_num.append(item)
 
    def clear(self):
        self.list_of_num = []
 
    def show_result(self):
        self.list_of_num.sort()
        len_of_list = len(self.list_of_num)
        center_of_list = int(len_of_list / 2)
        if len_of_list % 2 == 1:
            print(self.list_of_num[center_of_list])
        else:
            print((self.list_of_num[center_of_list - 1] + self.list_of_num[center_of_list]) / 2.0)
 
median = Median()
for x in range(10):
    median.get_item(x)
median.show_result()
 
median.clear()
for x in [0.5, 6.2, -0.4, 9.6, 0.4]:
    median.get_item(x)
median.show_result()
```

과제3.
아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오.
단, Animal 클래스는 수정하지 않고 구현하시오.
최소한의 메소드만을 추가하여 구현하시오.
하나의 메소드는 하나의 line만을 출력하시오.


```py
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
```

```
---------- 출력 -----------------
Nancy cannot speak.
Nancy moves like a jagger.
Michael is smart enough to speak.
Michael moves like a jagger.
---------------------------------
```



```py
class Animal:
    def __init__(self, name):
        self.name = name
 
    def speak(self):
        print(self.name + ' cannot speak.')
 
    def move(self):
        print(self.name + ' cannot move.')
 
 
class Dog(Animal):
    def move(self):
      print(self.name + ' moves like a jagger.')
 
class Retriever(Dog):
    def speak(self):
      print(self.name + ' is smart enough to speak.')
 
 
dog = Dog('Nancy')
dog.speak()
dog.move()
 
super_dog = Retriever('Michael')
super_dog.speak()
super_dog.move()

```

과제4.
아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오. 단, 하나의 메소드에서는 단 하나의 line만을 출력하시오.
PEP를 준수하여 코드를 작성하시오.

```py
class Foo:
    pass
 
print(Foo.bar)       # A 출력
print(Foo().bar)     # B 출력
print(Foo.Bar.bar)   # C 출력
print(Foo.Bar().bar) # D 출력
```

```
----- 출력 -----
A
B
C
D
----------------
```

답안


```py
class Foo:
  bar = 'A'
  def __init__(self):
    self.bar = 'B'
  
  class Bar:
    bar = 'C'
    def __init__(self):
      self.bar = 'D'
  
print(Foo.bar)
print(Foo().bar)
print(Foo.Bar.bar)
print(Foo.Bar().bar)
```

### Quiz 3 (2021/04/01 ~ 2021/04/04)


Q1. 다음 중 자료구조에 대한 설명으로 옳지 않은 것은?
1. 큐는 First-In, First-Out의 특성을 지니고 있어, 입력된 순서대로 처리하고자 할 때 사용된다.
2. 스택에서 pop을 수행하면 가장 마지막에 삽입된 자료를 반환하고 스택에서 삭제한다.
3. 해시 테이블은 자료에 O(1)로 접근할 수 있지만, 메모리를 과도하게 사용한다.
4. 링크드 리스트는 원하는 인덱스에 곧바로 접근할 수 있어, 배열 리스트보다 효율적이다. <- 답


Q2. 다음 프로그램의 시간 복잡도를 변수 n의 값에 대해서 Big-O Notation으로 바르게 표기한 것은?

```py
n = 100
sum = 0
for i in range(n):
  for j i range(i//2):
    sum += i**j
```
1. O(1)
2. O(n)
3. O(n^2) <- 답
4. O(n^n)


Q3. 주어진 해시 함수를 이용해 해시 테이블을 만들어 사용하고자 한다. 이 때 해시 테이블의 크기를 구하시오
(해시 충돌은 고려하지 않으며, 필요한 최소의 크기의 해시 테이블을 만든다. n은 양의 정수 입력이다)

```py
def hash_func(n):
  return abs((n % 10) - 5)
```

답: 6


Q4. 다음과 같은 출력을 얻기 위해 빈 곳을 채우시오.
```py
import queue
a = <이곳에 들어갈 코드를 작성하세요>
a.put((10, '캠퍼스'))
a.put((1, '패스트'))
a.put((55, '완주반'))
a.put((11, '온라인'))

print(''.join([a.get()[1], a.get()[1], a.get()[1], a.get()[1]]))

출력: 패스트 캠퍼스 온라인 완주반
```

답: queue.PriorityQueue()


Q5. 다음 중 링크드 리스트(linked list)의 특징으로 옳지 않은 것은?
1. 링크드 리스트의 길이는 동적으로 조절이 가능하다.
2. N개 노드에 대한 링크드 리스트의 탐색 시간복잡도는 O(1)이다. -> 답
3. 역순으로 노드 탐색이 필요한 경우 double linked list가 유용하다.
4. 데이터의 삽입/삭제를 효율적으로 할 수 있다.


Q6. 파이썬의 배열(리스트)과 자료구조로서의 배열은 그 의미가 다르다. 다음 중 배열 자료구조에 대한 설명으로 옳지 않은 것을 고르시오.
1. 배열은 크기가 정해져 있어, 크기를 증가시키려면 반드시 새 배열을 만들어야 한다.
2. 배열에는 다양한 자료형을 삽입할 수 있다. -> 답
3. 배열의 각 요소는 메모리에 연속적으로 위치한다.
4. 배열은 요소를 삭제할 때마다, 모든 요소를 앞으로 당겨 주어야 한다.


Q7. 해시 테이블에서 해시 충돌이 발생할 경우, 이를 해결하는 방법 중에 테이블의 비어있는 다음 인덱스에 자료를 삽입하는 기법을 무엇이라고 하는지 쓰시오.

답: 선형조사법(Linear Probing, 리니어 프루빙)

Q8. 알고리즘이 동작할 때 필요한 메모리의 정도를 무엇이라고 하는가?

답: 공간복잡도


Q9. 스택의 자료 입출력 순서에 대한 특성을 무엇이라고 부르는가?

답: LIFO, Last-In, First-Out , 후입선출

Q10. 해시 테이블 자료구조에서 다른 키 값이지만 동일한 해시 값을 가질 때 발생하는 문제를 무엇이라고 하는가?

답: 해시 충돌


### Report 3 (2021/04/01 ~ 2021/04/03)

과제 1.
아래 주어진 기반 코드를 완성하여 Linked Queue를 구현하시오. Linked Queue에 대한 설명을 참조하시오


- Linked Queue의 특징
  - Linked Queue는 Doubly Linked List를 기반으로 만들어진 Queue이다.
  - Linked Queue의 모든 동작은 O(1)의 시간복잡도로 동작한다.
  - Linked Queue에 정의된 동작은 아래와 같다.
    1. is_empty(): Queue가 비어있으면 True, 비어있지 않으면 False를 출력한다.
    2. put(): Queue의 rear에 새로운 데이터를 입력한다.
    3. get(): Qeueue의 front에서 데이터를 출력한다. 출력한 데이터는 Queue에서 삭제한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.
    4. peek(): Queue의 front에서 데이터를 출력한다. 출력한 데이터는 Queue에 그대로 유지한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.

```py
class Node:
  def __init__(self, data, prev=None, next=None):
    self.data =data
    self.prev = prev
    self.next = next
    
class LinkedQueue:
  def __init__(self):
    self.front = None
    self.rear = None
    
  def is_empty(self):
    pass
    
  def put(self, data):
    pass
    
  def get(self):
    pass
    
  def peek(self):
    pass
    
# Test code
queue = LinkedQueue()

print(queue.is_empty())
for i in range(10):
  queue.put(i)
print(queue.is_empty())

for _ in range(11):
  print(queue.get(), end = ' ')
print()

for i in range(20):
  queue.put(i)
print(queue.is_empty())

for _ in range(5):
  print(queue.peek(), end = ' ')
  
for _ in range(21):
  print(queue.get(), end = ' ')
print()
print(queue.is_empty())

```


### 강사님 예시답안

```py
class Node:
    def __init__(self, data, prev=None, next=None):
        self.data = data
        self.prev = prev
        self.next = next
 
class LinkedQueue:
    def __init__(self):
        self.front = None
        self.rear = None
 
    def is_empty(self):
        if self.front is None:
            return True
        else:
            return False
 
    def put(self, data):
        if self.rear is None:
            self.front = Node(data)
            self.rear = self.front
        else:
            self.rear = Node(data, self.rear, None)
            self.rear.prev.next = self.rear
 
    def get(self):
        if self.front is None:
            return None
        elif self.front is self.rear:
            data = self.front.data
            self.front, self.rear = None, None
        else:
            data = self.front.data
            self.front = self.front.next
            self.front.prev = None
        return data
 
    def peek(self):
        if self.front is None:
            return None
        else:
            return self.front.data
```

과제 2.
아래는 Python의 list를 이용하여 Stack을 구현한 것이다. Stack의 특성을 이용하면 후위 표기법으로 작성된 수식을 계산할 수 있다.
후위 표기법은 연산자를 나중에 표기하는 표기법으로, 아래와 같이 계산한다. 후위 표기법에서 사칙연산의 우선순위는 없다고 가정한다.

```py
10 5 + 2 * 3 /
= 15 2 * 3 /
= 30 3 /
= 10
```

연산자와 피연산자가 공백으로 구분된다고 할 때, 내부적으로 stack을 유일한 자료구조로 사용하여 
후위 표기법으로 표기된 수식을 계산하는 메소드 calculate()을 완성하시오.

```py
class Stack:
  def __init__(self):
    self.list = list()
    
  def push(self, data):
    self.list.append(data)
    
  def pop(self):
    return self.list.pop()
    
class Calculator:
  def __init__(self):
    self.stack = Stack()
    
  def calculate(self, string):
    pass
    
# Test code
calc = Calculator()
print(calc.calculate('4 6 * 2 / 2 +'))
print(calc.calculate('2 5 + 3 * 6 - 5 *'))

```


### 강사님 예시답안

```py
class Stack:
    def __init__(self):
        self.list = list()
 
    def push(self, data):
        self.list.append(data)
 
    def pop(self):
        return self.list.pop()
 
class Calculator:
    def __init__(self):
        self.stack = Stack()
 
    def calculate(self, string):
        for x in string.split(' '):
            if x == '+':
                self.stack.push(self.stack.pop() + self.stack.pop())
            elif x == '-':
                self.stack.push(- self.stack.pop() + self.stack.pop())
            elif x == '*':
                self.stack.push(self.stack.pop() * self.stack.pop())
            elif x == '/':
                self.stack.push(1 / self.stack.pop() * self.stack.pop())
            else:
                self.stack.push(int(x))
        return self.stack.pop()
 
calc = Calculator()
print(calc.calculate('4 6 * 2 / 2 +'))
print(calc.calculate('2 5 + 3 * 6 - 5 *'))
```

과제 3.
다음은 Tree 자료구조를 순회하는 방법 중, Pre-order 순회 방법을 설명한 것이다. 자료구조의 순회란, 자료구조에 속한 모든 data를 한 번씩 접근하는 것이다.
Pre-order 순회를 하면서 순회한 순서대로 Node의 data를 출력하는 preorder() 메소드를 완성하시오.
- Tree 자료구조를 선회할 때에는 반드시 root node부터 순회를 시작한다.
- Pre-order 순회를 할 때에는 아래와 같은 방법을 재귀적으로 수행한다.
  - 새로운 node에 접근할 경우, 아래 순서대로 동작한다.
    1. Node에 있는 data를 출력한다.
    2. Node에 left child가 있으면, left child node에 접근한다.
    3. Node에 right child가 있으면, right child node에 접근한다.
  - root node에서 순회를 시작할 경우, 재귀적 동작으로 인해 모든 node의 data를 출력할 수 있다.


```py
class Node:
  def __init__(self, data, left=None, right=None):
    self.data = data
    self.left = left
    self.right = right
    
class Tree:
  def __init__(self, root):
    self.root = root
    
  def preorder(self):
    pass
    
# Test code
root = Node(5, Node(2, Node(7, Node(4), Node(1)), Node(3)), Node(9, Node(6), Node(10)))
tree = Tree(root)
tree.preorder()
```


### 강사님 예시답안

```py
class Node:
    def __init__(self, data, left=None, right=None):
        self.data = data
        self.left = left
        self.right = right
 
class Tree:
    def __init__(self, root):
        self.root = root
 
    def preorder(self):
        def recursion(node):
            print(node.data, end=' ')
            if node.left:
                recursion(node.left)
            if node.right:
                recursion(node.right)
        recursion(self.root)
 
 
# Test code
root = Node(5, Node(2, Node(7, Node(4), Node(1)), Node(3)), Node(9, Node(6), Node(10)))
tree = Tree(root)
tree.preorder()
```

과제 4.
HashTable 클래스는 문자열을 key로 입력받는 해쉬 테이블 자료구조를 구현한 것이다.
HashTable 클래스는 단순한 해쉬 함수로 인해, 해쉬 충돌이 빈번히 발생한다.
이 단점을 개선하기 위해, Chaining 기법으로 ChainedHashTable을 구현하고자 한다.

HashTable을 상속하여 해쉬 충돌이 발생해도 정상적으로 동작하는 ChainedHashTable을 완성하시오.

```py
def hash_func(key):
  return ord(key[0]) % 10
  
class HashTable:
  def __init__(self):
    self.table = [None] * 10
    
  def self(self, key, value):
    self.table[hash_func(key)] = value
    
  def get(self, key):
    return self.table[hash_func(key)]
    
class Node:
  def __init__(self, key, data):
    self.key = key
    self.data = data 
    self.next = None
    
class ChainedHashTable(HashTable):
  pass
  
# Test code

ht = ChainedHashTable()
ht.set('hello', 1)
ht.set('hello2', 2)
ht.set('hello3', 3)
ht.set('hello4', 4)

print(ht.get('hello'), end=' ')
print(ht.get('hello2'), end=' ')
print(ht.get('hello3'), end=' ')
print(ht.get('hello4'), end=' ')
print()

ht.set('hello2', 5)

print(ht.get('hello'), end=' ')
print(ht.get('hello2'), end=' ')
print(ht.get('hello3'), end=' ')
print(ht.get('hello4'), end=' ')
```


### 강사님 예시답안

```py
def hash_func(key):
    return ord(key[0]) % 10
 
class HashTable:
    def __init__(self):
        self.table = [None]*10
 
    def set(self, key, value):
        self.table[hash_func(key)] = value
 
    def get(self, key):
        return self.table[hash_func(key)]
 
class Node:
    def __init__(self, key, data):
        self.key = key
        self.data = data
        self.next = None
 
class ChainedHashTable(HashTable):
    def __init__(self):
        super().__init__()
 
    def set(self, key, value):
        idx = self.hash_func(key)
        if self.table[idx] is None:
            self.table[idx] = Node(key, value)
        else:
            node = self.table[idx]
            while node.next is not None:
                if node.key == key:
                    node.data = value
                    return
                node = node.next
            node.next = Node(key, value)
 
    def get(self, key):
        idx = self.hash_func(key)
        if self.table[idx] is None:
            return None
        else:
            node = self.table[idx]            
            while node.next is not None:
                if node.key == key:
                    return node.data
                node = node.next
            if node.key == key:
                return node.data
            else:
                return None
 
ht = ChainedHashTable()
ht.set('hello', 1)
ht.set('hello2', 2)
ht.set('hello3', 3)
ht.set('hello4', 4)
 
print(ht.get('hello'), end=' ')
print(ht.get('hello2'), end=' ')
print(ht.get('hello3'), end=' ')
print(ht.get('hello4'), end=' ')
print()
 
ht.set('hello2', 5)
 
print(ht.get('hello'), end=' ')
print(ht.get('hello2'), end=' ')
print(ht.get('hello3'), end=' ')
print(ht.get('hello4'), end=' ')

```

### Quiz 4 (2021/04/08 ~ 2021/04/11)

Q1. 다음 중 자료구조 힙(Heap)에 대한 설명으로 옳지 않은 것은?
1. 데이터의 최대값 또는 최소값을 빠르게 찾을 수 있다.
2. 최대값을 찾을 때 배열을 사용할 경우 시간복잡도가 O(N)이나, 힙(heap)을 이용하게 되면 O(NlogN)의 시간복잡도를 갖는다 -> 이거, logN이니까
3. 완전 이진 트리의 일종으로 최대힙(max heap)과 최소힙(min heap)이 있다.
4. 힙과 이진탐색트리는 새로운 node를 삽입할 때의 조건이 다르다.


Q2. 다음과 같이 Max Heap 구조의 그래프가 있을 때 새로운 node를 삽입하려고 한다. 이 때 어떤 node에 삽입이 될지 아래 보기 중 고르시오(새로운 node의 데이터는 10이다)
1. node#2
2. node#3
3. node#4
4. node#5
5. node#6 -> 이거


Q3. 공간 복잡도(Space Complexity)에서 알고리즘 실행과 관련있는 공간으로, 알고리즘 실행 중 동적으로 필요한 공간을 무엇이라고 하는가?

답: 가변 공간


Q4. 가장 단순한 정렬 방법 중 하나로, 정렬이 끝날때까지 연속된 2개의 자료를 비교하는 정렬 알고리즘을 무엇이라 하는가?

답: 버블정렬


Q5. 다음 중 이진 탐색 트리의 특징으로 옳은 것을 고르시오.
1. 이진 탐색 트리는 자료를 입력하는 순서에 관계 없이 항상 최적의 구조를 가지게 된다.
2. 이진 탐색 트리는 이진 트리 중 하나로, 항상 완전 이진 트리(Complete Binary Tree)의 구조를 가진다.
3. 최적의 구조를 갖춘 이진 탐색 트리의 탐색은 O(logN)의 시간복잡도를 가진다. -> 이거 
4. 이진 탐색 트리는 자료를 입력할 때에는 복잡한 연산을 필요로 하지만, 자료를 삭제할 때에는 해당 노드만 삭제하면 된다.

 * 해설: 퀵정렬의 시간복잡도는 일반적으로 O(NlogN)이며, 최악의 경우 pivot으로 가장 크거나 작은 수를 선택하는 경우 O(N^2)의 시간복잡도를 가진다.


Q6. 해쉬 테이블에 대한 설명으로 옳지 않은 것을 고르시오.
1. 해쉬 테이블은 해쉬 함수를 이용하여 빠르게 자료를 저장할 수 있는 자료구조이다.
2. 해쉬 테이블은 해쉬 충돌이 없다고 가정했을 때, 자료의 입력과 검색이 O(1)의 시간복잡도로 이루어진다.
3. 해쉬 함수는 해쉬 테이블의 성능을 결정하는 중요한 함수이므로, 신중하게 선택해야 한다.
4. 해쉬 테이블에서 해쉬 충돌이 발생하면 기입력된 자료가 손실되기 때문에, 해쉬 충돌이 절대 일어나지 않는 해쉬 함수를 선택해야 한다.


Q7. 주어진 데이터 중 최소값을 찾아, 맨 앞의 데이터와 위치를 바꾸는 과정을 반복하는 정렬 방법을 무엇이라 하는가?


답: 선택정렬


Q8. 파이썬의 list slicing 기법을 사용하여 아래와 같이 출력을 얻었다고 할 때, 아래 빈칸에 들어갈 숫자를 각각 적으시오(이때 a는 양수, b는 음수이다)

```py
mystr = 'FastCampus'

a = __ # 양수
b = __ # 음수

res = mystr[a:b]
print(res)

출력: tCampu

```

답: a = 3, b = -1


Q9. 다음 중 삽입 정렬의 시간 복잡도와 공간 복잡도를 맞게 나열한 것은? (단, 삽입 정렬의 in-place 연산을 기준으로 한다. 즉, 출력을 위한 메모리를 새로 할당하지 않는다)
1. 시간복잡도: O(NlogN), 공간복잡도: O(N)
2. 시간복잡도: O(N^3), 공간복잡도: O(1)
3. 시간복잡도: O(N^2), 공간복잡도: O(NlogN)
4. 시간복잡도: O(N^2), 공간복잡도: O(1) -> 이거


Q10. 다음 중 시간복잡도가 다른 알고리즘을 고르시오.
1. 링크드 리스트에서 첫번째 위치에 자료를 삽입하는 알고리즘 -> O(1)
2. 해쉬 테이블에서 자료를 입력하는 알고리즘 -> O(1)
3. 힙에 자료를 하나 추가하는 알고리즘 -> O(nlogn) -> 이거
4. 정렬된 배열에서 가장 작은 값을 반환하는 알고리즘 -> O(1)




### Report 4 (2021/04/08 ~ 2021/04/11)


과제1.
<br> Min Heap 자료구조를 이용하면 최대값을 O(logN)의 시간복잡도로 찾을 수 있다. Min Heap을 이용하면 우선순이 값이 낮은 자료를 먼저 출력하는 Priority Queue를 구현할 수 있다.
<br> Min Heap을 이용한 Priority Queue는 아래와 같은 특징을 가진다.
- Min Heap을 이용한 Priority Queue의 특징
  - 자료를 입력하는 동작과 출력하는 동작 모두 O(logN)으로 일어진다.
  - 우선순위 값이 낮은 자료를 먼저 출력하되, 우선순위 값이 같은 자료끼리는 순서를 고려하지 않는다.
  - 다음과 같은 Method들을 구현한다.
    1. is_empty(): Queue가 비어있으면 True, 비어있지 않으면 False를 출력한다.
    2. put(): Priority Queue에 자료를 입력한다. 자료는 길이가 2인 Tuple로, (우선순위, 자료) 형태로 입력받는다.
    3. get(): Priority Queue에서 자료를 출력한다. 출력한 데이터는 Priority Queue에서 삭제한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.
    4. peek(): Priority Queue에서 자료를 출력한다. 출력한 데이터는 Priority Queue에 그대로 유지한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.


```py
class PriorityQueue:
  def __init__(self):
    pass
    
  def is_empty(self):
    pass
    
  def put(self, data):
    pass
    
  def get(self):
    pass
    
  def peek(self):
    pass
    
# Test code
pq = PriorityQueue()
pq.put((0, 'a'))
pq.put((5, 'b'))
pq.put((2, 'c'))
pq.put((1, 'd'))
pq.put((3, 'e'))
pq.put((4, 'f'))

print(pq.get())
print(pq.get())
print(pq.get())
print(pq.get())
print(pq.get())
print(pq.get())
print(pq.get())

```

과제2.
<br> 오름차순으로 정렬된 N개의 정수를 가진 List가 주어져있을 때, 해당 List에 존재하는 서로 다른 값이 몇 가지인지 알아내는 알고리즘을 구현하라.
<br> 알고리즘의 제약사항은 아래와 같다. (알고리즘은 1 <= N <= 10000에서 테스트된다)
    - 추가 메모리 사용은 O(1)으로 제한된다. 따라서 set()와 dict() 등의 자료구조를 사용할 수 없다.
    - 알고리즘의 시간복잡도는 O(N) 이하로 제한된다.

```py
def countUniques(a):
  pass

# Test code
print(countUniques([-1, 1, 1, 1, 1, 4, 4, 4, 4, 10, 14, 14])) # 5
print(countUniques([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])) # 2

```

과제3
<br> N개의 문자열로 이루어진 List에서 전체 문자열이 앞 n개 문자열이 같다고 할 때, 가장 큰 n을 출력하는 알고리즘을 구현하라.
<br> (즉, 주어진 모든 문자열의 앞의 몇개의 문자가 일치하는지 출력하라)

```py
def solution(a):
  return 0

# Test code
print(solution(['abcd', 'abce', 'abchg', 'abcfwqw', 'abcdfg'])) # 3
print(solution(['abcd', 'gbce', 'abchg', 'abcfwqw', 'abcdfg'])) # 0

```

과제4.
<br> 자연수 중, 각 자리수를 제곱한 것을 더하는 과정을 반복했을 때 1로 끝나는 수를 '행복한 수'라고 한다.
<br> '행복한 수'가 아닌 경우 이 과정이 1에 도달하지 못하고 같은 수열이 반복되는 무한 루프에 빠지게 된다.
<br> 자연수를 입력받았을 때 '행복한 수'인지 판별하는 알고리즘을 작성하라.

'행복한 수'를 찾는 과정의 예

19이 행복한 수인지 확인하는 과정
1^2 + 9^2 = 82
8^2 + 2^2 = 68
6^2 + 8^2 = 100
1^2 + 0^2 + 0^2 = 1 --> True


```py
def solution(n):
  return True

# Test code
print(solution(19)) # True
print(solution(61)) # False

```
