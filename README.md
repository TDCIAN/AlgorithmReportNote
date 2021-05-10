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
## 과제1.

----
반복문과 조건문을 이용하여, 다음과 같은 출력이 나오도록 프로그램을 작성하시오.

출력:
```
*
**
****
*****
*******
********
```
----

### 과제1 답안(25/25)

- for문과 if문을 이용하여 구현하는 문제였습니다.
- 잘 구현해 주셨습니다! :)

예시 답안)

```python
for i in range(9):
    if i % 3 != 0:
        print('*'*i)
```

## 과제2.

----

다음은 map함수에 대한 설명이다. map 함수와 lambda 함수를 이용하여, 10진수 숫자가 문자열로 작성된 리스트 a의 각 원소의 값을 1씩 증가시킨 문자열로 변경하는 프로그램을 한 줄의 코드로 작성하시오.

- map(func, iter) 함수는 두 개의 입력을 받는다. 
- 첫 번째 입력 func은 하나의 입력을 받는 함수이며, 반드시 출력이 존재한다. 
- map 함수는 두 번째 입력 iter를 순회하면서 각 원소 elem을 func의 입력으로 하여, func(elem)을 출력하는 iterative object를 출력한다. 
- map의 출력은 일회성으로 동작하는 iterative object이며, list() 또는 tuple()을 이용하여 여러번 참조할 수 있도록 변환할 수 있다.

```python
a = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
<이곳에 들어갈 한 줄의 코드를 작성하시오.>
print(a)
```

출력:
```python
['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
```
----

### 과제2 답안(25/25)

- map함수를 이해하고 활용해 보는 문제였습니다.
- 잘 구현해 주셨습니다! :)


예시 답안)


예시 답안)

```python
a = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
a = list(map(lambda x: str(int(x) + 1), a))
print(a)
```



## 과제3.

----
다음 동작 수행하는 프로그램을 작성하시오. (단, 입력 a의 내용이 아래 예시 입력과 달라져도 프로그램이 동작해야 한다.)

- 최대 인원 수가 정해진 방과후 수업에 학생들을 배정하려고 한다. 
- 학생들은 각자 원하는 스포츠 종목을 적어냈고, 해당 종목들은 리스트 a에 저장되어 있다. 
- 방과후 수업에는 최대 정원이 있어, 파이썬 프로그램을 이용해 자료를 처리하고자 한다. 각 스포츠 종목별로 지원자의 수를 출력하는 프로그램을 작성하시오.


```python
a = ['base ball', 'basket ball', 'soccer', 'base ball', 'soccer', 'soccer', 'basket ball', 'base ball', 'basket ball', 'soccer', 'basket ball', 'basket ball', 'base ball', 'soccer', 'soccer', 'basket ball', 'basket ball', 'base ball', 'base ball']

```

출력:
```python
basket ball 7
base ball 6
soccer 6

```

### 과제3 답안(25/25)

- 리스트를 해석하고 종합하는 문제였습니다.
- 잘 구현해 주셨습니다! :)


예시 답안)


```python
a = ['base ball', 'basket ball', 'soccer', 'base ball', 'soccer', 'soccer', 'basket ball', 'base ball', 'basket ball', 'soccer', 'basket ball', 'basket ball', 'base ball', 'soccer', 'soccer', 'basket ball', 'basket ball', 'base ball', 'base ball']
for sport in set(a):
    print(sport, a.count(sport))
```


## 과제4.

----
반복문과 print() 함수를 이용하여 아래와 같은 출력을 하는 프로그램을 구현하시오.

출력:
```python
0 1 2 4 8 16 32 64 128 256 256 256
```

----

### 과제4 답안(25/25)

- 반복문과 조건문 등을 조합하여 원하는 숫자를 출력하는 문제였습니다.
- 잘 구현해 주셨습니다! :) 아래 하나의 예시를 드리니 참고해 주세요 :)

예시 답안)

```python
x = 0
for _ in range(12):
    print(x, end=' ')
    if x == 0:
        x += 1
    elif x < 256:
        x *= 2
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

## 과제1.

----

다음과 같이 작성된 csv 파일을 읽고, 읽어들인 모든 값을 더해서 출력하는 파이썬 프로그램을 작성하시오. csv파일의 위치는 실행 위치와 동일하다고 가정한다(`a.csv`). (단, csv 파일의 내용은 달라질 수 있으며, 자료의 개수는 10000개 이하이다.)

```
--------------- a.csv --------------------
10,60,20,33,55,25,64,83,523,54,87,84,56,84
------------------------------------------
```

```
---------- 출력 ------------
1238
----------------------------
```

----

### 과제1 답안(25/25)

- 파일 입력을 이용해 csv파일 파싱을 잘 구현해 주셨습니다 :)
- 정수형 입력을 종합하여 총합을 잘 계산하여 출력해 주셨습니다.

예시 답안)

```python
import csv

sum = 0
with open('a.csv', 'r') as f:
    reader = csv.reader(f)
    for line in reader:
        for elem in line:
            sum += int(elem)
print(sum)
```


## 과제2.

----

아래 기반 코드를 완성하여, 입력받은 값 중 중앙값을 출력하는 클래스를 완성하시오. 입력받은 값이 짝수개이면, 중앙값 2개의 평균을 출력하시오. (단, clear 메소드는 입력받은 내역을 모두 삭제)

```python
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

----

### 과제2 답안(25/25)

- 객체지향적으로 중간값을 구하는 문제였습니다.
- 클래스의 기능을 충실하게 잘 구현해 주셨습니다!

```python
class Median:
    def __init__(self):
        self.list = list()

    def get_item(self, item):
        self.list.append(item)

    def clear(self):
        self.list = list()

    def show_result(self):
        self.list.sort()
        n = len(self.list)
        if n % 2 == 1:
            med = self.list[n // 2]
        else:
            med = (self.list[n // 2 - 1] + self.list[n // 2]) / 2
        print(med)

median= Median()
for x in range(10):
    median.get_item(x)
median.show_result()

median.clear()
for x in [0.5, 6.2, -0.4, 9.6, 0.4]:
    median.get_item(x)
median.show_result()
```


## 과제3.

----

아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오. 단, Animal 클래스는 수정하지 않고 구현하시오. 최소한의 메소드만을 추가하여 구현하시오. 하나의 메소드는 하나의 line만을 출력하시오.

```python
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

----

### 과제3 답안(25/25)

- 클래스의 상속을 이해하고, 이를 직접 구현하는 문제였습니다.
- 상속과 오버라이딩을 잘 이해하고 구현해 주셨습니다 :)

```python
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

## 과제4.

----

아래 기반 코드를 완성하여, 주어진 출력을 하는 클래스를 구현하시오. 단, 하나의 메소드에서는 단 하나의 line만을 출력하시오. PEP를 준수하여 코드를 작성하시오.

```python
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

----

### 과제4 답안(25/25)

- 클래스 변수와 인스턴스 변수를 이해하고 구현하는 문제였습니다.
- 중첩 클래스까지 활용하면 주어진 과제를 모두 해결하실 수 있습니다. :)

```python
class Foo:
    bar = 'A'
    def __init__(self):
        self.bar = 'B'
    
    class Bar:
        bar = 'C'
        def __init__(self):
            self.bar = 'D'

print(Foo.bar)       # A 출력
print(Foo().bar)     # B 출력
print(Foo.Bar.bar)   # C 출력
print(Foo.Bar().bar) # D 출력
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

## 과제1.

----
아래 주어진 기반 코드를 완성하여 Linked Queue를 구현하시오. Linked Queue에 대한 설명을 참조하시오.

- Linked Queue의 특징
  - Linked Queue는 Doubly Linked List를 기반으로 만들어진 Queue이다.
  - Linked Queue의 모든 동작은 O(1)의 시간복잡도로 동작한다.
  - Linked Queue에 정의된 동작은 아래와 같다.
    1. `is_empty()`: Queue가 비어있으면 True, 비어있지 않으면 False를 출력한다.
    1. `put()`: Queue의 rear에 새로운 데이터를 입력한다.
    1. `get()`: Queue의 front에서 데이터를 출력한다. 출력한 데이터는 Queue에서 삭제한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.
    1. `peek()`: Queue의 front에서 데이터를 출력한다. 출력한 데이터는 Queue에 그대로 유지한다.  더이상 출력할 데이터가 없는 경우 None을 출력한다.


```python
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
    print(queue.get(), end=' ')
print()

for i in range(20):
    queue.put(i)
print(queue.is_empty())

for _ in range(5):
    print(queue.peek(), end=' ')
print()

for _ in range(21):
    print(queue.get(), end=' ')
print()
print(queue.is_empty())

```
----


### 과제1 답안(25/25)

- 수업시간에 배운 Doubly Linked List를 이용하여 Linked Queue를 구현하는 문제였습니다.
- 기능을 잘 구현해 주셨습니다! 아래 예시답안을 첨부하니 참고해 주세요 :)

예시 답안)

```python
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



## 과제2.

----
아래는 Python의 list를 이용하여 Stack을 구현한 것이다. Stack의 특성을 이용하면 후위 표기법으로 작성된 수식을 계산할 수 있다. 후위 표기법은 연산자를 나중에 표기하는 표기법으로, 아래와 같이 계산한다. 후위 표기법에서 사칙연산의 우선순위는 없다고 가정한다.

```
10 5 + 2 * 3 /
= 15 2 * 3 /
= 30 3 /
= 10
```

연산자와 피연산자가 공백으로 구분된다고 할 때, 내부적으로 stack을 유일한 자료구조로 사용하여 후위 표기법으로 표기된 수식을 계산하는 메소드 `calculate()`을 완성하시오.

```python
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
----


### 과제2 답안(25/25)

- Stack 자료구조를 응용하여 계산기를 구현하는 문제였습니다.
- Stack의 기능을 활용하여 잘 구현해 주셨습니다. 아래 예시답안도 확인해 주세요 :)

예시 답안)

```python
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



## 과제3.

----
다음은 Tree 자료구조를 순회하는 방법 중, Pre-order 순회 방법을 설명한 것이다. 자료구조의 순회란, 자료구조에 속한 모든 data를 한 번씩 접근하는 것이다. Pre-order 순회를 하면서 순회한 순서대로 Node의 data를 출력하는 `preorder()` 메소드를 완성하시오.

- Tree 자료구조를 순회할 때에는 반드시 root node부터 순회를 시작한다.
- Pre-order 순회를 할 때에는 아래와 같은 방법을 재귀적으로 수행한다.
  - 새로운 node에 접근할 경우, 아래 순서대로 동작한다.
    1. Node에 있는 data를 출력한다.
    1. Node에 left child가 있으면, left child node에 접근한다.
    1. Node에 right child가 있으면, right child node에 접근한다.
  - root node에서 순회를 시작할 경우, 재귀적 동작으로 인해 모든 node의 data를 출력할 수 있다.

```python
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

----

### 과제3 답안(0/25)

- Tree의 Preorder traversal(depth-firsth traversal)을 구현하는 문제였습니다.
- 재귀함수를 이용하여 구현하면 쉽게 구현할 수 있습니다.
- 아래 예시 답안을 확인해 주세요 :)

예시 답안)

```python
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

## 과제4.

----
HashTable 클래스는 문자열을 key로 입력받는 해쉬 테이블 자료구조를 구현한 것이다. HashTable 클래스는 단순한 해쉬 함수로 인해, 해쉬 충돌이 빈번히 발생한다. 이 단점을 개선하기 위해, Chaining 기법으로 ChainedHashTable을 구현하고자 한다.

HashTable을 상속하여 해쉬 충돌이 발생해도 정상적으로 동작하는 ChainedHashTable을 완성하시오.

```python
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

----



### 과제4 답안(0/25)

- Hash Table에서 Chaining 기법을 구현하는 문제였습니다.
- 수업시간에 배운 list를 이용하는 방법을 사용해도 되며, 아래 Node를 이용하는 예시 답안도 확인해 주세요 :)

예시 답안)

```python
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



## 과제1.

----
Min Heap 자료구조를 이용하면 최대값을 `O(logN)`의 시간복잡도로 찾을 수 있다. Min Heap을 이용하면 우선순위 값이 낮은 자료를 먼저 출력하는 Priority Queue를 구현할 수 있다. Min Heap을 이용한 Priority Queue는 아래와 같은 특징을 가진다.

- Min Heap을 이용한 Priority Queue의 특징
  - 자료를 입력하는 동작과 출력하는 동작 모두 `O(logN)`으로 이루어진다.
  - 우선순위 값이 낮은 자료를 먼저 출력하되, 우선순위 값이 같은 자료끼리는 순서를 고려하지 않는다.
  - 다음과 같은 Method들을 구현한다.
    1. `is_empty()`: Queue가 비어있으면 True, 비어있지 않으면 False를 출력한다.
    1. `put()`: Priority Queue에 자료를 입력한다. 자료는 길이가 2인 Tuple로, `(우선순위, 자료)` 형태로 입력받는다.
    1. `get()`: Priority Queue에서 자료를 출력한다. 출력한 데이터는 Priority Queue에서 삭제한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.
    1. `peek()`: Priority Queue에서 자료를 출력한다. 출력한 데이터는 Priority Queue에 그대로 유지한다. 더이상 출력할 데이터가 없는 경우 None을 출력한다.



```python
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
```

```python
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
----


### 과제1 답안(0/25)

- 수업시간에 배운 Heap 구조를 이용하여 PriorityQueue를 구현하는 문제였습니다.
- Heap 구조를 직접 구현해 주셔야 하며, 다른 방법을 사용할 경우 시간복잡도 조건이 맞지 않게 됩니다.
- Heap을 구현하시되, 입력을 우선순위와 데이터 2가지를 함께 입력받는 형식으로 구현하시면 됩니다.

예시 답안)

```python
class PriorityQueue:
    def __init__(self):
        self.tree = [None]

    def is_empty(self):
        return len(self.tree) == 1

    def put(self, data):
        self.tree.append(data)
        curr = len(self.tree) - 1
        parent = curr // 2
        while parent > 0:
            if self.tree[curr][0] > self.tree[parent][0]:
                return
            self.tree[curr], self.tree[parent] = self.tree[parent], self.tree[curr]
            curr = parent
            parent = curr // 2

    def get(self):
        if self.is_empty() is True:
            return None
        data = self.tree[1]
        self.tree[1] = self.tree[-1]
        self.tree = self.tree[:-1]
        curr = 1
        while curr < len(self.tree):
            left = curr * 2
            right = curr * 2 + 1
            if left < len(self.tree) and right < len(self.tree):
                if self.tree[left][0] < self.tree[right][0]:
                    if self.tree[left][0] < self.tree[curr][0]:
                        self.tree[curr], self.tree[left] = self.tree[left], self.tree[curr]
                        curr = left
                else:
                    if self.tree[right][0] < self.tree[curr][0]:
                        self.tree[curr], self.tree[right] = self.tree[right], self.tree[curr]
                        curr = right

            elif left < len(self.tree) and self.tree[left][0] < self.tree[curr][0]:
                self.tree[curr], self.tree[left] = self.tree[left], self.tree[curr]
                curr = left
            elif right < len(self.tree) and self.tree[right][0] < self.tree[curr][0]:
                self.tree[curr], self.tree[right] = self.tree[right], self.tree[curr]
                curr = right
            else:
                break
        return data

    def peek(self):
        if self.is_empty() is True:
            return None
        return self.tree[1]

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


## 과제2.

----
오름차순으로 정렬된 N개의 정수를 가진 List가 주어져있을 때, 해당 List에 존재하는 서로 다른 값이 몇 가지인지 알아내는 알고리즘을 구현하라. 알고리즘의 제약사항은 아래와 같다. (알고리즘은 `1 <= N <= 10000`에서 테스트된다.)

- 추가 메모리 사용은 `O(1)`으로 제한된다. 따라서 set()와 dict() 등의 자료구조를 사용할 수 없다.
- 알고리즘의 시간복잡도는 `O(N)` 이하로 제한된다.

```python
def countUniques(a):
    pass

# Test code
print(countUniques([-1, 1, 1, 1, 1, 4, 4, 4, 4, 10, 14, 14])) # 5
print(countUniques([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])) # 2
```
----


### 과제2 답안(25/25)

- 정렬된 리스트의 특성을 이용하여 주어진 스펙에 맞는 알고리즘을 구현하는 문제였습니다.
- O(n)의 시간 복잡도와 O(1)의 공간 복잡도를 만족시키도록 잘 구현해 주셨습니다! :)

예시 답안)

```python
def countUniques(a):
    last_el = None
    count = 0
    for el in a:
        if last_el != el:
            count += 1
        last_el = el
    return count

print(countUniques([-1, 1, 1, 1, 1, 4, 4, 4, 4, 10, 14, 14])) # 5
print(countUniques([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1])) # 2
```


## 과제3.

----
N개의 문자열로 이루어진 List에서 전체 문자열이 앞 n개 문자열이 같다고 할때, 가장 큰 n을 출력하는 알고리즘을 구현하라. (즉, 주어진 모든 문자열의 앞의 몇개의 문자가 일치하는지 출력하라)

```python
def solution(a):
    return 0

# Test code
print(solution(['abcd', 'abce', 'abchg', 'abcfwqw', 'abcdfg'])) # 3
print(solution(['abcd', 'gbce', 'abchg', 'abcfwqw', 'abcdfg'])) # 0
```

----


### 과제3 답안(0/25)

- 문자열 매칭을 다루는 문제였습니다!
- for문과 if문을 적절히 사용하여 주어진 내용을 충실히 구현하면 됩니다 :)

예시 답안)

```python
def solution(a):
    count = 0
    w = a[0]
    for idx, c in enumerate(w):
        is_match = True
        for w_ in a:
            if c != w_[idx]:
                is_match = False
                break
        if is_match is True:
            count += 1
        else:
            break
    return count

print(solution(['abcd', 'abce', 'abchg', 'abcfwqw', 'abcdfg'])) # 3
print(solution(['abcd', 'gbce', 'abchg', 'abcfwqw', 'abcdfg'])) # 0
```




## 과제4.

----
자연수 중, **각 자리수를 제곱한 것을 더하는 과정을 반복했을 때 1으로 끝나는 수**를 '행복한 수'라고 한다. '행복한 수'가 아닌 경우 이 과정이 1에 도달하지 못하고 같은 **수열이 반복되는 무한 루프**에 빠지게 된다. 자연수를 입력받았을 때 '행복한 수'인지 판별하는 알고리즘을 작성하라.

'행복한 수'를 찾는 과정의 예
  ```
  19이 행복한 수인지 확인하는 과정
  1^2 + 9^2 = 82
  8^2 + 2^2 = 68
  6^2 + 8^2 = 100
  1^2 + 0^2 + 0^2 = 1 --> True
  ```

```python
def solution(n):
    return True

# Test code
print(solution(19)) # True
print(solution(61)) # False
```

----


### 과제4 답안(0/25)

- 새로운 개념을 이해하고, 직접 구현해 보는 문제였습니다.
- 재귀적으로 함수를 구현하면 간결하게 구현할 수 있습니다 :)

예시 답안)

```python

def solution(n):
    def calc_value(m):
        val = 0
        for c in str(m):
            val += int(c) ** 2
        return val

    hist = set()
    while n != 1:
        hist.add(n)
        n = calc_value(n)
        if n in hist:
            return False
    return True

print(solution(19)) # True
print(solution(61)) # False
```


### Quiz 5 (2021/04/15 ~ 2021/04/18)

Q1. 다음 중 이진탐색(Binary Search) 알고리즘에 대한 설명으로 옳지 않은 것은?
1. 탐색할 자료를 둘로 나누어 해당 데이터가 있을 만한 곳을 탐색하는 방법이다.
2. 분할정복 알고리즘의 하나로, 하위 문제부터 풀어나가는 bottom-up 방식이다. -> 답
3. 자료 N개를 이진탐색으로 탐색 시, 시간복잡도는 Big-O 표기법으로 O(logN)이다.
4. 이진탐색을 이용하면 순차탐색보다 더 빠르게 탐색이 가능하다.


Q2. 다음 그래프와 트리에 대한 설명 중 옳지 않은 것을 모두 고르시오.
1. 그래프는 노드 및 간선으로 표현되는 자료 구조이며, 트리의 한 종류이다. -> 답 
2. 그래프 사이클이 가능한 반면, 트리는 비순환 그래프로 사이클이 존재하지 않는다.
3. 그래프는 루트 노드가 존재하지 않는 반면, 트리는 루트 노드가 존재한다.
4. 트리는 부모자식 관계가 있으나, 그래프는 부모자식 관계가 존재하지 않는다.


Q3. 아래 그래프를 DFS(깊이우선탐색)로 1번 노드부터 탐색한다고 할 때 방문하는 노드의 순서를 고르시오.
    (단, 여러 개의 노드들이 연결되어 있는 경우, 작은 노드번호를 기준으로 먼저 순회한다.)
1. 1, 2, 3, 4, 5, 6, 7
2. 1, 2, 4, 5, 3, 6, 7
3. 1, 2, 4, 5, 7, 6, 3
4. 1, 2, 4, 7, 5, 6, 3 -> 이거 
5. 1, 2, 4, 7, 5, 3, 6


Q4. 다음은 이진탐색(Binary Search)의 함수이다. 아래 빈칸을 채우시오
def binary_search(data, search):
  if len(data) == 1 and search == data[0]:
    return True
  if len(data) == 1 and search != data[0]:
    return False
  if len(data) == 0:
    return False
    
  medium = len(data)//2
  if search == data[medium]:
    return True
  else:
    if ______:
      return binary_search(data[medium:], search)
    else:
      return binary_search(data[:medium], search)
  
답: search > data[medium]
      
 
Q5. 다음 탐욕 알고리즘에 대한 내용 중 옳은 것은?
1. 탐욕 알고리즘은 매순간 최적이라고 생각되는 해(locally optimal solution)를 선택하는 알고리즘으로,
   최종적으로 항상 최적의 해를 찾을 수 있다.
   -> 탐욕 알고리즘은 매순간 최적이라고 생각되는 경우를 선택하나, 최종 해는 근사치의 값을 찾을 뿐 최적의 값이 아닐 수도 있다.
2. 탐욕 알고리즘은 메모이제이션 기법을 활용하여 중복계산을 방지한다.
   -> 메모이제이션 기법은 동적 계획법에서 사용되는 기법이다.
4. 탐욕 알고리즘은 brute-force 방식의 접근으로, 동적 계획법보다 비효율적이다.
   -> 모든 경우를 확인하는(brute-force) 동적 계획법보다 탐욕 알고리즘이 더 효율적이며, 시간 복잡도가 더 낮다.
6. 탐욕 알고리즘은 매 step마다(매순간) 한 개의 sub-problem만 처리한다. -> 답


Q6. 다음은 재귀함수를 이용하여 factorial을 구현한 함수이다. 아래 빈칸을 채워 함수를 완성하시오
def factorial(num):
  if num > 1:
    return ____
  else:
    return num
  
print(factorial(5))
출력: 120

-> 답: num * factorial(num - 1)

Q7. 다음 그래프에서 다익스트라 알고리즘을 이용하여 최단경로를 구한다고 할 때, A노드와 각 노드들 간의 최단거리를 구하는 과정을 단계별로 나타내었다.
    우선순위 큐를 이용한다고 할 때, STEP4에 채워질 각 노드까지의 거리 중 옳은 것을 고르시오.
    (각 STEP은 우선순위 큐를 한 번 pop할 때마다 업데이트된다.)


Q8. 다음 정렬 알고리즘에 대한 내용 중 옳지 않은 것은?
1. 버블정렬은 두 인접한 데이터의 크기를 비교하여 자리를 바꾸며 정렬하는 알고리즘이다.
2. 병합정렬과 퀵정렬은 재귀함수를 이용하여 구현이 가능하다.
3. 일반적으로 퀵정렬의 시간복잡도는 O(NlogN)이나, pivot으로 가장 크거나 작은 수를 선택하는 최악의 경우 O(N^3)의 시간복잡도를 가지기도 한다 -> 답
4. 선택정렬은 주어진 데이터의 최소값을 찾아, 데이터의 맨 앞과 위치를 교체하며 정렬하는 방식으로 시간복잡도는 항상 O(N^2)이다.


Q9. 다음은 퀵정렬(quick sort)을 구현한 코드이다. 아래 빈칸을 채워 퀵정렬 함수를 완성하시오.
def quicksort(data_list):
  if len(data_list) <= 1:
    return data_list
  pivot = data_list[0]
  
  left = [item for item in data_list[1:] if pivot > item]
  right = [item for item in data_list[1:] if pivot <= item]
  
  return ___+ [] +____
  
data_list = [50, 90, 1, 14, 8, 21, 65]
print(quicksort(data_list))

출력: [1, 8, 14, 21, 50, 65, 90]

-> 답: quicksort(left) + [pivot] + quicksort(right)

Q10. 최소 신장 트리를 구하는 알고리즘 중 하나로, 전체 그래프에서 최소비용인 간선을 하나씩 추가해 나가는 알고리즘의 이름을 쓰시오.

-> 크루스칼 



### Report 5 (2021/04/15 ~ 2021/04/18)


## 과제1.

----
이진 탐색법은 정렬된 자료를 탐색하는 데에 사용할 수 있다. 인덱스가 낮을 수록 더 작은 값으로 정렬된 2차원 리스트에서 `target`을 찾으면 True를 반환하고, `target`을 찾을 수 없으면 False를 반환하는 프로그램을 작성하시오.

예시 입력1
```python
matrix = [
  [1,   3,  5,  7],
  [10, 11, 16, 20],
  [23, 30, 34, 50]
]
target = 3
출력: True
```

예시 입력2
```python
matrix = [
  [1,   3,  5,  7],
  [10, 11, 16, 20],
  [23, 30, 34, 50]
]
target = 13
출력: False
```

```python
def searchMatrix(matrix, target):
    pass
```
----

### 과제1 답안(0/25)

- 이진 탐색법을 2차원 배열에 대해서 구현하는 문제였습니다.
- 첫번째 탐색을 범위에 대해서 수행하고, 두번째 탐색을 기존에 배운 내용으로 수행하면 해결할 수 있습니다 :)

예시 답안)

```python
def searchMatrix(matrix, target):
    def searchRow(sub_matrix):
        m = len(sub_matrix)

        if m == 1:
            return sub_matrix[0]

        mid = m // 2
        left = sub_matrix[:mid]
        right = sub_matrix[mid+1:]

        if sub_matrix[mid][0] <= target <= sub_matrix[mid][-1]:
            return sub_matrix[mid]
        elif sub_matrix[mid][0] > target:
            return searchRow(left)
        else:
            return searchRow(right)

    def searchCol(array):
        n = len(array)

        if n == 0:
            return False

        if n == 1:
            if array[0] == target:
                return True
            else:
                return False

        mid = n // 2
        left = array[:mid]
        right = array[mid+1:]

        if array[mid] == target:
            return True
        elif array[mid] > target:
            return searchCol(left)
        else:
            return searchCol(right)

    array = searchRow(matrix)
    return searchCol(array)


## 과제2.

----
두 문자열 A와 B가 있을 때, 두 문자열의 '최대공약문자열' C를 아래와 같이 정의하자.

1. 문자열 C를 반복하여 문자열 A와 B를 생성할 수 있다.
1. 가능한 C 중에 가장 긴 문자열을 C로 한다.
1. 위 조건을 만족하는 C가 없으면 빈 문자열을 C로 한다.

이 때, 문자열 A와 B를 입력받아 C를 출력하는 프로그램을 작성하시오.

예시입력1
```python
A = 'ababcde'
B = 'ababcde'
출력: 'ababcde'
```

예시입력2
```python
A = 'ababababab'
B = 'abab'
출력: 'ab'
```

예시입력3
```python
A = 'abababab'
B = 'abab'
출력: 'abab'
```

예시입력3
```python
A = 'fast'
B = 'campus'
출력: ''
```

```python
def gcdString(A, B):
    pass
```
----


### 과제2 답안(25/25)

- 탐욕 알고리즘으로 적절한 답안을 찾아내는 문제였습니다.
- 문제에서 제시하는 정의에 맞게 잘 구현해 주셨습니다 :)

예시 답안)

```python

def gcdString(A, B):
    def isDivisor(string, divisor):
        n = len(divisor)
        if len(string) % n != 0:
            return False
        
        while string != '':
            if string[:n] != divisor:
                return False
            string = string[n:]
        return True
    
    if len(A) > len(B):
        str1, str2 = A, B
    else:
        str1, str2 = B, A
    
    divisor = str2
    m = 1
    while divisor != '':
        if isDivisor(str2, divisor) and isDivisor(str1, divisor):
            return divisor
        m += 1
        divisor = str2[:len(str2) // m]
    return ''

A = 'ababcde'
B = 'ababcde'
print(gcdString(A, B))

A = 'ababababab'
B = 'abab'
print(gcdString(A, B))

A = 'abababab'
B = 'abab'
print(gcdString(A, B))

A = 'fast'
B = 'campus'
print(gcdString(A, B))
```


## 과제3.

----
n개의 노드가 있는 그래프가 있다. 각 노드는 1부터 n까지 번호가 적혀있다. 1번 노드에서 가장 멀리 떨어진 노드의 갯수를 구하려고 한다. 가장 멀리 떨어진 노드란 최단경로로 이동했을 때 간선의 개수가 가장 많은 노드들을 의미한다.

노드의 개수 n, 간선에 대한 정보가 담긴 2차원 배열 vertex가 매개변수로 주어질 때, 1번 노드로부터 가장 멀리 떨어진 노드가 몇 개인지를 return 하도록 solution 함수를 작성하라.

- 제한사항
  - 노드의 개수 n은 2 이상 20,000 이하입니다.
  - 간선은 양방향이며 총 1개 이상 50,000개 이하의 간선이 있습니다.
  - vertex 배열 각 행 `[a, b]`는 a번 노드와 b번 노드 사이에 간선이 있다는 의미입니다.

- 입출력 예

|n|vertex|return|
|--|-----|------|
|6|`[[3, 6], [4, 3], [3, 2], [1, 3], [1, 2], [2, 4], [5, 2]]`|3|


```python
def solution(n, vertex):
    return 0

```

----


### 과제3 답안(0/25)

- 그래프 구조에서 최단 거리를 구하는 문제였습니다.
- 다익스트라 알고리즘을 구현하면 되는 문제였습니다 :)

예시 답안)

```python
import heapq

def solution(n, vertex):
    to_visit = []
    dists = [float('inf')] * (n + 1)
    
    dists[1] = 0
    heapq.heappush(to_visit, (0, 1))
    while len(to_visit) > 0:
        dist, node = heapq.heappop(to_visit)
        adj_list = list(map(lambda x: x[1], filter(lambda x: x[0] == node, vertex)))
        adj_list += list(map(lambda x: x[0], filter(lambda x: x[1] == node, vertex)))
        for adj_node in adj_list:
            if dists[adj_node] > dist + 1:
                dists[adj_node] = dist + 1
                heapq.heappush(to_visit, (dists[adj_node], adj_node))
    
    return dists.count(max(dists[1:]))
    
n = 6
vertex = [[3, 6], [4, 3], [3, 2], [1, 3], [1, 2], [2, 4], [5, 2]]
print(solution(n, vertex))
```


## 과제4.

----
마을에 1부터 N의 고유 번호를 가진 사람들이 있다. 소문으로는 마을 사람 중에 마을 판사가 있다고 한다. 마을 판사가 실제로 존재한다면,

- 마을 판사는 아무도 믿지 않는다.
- 다른 모든 사람들은 마을 판사를 믿는다.
- 마을 판사가 있다면 오직 한명 뿐이다.

리스트 trust가 주어졌을 때, `trust[i] = [a, b]`는 고유 번호가 a인 사람이 고유 번호가 b인 사람을 믿는다는 것을 의미한다고 한다. 

마을 판사가 존재한다면 마을 판사의 고유 번호를, 존재하지 않는다면 -1을 출력하는 프로그램을 작성하시오.

(단, a가 b를 믿고 b가 c를 믿는다고 할 때, a가 c를 믿는다는 의미는 아니다.)

예시입력

|N| trust| 출력|
|-|------|----|
|2| `[[1,2]]`| 2|
|3| `[[1,3],[2,3]]` | 3 |
|3| `[[1,3],[2,3],[3,1]]`| -1 |
|3|`[[1,2],[2,3]]` | -1 |
|4|`[[1,3],[1,4],[2,3],[2,4],[4,3]]`| 3 |

```python
def solution(N, trust):
    return -1
```

----


### 과제4 답안(25/25)

- 그래프 구조의 구성을 이해하는 문제였습니다.
- 잘 구현해 주셨습니다! :) 아래 예시 답안도 확인해 주세요 :)

예시 답안)

```python
def solution(N, trust):
    for i in range(1, N + 1):
        if len(list(filter(lambda x: x[0] == i, trust))) > 0:
            continue
        if len(list(filter(lambda x: x[1] == i, trust))) == N - 1:
            return i
    return -1

print(solution(2, [[1,2]])) # 2
print(solution(3, [[1,3],[2,3]])) #3
print(solution(3, [[1,3],[2,3],[3,1]])) #-1
print(solution(3, [[1,2],[2,3]])) #-1
print(solution(4, [[1,3],[1,4],[2,3],[2,4],[4,3]])) #3
```




### Report 6 (2021/04/22 ~ 2021/04/25)


## 과제1.

----
리스트 `[1,2,3,...,n]` 를 섞는 방법은 총 `n!` 가지이다. `n = 3`일 때 `3! = 6`개의 섞은 결과는 아래와 같은 순서를 가진다고 하자.

```python
[1, 2, 3]
[1, 3, 2]
[2, 1, 3]
[2, 3, 1]
[3, 1, 2]
[3, 2, 1]
```

n과 k가 주어졌을 때, k번째 섞은 결과를 반환하시오. (단, `1 <= n <= 9`, `1 <= k <= n!`)

예시입력

|n|k|return|
|-|-|--|
|3|3|`[2, 1, 3]`|
|4|9|`[2, 3, 1, 4]`|

```python
def solution(n, k):
    return []
```
----

### 과제1 답안(0/20)

- 탐욕법을 이용하여 가능한 조합을 빠르게 계산하는 문제였습니다.
- factorial은 동적계획법을 이용하고, 조합 계산은 탐욕법을 사용하는 응용 형식으로 문제를 해결할 수 있습니다 :)
- 아래 예시 답안을 확인해 주세요!

예시 답안)

```python
def solution(n, k):
    fact = {0: 1}
    def factorial(num):
        if num in fact:
            return fact[num]
        val = factorial(num - 1) * num
        fact[num] = val
        return val
    
    remainder = k - 1
    seq = [i for i in range(1, n + 1)]
    ans = []
    for i in range(n - 1, 0, -1):
        div = factorial(i)
        val = remainder // div
        remainder %= div
        ans.append(seq[val])
        del seq[val]
    ans.append(seq[0])
    return ans

print(solution(3, 3))
print(solution(4, 9))
```


## 과제2.

----
아래와 같이 5와 사칙연산만으로 12를 표현할 수 있습니다.

```
12 = 5 + 5 + (5 / 5) + (5 / 5)
12 = 55 / 5 + 5 / 5
12 = (55 + 5) / 5
```

5를 사용한 횟수는 각각 6,5,4 입니다. 그리고 이중 가장 작은 경우는 4입니다.
이처럼 숫자 N과 number가 주어질 때, N과 사칙연산만 사용해서 표현 할 수 있는 방법 중 N 사용횟수의 최솟값을 return 하도록 solution 함수를 작성하세요.

제한사항

- N은 1 이상 9 이하입니다.
- number는 1 이상 32,000 이하입니다.
- 수식에는 괄호와 사칙연산만 가능하며 나누기 연산에서 나머지는 무시합니다.
- 최솟값이 8보다 크면 -1을 return 합니다.

입출력 예

|N|number|return|
|-|------|-----|
|5|12|4|
|2|11|3|

입출력 예 설명

- 예제 #1: 문제에 나온 예와 같습니다.
- 예제 #2: `11 = 22 / 2`와 같이 2를 3번만 사용하여 표현할 수 있습니다.

```python
def solution(N, number)
    return 0
```
----


### 과제2 답안(20/20)

- 동적계획법을 이용해, 부분 문제의 결과를 취합해 더 복잡한 문제를 해결하는 문제였습니다.
- 문제의 요구사항에 맞게 충실하게 잘 구현해 주셨습니다! :)
- 아래 예시 답안을 확인해 주세요 :)

예시 답안)

```python
def solution(N, number):
    sets = [{}, {N}]
    
    if N == number:
        return 1
    
    for i in range(2, 9):
        current_set = {int(str(N)*i)}
        for j in range(1, i // 2 + 1):
            for val_j in sets[j]:
                for val_k in sets[i - j]:
                    current_set.add(val_j + val_k)
                    current_set.add(val_j - val_k)
                    current_set.add(val_k - val_j)
                    current_set.add(val_j * val_k)
                    if val_k != 0:
                        current_set.add(val_j // val_k)
                    if val_j != 0:
                        current_set.add(val_k // val_j)
                    
                    if number in current_set:
                        return i
        sets.append(current_set)
    return -1
```


## 과제3.

----
n개의 정수로 이루어진 리스트 nums와 정수 target이 주어졌을 때, nums에 있는 정수 4개를 합하여 target을 만들 수 있는 모든 조합을 구하시오. 단, 정답에는 동일한 정수 조합이 여러개 포함되어서는 안된다.

예시 입력
```python
nums = [1, 0, -1, 0, -2, 2]
target = 0
```
출력:
```
[
  [-1,  0, 0, 1],
  [-2, -1, 1, 2],
  [-2,  0, 0, 2]
]
```

```python
def solution(nums, target):
    return []
```

----

### 과제3 답안(20/20)

- 주어진 문제에 맞게 충실하게 잘 구현해 주셨습니다! :)
- 아래 예시답안도 확인해 보시고 비교해 보세요 :)

예시 답안)

```python
def solution(nums, target):
    n = len(nums)
    sets = []
    ans = []
    for i in range(n - 3):
        for j in range(i + 1, n - 2):
            for k in range(j + 1, n - 1):
                for l in range(k + 1, n):
                    curr = [nums[i], nums[j], nums[k], nums[l]]
                    if sum(curr) == target:
                        if set(curr) not in sets:
                            ans.append(curr)
                            sets.append(set(curr))
    return ans
```



## 과제4.

----
정수로 이루어진 수열 x가 주어졌을 때, `x[i-1] < x[i], x[i+1] < x[i]`인 `x[i]`를 피크라고 부른다. a에 피크가 단 하나 반드시 존재할 때, 이 피크를 찾아 출력하는 `O(logN)` 알고리즘을 구현하시오.

예시 입력

|x | return|
|--|----|
|`[-4, -4, -2, 0, 0, 2, 4, 5, 6, 3, 2, -4, -6]` | 6 |
|`[-1, -1, -1, -1, 0, 1, 20, 19, 17]` | 20 |

```python
def solution(x):
    return 0
```

----


### 과제4 답안(0/20)

- 이진 탐색의 응용문제로, O(logN) 복잡도를 실현하는 문제였습니다.
- 기능 구현은 다양하게 가능하나, 이진 탐색으로 구현해야 O(N)이 아닌 O(logN)으로 동작하는 점 확인해 주세요 :)

예시 답안)

```python
def solution(x):
    n = len(x)
    
    if n < 3:
        return None
    
    mid = x[n//2 - 1 : n // 2 + 2]
    left = x[:n//2 + 1]
    right = x[n//2:]
    
    if mid[0] < mid[1] and mid[1] > mid[2]:
        return mid[1]
    elif mid[0] > mid[1]:
        return solution(left)
    else:
        return solution(right)

print(solution([-4, -4, -2, 0, 0, 2, 4, 5, 6, 3, 2, -4, -6]))
print(solution([-1, -1, -1, -1, 0, 1, 20, 19, 17]))
```


## 과제5.

----

그래프를 DFS로 탐색한 결과를 출력하는 프로그램을 작성하시오. 단, 방문할 수 있는 정점이 여러 개인 경우에는 정점 번호가 작은 것을 먼저 방문하고, 더 이상 방문할 수 있는 점이 없는 경우 종료한다. 정점 번호는 1번부터 N번까지이다.

- 입력: 첫째 줄에 정점의 개수 N(1 ≤ N ≤ 1,000), 간선의 개수 M(1 ≤ M ≤ 10,000), 탐색을 시작할 정점의 번호 V가 주어진다. 다음 M개의 줄에는 간선이 연결하는 두 정점의 번호가 주어진다. 어떤 두 정점 사이에 여러 개의 간선이 있을 수 있다. 입력으로 주어지는 간선은 양방향이다.

- 출력: V부터 방문된 점을 순서대로 출력한다.

- 예시 입출력

|N| M| V| edges| 출력|
|--|--|--|-----|-------|
|4|5|1|[[1, 2], [1, 3], [1,4], [2, 3], [3, 4]]|1 2 3 4|

----

### 과제5 답안(20/20)

- DFS를 구현하는 문제였습니다.
- 잘 구현해 주셨습니다 :) 아래 예시 답안과 테스트 코드도 확인해 보세요!

예시 답안)

```python
def solution(N, M, V, edges):
    visited = []
    adj_lists = [[]]*(N + 1)
    for i in range(1, N + 1):
        adj_list = list(map(lambda x:x[1], (filter(lambda x:x[0] == i, edges)))) + list(map(lambda x:x[0], (filter(lambda x:x[1] == i, edges))))
        adj_list.sort()
        adj_lists[i] = adj_list
    
    def dfs(node):
        visited.append(node)
        print(node, end=' ')
        for n in adj_lists[node]:
            if n not in visited:
                dfs(n)
    dfs(V)
    
N, M, V = 4, 5, 1
edges = [[1, 2], [1, 3], [1,4], [2, 3], [3, 4]]
solution(N, M, V, edges)
```
  


### Report 7 (2021/04/29 ~ 2021/05/02)


## 과제1.

----
0 또는 양의 정수가 주어졌을 때, 정수를 이어 붙여 만들 수 있는 가장 큰 수를 알아내 주세요.

예를 들어, 주어진 정수가 `[6, 10, 2]`라면 `[6102, 6210, 1062, 1026, 2610, 2106]`를 만들 수 있고, 이중 가장 큰 수는 `6210`입니다.

0 또는 양의 정수가 담긴 배열 numbers가 매개변수로 주어질 때, 순서를 재배치하여 만들 수 있는 가장 큰 수를 문자열로 바꾸어 return 하도록 solution 함수를 작성해주세요.

- 제한 사항
  - numbers의 길이는 1 이상 100,000 이하입니다.
  - numbers의 원소는 0 이상 1,000 이하입니다.
  - 정답이 너무 클 수 있으니 문자열로 바꾸어 return 합니다.

- 입출력 예


  | numbers | return |
  |--------|--------|
  |`[6, 10, 2]` | 6210 |
  |`[3, 30, 34, 5, 9]` | 9534330 |


```python
def solution(numbers):
    answer = 0
    return answer
```
----

### 과제1 답안(25/25)

- 정렬 기준을 설정하고, 정렬을 할 수 있는지 여부를 묻는 문제였습니다.
- 정답을 잘 구현해 주셨습니다! 아래 예시 답안도 확인해 주세요 :)

예시 답안)

```python

def cmp_to_key(mycmp):
    'Convert a cmp= function into a key= function'
    class K:
        def __init__(self, obj, *args):
            self.obj = obj
        def __lt__(self, other):
            return mycmp(self.obj, other.obj) < 0
        def __gt__(self, other):
            return mycmp(self.obj, other.obj) > 0
        def __eq__(self, other):
            return mycmp(self.obj, other.obj) == 0
        def __le__(self, other):
            return mycmp(self.obj, other.obj) <= 0
        def __ge__(self, other):
            return mycmp(self.obj, other.obj) >= 0
        def __ne__(self, other):
            return mycmp(self.obj, other.obj) != 0
    return K

def compare(x, y):
    a = int(str(x) + str(y))
    b = int(str(y) + str(x))
    return b - a

def solution(numbers):
    numbers.sort(key=cmp_to_key(compare))
    answer = ''.join(list(map(str, numbers)))
    
    if answer[0] == '0':
        answer = str(int(answer))
    
    return answer

print(solution([6, 10, 2]))
print(solution([3, 30, 34, 5, 9]))
```


## 과제2.

----
여러 개의 구간이 리스트 intervals로 주어졌을 때, 겹치는 구간을 모두 병합하여 출력하시오.

입력 예시1

```
입력: intervals = [[1,3],[2,6],[8,10],[15,18]]
출력: [[1,6],[8,10],[15,18]]
설명: 구간 [1,3]와 [2,6]이 겹치므로, [1,6]으로 병합하였다.
```

입력 예시 2

```
입력: intervals = [[1,4],[4,5]]
출력: [[1,5]]
설명: 구간 [1,4]와 [4,5]는 겹치는 것으로 간주한다.
```

```python
def solution(intervals)
    return []
```
----

### 과제2 답안(25/25)

- 재귀적으로 구현하면 비교적 쉽게 구현할 수 있는 구현 문제였습니다.
- 요구사항에 맞게 잘 구현해 주셨습니다! :) 아래 예시 답안도 확인해 주세요 :)

예시 답안)

```python

def solution(intervals):
    intervals.sort()
    
    def merge(x):
        if len(x) <= 1:
            return x
        
        to_merge = [x[0]]
        del x[0]
        while len(x) > 0:
            if to_merge[0][1] >= x[0][0]:
                to_merge.append(x[0])
                del x[0]
            else:
                break
        
        merged = [to_merge[0][0], max(map(lambda e: e[1], to_merge))]
        return [merged] + merge(x)
    
    return merge(intervals)

intervals = [[1,3],[2,6],[8,10],[15,18]]
print(solution(intervals))

intervals = [[1,4],[4,5]]
print(solution(intervals))
```


## 과제3.

----
문자열 s1, s2, s3가 주어졌을 때, 문자열 s3가 문자열 s1과 s2를 교차로 배치하여 만들어질 수 있는지 여부를 출력하라.

예시 입력1

```
입력: s1 = "aabcc", s2 = "dbbca", s3 = "aadbbcbcac"
출력: True
```
예시 입력2

```
입력: s1 = "aabcc", s2 = "dbbca", s3 = "aadbbbaccc"
출력: False
```

```python
def solution(s1, s2, s3):
    return False
```

----

### 과제3 답안(25/25)

- 그래프를 탐색하는 문제였습니다!
- DFS를 이용하면 효율적으로 동작하는 알고리즘을 구현할 수 있습니다. 아래 예시답안을 확인해 주세요 :)

예시 답안)

```python
def solution(s1, s2, s3):
    found = False
    
    def dfs(str1, str2, str3):
        nonlocal found
        n, m = len(str1), len(str2)
        
        if found is True:
            return
        
        if str3 == s3:
            found = True
            return
        
        if n > 0 and str1[0] == s3[len(str3)]:
            dfs(str1[1:], str2, str3 + str1[0])
        
        if m > 0 and str2[0] == s3[len(str3)]:
            dfs(str1, str2[1:], str3 + str2[0])
    
    dfs(s1, s2, '')
    return found

s1 = "aabcc"
s2 = "dbbca"
s3 = "aadbbcbcac"
print(solution(s1, s2, s3))

s1 = "aabcc"
s2 = "dbbca"
s3 = "aadbbbaccc"
print(solution(s1, s2, s3))
```


## 과제4.

----
2개의 단어 beginWord와 endWord, 그리고 여러개의 단어 wordList가 주어졌을 때, beginWord에서 endWord로 변환하기 위해 필요한 가장 적은 변환 횟수를 구하시오.

- 변환 조건
  - 단어는 wordList에 있는 단어로만 변환할 수 있다.
  - 단어를 변환할 때에는 한번에 하나씩의 문자만 바꿀 수 있다.

- 문제 조건
  - endWord로의 변환이 불가한 경우에는 0을 출력하시오.
  - 문제에 등장하는 모든 단어의 길이는 같으며, 알파벳 소문자로만 이루어져 있다.
  - wordList에는 겹치는 단어가 없다.
  - beginWord와 endWord는 같은 단어로 주어지지 않는다.

예시 입력1

```
입력:
beginWord = "hit",
endWord = "cog",
wordList = ["hot","dot","dog","lot","log","cog"]

출력: 5

설명: 가장 짧은 변환 방법은 "hit" -> "hot" -> "dot" -> "dog" -> "cog"이다.
```

예시 입력2

```
입력:
beginWord = "hit"
endWord = "cog"
wordList = ["hot","dot","dog","lot","log"]

출력: 0

설명: endWord인 "cog"가 wordList에 없으므로, endWord로 변환할 수 있는 방법이 없다.
```

```python
def solution(beginWord, endWord, wordList):
    return 0
```

----

### 과제4 답안(0/25)

- 문제를 그래프로 해석하여 탐색하는 문제였습니다.
- 한 문자씩 차이나는 단어로 인접 리스트를 구현하는 문제였습니다 :) 아래 예시 답안을 확인해주세요!

예시 답안)

```python

def isAdj(s1, s2):
    count = 0
    for c1, c2 in zip(s1, s2):
        if c1 != c2:
            count += 1
        if count > 1:
            return False
    return count == 1
    

def solution(beginWord, endWord, wordList):
    adjMap = {w: list(filter(lambda ww: isAdj(w, ww), wordList)) for w in wordList}
    adjList = list(filter(lambda w: isAdj(beginWord, w), wordList))
    visited = set()
    queue = list(map(lambda x: (1, x), adjList))
    
    while len(queue) > 0:
        count, word = queue.pop()
        
        if word == endWord:
            return count + 1
        
        if word not in visited:
            visited.add(word)
            queue = list(map(lambda x: (count + 1, x), adjMap[word])) + queue
            
    return 0


beginWord = "hit"
endWord = "cog"
wordList = ["hot","dot","dog","lot","log","cog"]
print(solution(beginWord, endWord, wordList))

beginWord = "hit"
endWord = "cog"
wordList = ["hot","dot","dog","lot","log"]
print(solution(beginWord, endWord, wordList))
```



### Report 8 (2021/05/06 ~ 2021/05/09)

## 과제1.

----
패캠이는 아메바를 분열시키는 취미가 생겼다. 패캠이는 아메바 하나하나가 모두 소중하기 때문에, 새로 생겨난 아메바는 모두 새로운 이름을 지어주기로 하였다. 이번에 분열하기로 한 아메바는 아래와 같은 특성을 가진다.

- 아메바가 분열하여 두 개체로 완전히 나뉘는 데에는 1분이 걸린다.
- 분열한 아메바 중 하나는 곧바로 분열을 시작하고, 다른 하나는 1분간 휴식 후 분열을 시작한다.
- 분열하면 기존의 개체는 사라지고 새로운 두 개체가 생긴 것으로 본다.
- 분열되는 도중에는 기존의 개체가 남아있고, 아직 새로운 개체가 생겨나지 않은 것으로 본다.

패캠이는 아메바 한 개체를 분열 시키기 시작한 후, N분 후까지 만들어진 모든 아메바 개체에 새로운 이름을 지어주기로 했다. 패캠이가 준비해야 하는 아메바의 이름은 총 몇 개인가?


- 입출력 예


  | N | return |
  |--------|--------|
  | 2 | 5 |
  | 4 | 15 |


```python
def solution(N):
    answer = 0
    return answer
```
----



## 과제2.

----
철수는 개발자에서 은퇴하여 치킨집을 하게 되었다. 철수는 뛰어난 개발 실력으로 N대의 자동 튀김기를 만들어냈다. i번째 자동 튀김기는 치킨을 한 번 튀기는 데에 fry[i] 만큼의 시간이 걸리며, 튀김이 한번 끝나면 clean[i] 만큼의 시간동안 자동 세척을 한다.

철수가 C 번 치킨을 튀겨내려고 할 때, 최소한 몇 시간 동안 자동 튀김기를 가동해야 하는지 계산하시오.

제약 사항
- 0 < N <= 100000
- fry[i]는 0 < fry[i] <= 100를 만족하는 정수
- clean[i]는 0 < clean[i] <= 100를 만족하는 정수
- 0 < C <= 100000


- 입출력 예


  | N | fry | clean | C | return |
  |---|-----|-------|---|--------|
  | 2 | `[3, 6]` | `[2, 1]` | 20 | 58 |
  | 4 | `[2, 2, 1, 3]` | `[2, 4, 3, 2]` | 2 | 2 |

```python
def solution(N, fry, clean, C)
    answer = 0
    return answer
```
----



## 과제3.

----
민수는 최근 숫자 세기 놀이에 푹 빠져있다. 민수는 숫자를 N진수로 세며, 9보다 큰 숫자는 한자리로 표현하기 위해 아래와 같이 바꾸어서 센다.

- 10 ~ 35:  a~z (알파벳 소문자)
- 36 ~ 61:  A~Z (알파벳 대문자)

민수가 N진수의 숫자를 start부터 end까지 센 결과를 counts라고 할 때, 민수가 잘 못 센 숫자의 개수를 반환하는 함수를 구현하시오.

(단, 2 < N <= 61, start < end이며, counts의 길이는 (end - start + 1)이다.)


- 입출력 예시


  | N | start | end | counts | return |
  |---|-----|-------|---|--------|
  | 13 | `'9'` | `'d'` | `['9', 'a', 'c', 'd', 'e']` | 3 |
  | 62 | `'Z'` | `'12'` | `['Z', '10', '11', '12']` | 0 |

```python
def solution(N, start, end, counts):
    answer = 0
    return answer
```

----



## 과제4.

----
철수와 영희는 함께 여행을 가기로 했다. 단짝인 두 친구는 계속 붙어다니기로 하고 각자의 짐을 모두 모아서, 두 가방에 적절하게 함께 나누어 담기로 했다. 즉, 총 N개의 짐을 무게 K1, K2만큼 담을 수 있는 가방에 각각 나누어 담고자 한다. i번째 짐의 무게와 가치가 각각 W[i]와 V[i]로 주어졌을 때, 두 사람이 담을 수 있는 짐의 가치의 합 중 최대값을 구하시오.

- 입출력 예시


  | N | K1 | K2 | W | V | return |
  |---|-----|-------|---|--|--------|
  | 4 | 3 | 8 | [1, 5, 6, 3] | [5, 2, 14, 6] | 19 |
  

```python
def solution(N, K1, K2, W, V):
    answer = 0
    return answer
```

----


### Final Report (2021/05/06 ~ 2021/05/09)

## 과제1.

----
문자열을 뒤에서부터 읽어도 원래 문자열과 같은 단어를 팰린드롬이라 한다.

입력으로 주어진 문자열이 팰린드롬인지 판별한 뒤, 팰린드롬이면 빈 문자열을 출력한다.

입력된 문자열이 팰린드롬이 아닐 경우 문자열을 반으로 나누어 앞부분의 단어를 기준으로 팰린드롬 단어로 만드는 함수를 작성하시오.

예시 입력1

```
입력: s = 'abcdcba'
출력: ''
```

예시 입력2

```
입력: s = 'bannana'
출력: 'bannab'
```

예시 입력3

```
입력: s = 'wabe'
출력: 'waaw'
```

```python
def solution(s):
    return ''

s = 'abcdcba'
print(solution(s))

s = 'bannana'
print(solution(s))

s = 'wabe'
print(solution(s))
```
----

## 과제2.

----
수많은 마라톤 선수들이 마라톤에 참여하였습니다. 단 한 명의 선수를 제외하고는 모든 선수가 마라톤을 완주하였습니다.

마라톤에 참여한 선수들의 이름이 담긴 배열 participant와 완주한 선수들의 이름이 담긴 배열 completion이 주어질 때, 완주하지 못한 선수의 이름을 return 하도록 solution 함수를 작성해주세요.

- 제한사항
  - 마라톤 경기에 참여한 선수의 수는 1명 이상 100,000명 이하입니다.
  - completion의 길이는 participant의 길이보다 1 작습니다.
  - 참가자의 이름은 1개 이상 20개 이하의 알파벳 소문자로 이루어져 있습니다.
  - 참가자 중에는 동명이인이 있을 수 있습니다.

- 입출력 예시

|participant|completion|return|
|-----|-------|------|
|["leo", "kiki", "eden"]|["eden", "kiki"]|"leo"|
|["marina", "josipa", "nikola", "vinko", "filipa"]| ["josipa", "filipa", "marina", "nikola"]|"vinko"| 
|["mislav", "stanko", "mislav", "ana"]|["stanko", "ana", "mislav"]|"mislav"| 

- 입출력 예에 대한 설명
  - 예제 1: "leo"는 참여자 명단에는 있지만, 완주자 명단에는 없기 때문에 완주하지 못했습니다.
  - 예제 2: "vinko"는 참여자 명단에는 있지만, 완주자 명단에는 없기 때문에 완주하지 못했습니다.
  - 예제 3: "mislav"는 참여자 명단에는 두 명이 있지만, 완주자 명단에는 한 명밖에 없기 때문에 한명은 완주하지 못했습니다.

```python
def solution(participant, completion):
    return []

participant = ["leo", "kiki", "eden"]
completion = ["eden", "kiki"]
print(solution(participant, completion))

participant = ["marina", "josipa", "nikola", "vinko", "filipa"]
completion = ["josipa", "filipa", "marina", "nikola"]
print(solution(participant, completion))

participant = ["mislav", "stanko", "mislav", "ana"]
completion = ["stanko", "ana", "mislav"]
print(solution(participant, completion))
```
----



## 과제3.

----
배열 array의 i번째 숫자부터 j번째 숫자까지 자르고 정렬했을 때, k번째에 있는 수를 구하려 합니다.

예를 들어 array가 [1, 5, 2, 6, 3, 7, 4], i = 2, j = 5, k = 3이라면,

- array의 2번째부터 5번째까지 자르면 [5, 2, 6, 3]입니다.
- 1에서 나온 배열을 정렬하면 [2, 3, 5, 6]입니다.
- 2에서 나온 배열의 3번째 숫자는 5입니다.

배열 array, [i, j, k]를 원소로 가진 2차원 배열 commands가 매개변수로 주어질 때, commands의 모든 원소에 대해 앞서 설명한 연산을 적용했을 때 나온 결과를 배열에 담아 return 하도록 solution 함수를 작성해주세요.

- 제한사항
  - array의 길이는 1 이상 100 이하입니다.
  - array의 각 원소는 1 이상 100 이하입니다.
  - commands의 길이는 1 이상 50 이하입니다.
  - commands의 각 원소는 길이가 3입니다.

- 입출력 예

|array|commands|return|
|-----|-------|------|
|[1, 5, 2, 6, 3, 7, 4]|[[2, 5, 3], [4, 4, 1], [1, 7, 3]]|[5, 6, 3]|

- 입출력 예에 대한 설명
 - [1, 5, 2, 6, 3, 7, 4]를 2번째부터 5번째까지 자른 후 정렬합니다. [2, 3, 5, 6]의 세 번째 숫자는 5입니다.
 - [1, 5, 2, 6, 3, 7, 4]를 4번째부터 4번째까지 자른 후 정렬합니다. [6]의 첫 번째 숫자는 6입니다.
 - [1, 5, 2, 6, 3, 7, 4]를 1번째부터 7번째까지 자릅니다. [1, 2, 3, 4, 5, 6, 7]의 세 번째 숫자는 3입니다.

```python
def solution(array, commands):
    answer = []
    return answer

array = [1, 5, 2, 6, 3, 7, 4]
commands = [[2, 5, 3], [4, 4, 1], [1, 7, 3]]
print(solution(array, commands))
```

----


## 과제4. 삼성 SW 역량 테스트 유사 문제

----
상담원으로 일하고 있는 백준이는 퇴사를 하려고 한다.

오늘부터 N+1일째 되는 날 퇴사를 하기 위해서, 남은 N일 동안 최대한 많은 상담을 하려고 한다.
백준이는 비서에게 최대한 많은 상담을 잡으라고 부탁을 했고, 비서는 하루에 하나씩 서로 다른 사람의 상담을 잡아놓았다.

각각의 상담은 상담을 완료하는데 걸리는 기간 Ti와 상담을 했을 때 받을 수 있는 금액 Pi로 이루어져 있다.
N = 7인 경우에 다음과 같은 상담 일정표를 보자.

|  |1일 | 2일 | 3일 | 4일 | 5일 | 6일 | 7일 |
|--|---|-----|-----|----|----|-----|-----|
|Ti |3 | 5 |1 |1 |2|4|2|
|Pi |10|20|10|20|15|40|200|

- 1일에 잡혀있는 상담은 총 3일이 걸리며, 상담했을 때 받을 수 있는 금액은 10이다. 5일에 잡혀있는 상담은 총 2일이 걸리며, 받을 수 있는 금액은 15이다.
- 상담을 하는데 필요한 기간은 1일보다 클 수 있기 때문에, 모든 상담을 할 수는 없다. 예를 들어서 1일에 상담을 하게 되면, 2일, 3일에 있는 상담은 할 수 없게 된다. 2일에 있는 상담을 하게 되면, 3, 4, 5, 6일에 잡혀있는 상담은 할 수 없다.
- 또한, N+1일째에는 회사에 없기 때문에, 6, 7일에 있는 상담을 할 수 없다.
- 퇴사 전에 할 수 있는 상담의 최대 이익은 1일, 4일, 5일에 있는 상담을 하는 것이며, 이때의 이익은 10+20+15=45이다.
- 상담을 적절히 했을 때, 백준이가 얻을 수 있는 최대 수익을 구하는 프로그램을 작성하시오.
(힌트: 동적계획법 알고리즘을 이용하여 풀 수 있다.)

예시 입력1

- 입력:
  ```
  N = 7
  duration = [3, 5, 1, 1, 2, 4, 2]
  cost = [10, 20, 10, 20, 15, 40, 200]
  ```

- 출력:
  ```
  45
  ```

예시 입력2

- 입력:
```
N = 10
duration = [5, 4, 3, 2, 1, 1, 2, 3, 4, 5]
cost = [50, 40, 30, 20, 10, 10, 20, 30, 40, 50]
```

- 출력:
```
90
```

기반 코드
```python
def solution(N, duration, cost):
    dp = [0]*(N+1)
    
    def dynamic_programming():
        max_val = 0
        for i in range(N-1, -1, -1):
           pass # 코드를 작성하여 함수를 완성하세요.

        return max_val

    result = dynamic_programming()
    return result


N = 7
duration = [3, 5, 1, 1, 2, 4, 2]
cost = [10, 20, 10, 20, 15, 40, 200]
print(solution(N, duration, cost))

N = 10
duration = [5, 4, 3, 2, 1, 1, 2, 3, 4, 5]
cost = [50, 40, 30, 20, 10, 10, 20, 30, 40, 50]
print(solution(N, duration, cost))
```

----

## 과제5. 2020 KAKAO BLIND RECRUITMENT

----
친구들로부터 천재 프로그래머로 불리는 프로도는 음악을 하는 친구로부터 자신이 좋아하는 노래 가사에 사용된 단어들 중에 특정 키워드가 몇 개 포함되어 있는지 궁금하니 프로그램으로 개발해 달라는 제안을 받았습니다.
그 제안 사항 중, 키워드는 와일드카드 문자중 하나인 `'?'`가 포함된 패턴 형태의 문자열을 뜻합니다. 와일드카드 문자인 `'?'`는 글자 하나를 의미하며, 어떤 문자에도 매치된다고 가정합니다. 예를 들어 `"fro??"`는 `"frodo"`, `"front"`, `"frost"` 등에 매치되지만 `"frame"`, `"frozen"`에는 매치되지 않습니다.

가사에 사용된 모든 단어들이 담긴 배열 `words`와 찾고자 하는 키워드가 담긴 배열 `queries`가 주어질 때, 각 키워드 별로 매치된 단어가 몇 개인지 순서대로 배열에 담아 반환하도록 `solution` 함수를 완성해 주세요.

- 가사 단어 제한사항

  - `words`의 길이(가사 단어의 개수)는 2 이상 100,000 이하입니다.
  - 각 가사 단어의 길이는 1 이상 10,000 이하로 빈 문자열인 경우는 없습니다.
  - 전체 가사 단어 길이의 합은 2 이상 1,000,000 이하입니다.
  - 가사에 동일 단어가 여러 번 나올 경우 중복을 제거하고 `words`에는 하나로만 제공됩니다.
  - 각 가사 단어는 오직 알파벳 소문자로만 구성되어 있으며, 특수문자나 숫자는 포함하지 않는 것으로 가정합니다.

- 검색 키워드 제한사항

  - `queries`의 길이(검색 키워드 개수)는 2 이상 100,000 이하입니다.
  - 각 검색 키워드의 길이는 1 이상 10,000 이하로 빈 문자열인 경우는 없습니다.
  - 전체 검색 키워드 길이의 합은 2 이상 1,000,000 이하입니다.
  - 검색 키워드는 중복될 수도 있습니다.
  - 각 검색 키워드는 오직 알파벳 소문자와 와일드카드 문자인 `'?'` 로만 구성되어 있으며, 특수문자나 숫자는 포함하지 않는 것으로 가정합니다.
  - 검색 키워드는 와일드카드 문자인 `'?'`가 하나 이상 포함돼 있으며, `'?'`는 각 검색 키워드의 접두사 아니면 접미사 중 하나로만 주어집니다.
  - 예를 들어 `"??odo"`, `"fro??"`, `"?????"`는 가능한 키워드입니다.
  - 반면에 `"frodo"`(`'?'`가 없음), `"fr?do"`(`'?'`가 중간에 있음), `"?ro??"`(`'?'`가 양쪽에 있음)는 불가능한 키워드입니다.

- 입출력 예

  ```python
  words = ["frodo", "front", "frost", "frozen", "frame", "kakao"]
  queries = ["fro??", "????o", "fr???", "fro???", "pro?"]
  result = [3, 2, 4, 1, 0]
  ```

- 입출력 예에 대한 설명
 
  - `"fro??"`는 `"frodo"`, `"front"`, `"frost"`에 매치되므로 3입니다.
  - `"????o"`는 `"frodo"`, `"kakao"`에 매치되므로 2입니다.
  - `"fr???"`는 `"frodo"`, `"front"`, `"frost"`, `"frame"`에 매치되므로 4입니다.
  - `"fro???"`는 `"frozen"`에 매치되므로 1입니다.
  - `"pro?"`는 매치되는 가사 단어가 없으므로 0 입니다.

```python
def solution(words, queries):
    answer = []
    return answer

words = ["frodo", "front", "frost", "frozen", "frame", "kakao"]
queries = ["fro??", "????o", "fr???", "fro???", "pro?"]
print(solution(words, queries))
```

----


## 과제6. 2020 KAKAO BLIND RECRUITMENT

----

레스토랑을 운영하고 있는 스카피는 레스토랑 내부가 너무 낡아 친구들과 함께 직접 리모델링 하기로 했습니다. 레스토랑이 있는 곳은 스노우타운으로 매우 추운 지역이어서 내부 공사를 하는 도중에 주기적으로 외벽의 상태를 점검해야 할 필요가 있습니다.

레스토랑의 구조는 완전히 동그란 모양이고 외벽의 총 둘레는 n미터이며, 외벽의 몇몇 지점은 추위가 심할 경우 손상될 수도 있는 취약한 지점들이 있습니다. 따라서 내부 공사 도중에도 외벽의 취약 지점들이 손상되지 않았는 지, 주기적으로 친구들을 보내서 점검을 하기로 했습니다. 다만, 빠른 공사 진행을 위해 점검 시간을 1시간으로 제한했습니다. 친구들이 1시간 동안 이동할 수 있는 거리는 제각각이기 때문에, 최소한의 친구들을 투입해 취약 지점을 점검하고 나머지 친구들은 내부 공사를 돕도록 하려고 합니다. 편의 상 레스토랑의 정북 방향 지점을 0으로 나타내며, 취약 지점의 위치는 정북 방향 지점으로부터 시계 방향으로 떨어진 거리로 나타냅니다. 또, 친구들은 출발 지점부터 시계, 혹은 반시계 방향으로 외벽을 따라서만 이동합니다.

외벽의 길이 `n`, 취약 지점의 위치가 담긴 배열 `weak`, 각 친구가 1시간 동안 이동할 수 있는 거리가 담긴 배열 `dist`가 매개변수로 주어질 때, 취약 지점을 점검하기 위해 보내야 하는 친구 수의 최소값을 return 하도록 `solution` 함수를 완성해주세요.

- 제한사항
  - `n`은 1 이상 200 이하인 자연수입니다.
  - `weak`의 길이는 1 이상 15 이하입니다.
  - 서로 다른 두 취약점의 위치가 같은 경우는 주어지지 않습니다.
  - 취약 지점의 위치는 오름차순으로 정렬되어 주어집니다.
  - `weak`의 원소는 0 이상 n - 1 이하인 정수입니다.
  - `dist`의 길이는 1 이상 8 이하입니다.
  - `dist`의 원소는 1 이상 100 이하인 자연수입니다.
  - 친구들을 모두 투입해도 취약 지점을 전부 점검할 수 없는 경우에는 -1을 return 해주세요.


- 입출력 예


  |n | weak | dist | result |
  |--|-----|------|---------|
  |12 |`[1, 5, 6, 10]` |`[1, 2, 3, 4]` |2 |
  |12 |`[1, 3, 4, 9, 10]`|`[3, 5, 7]`|1 |


- 입출력 예에 대한 설명
  - 입출력 예 #1
    - 4m를 이동할 수 있는 친구는 10m 지점에서 출발해 시계방향으로 돌아 1m 위치에 있는 취약 지점에서 외벽 점검을 마칩니다.
    - 2m를 이동할 수 있는 친구는 4.5m 지점에서 출발해 6.5m 지점에서 외벽 점검을 마칩니다.
    - 그 외에 여러 방법들이 있지만, 두 명보다 적은 친구를 투입하는 방법은 없습니다. 따라서 친구를 최소 두 명 투입해야 합니다.

  - 입출력 예 #2
    - 7m를 이동할 수 있는 친구가 4m 지점에서 출발해 반시계 방향으로 점검을 돌면 모든 취약 지점을 점검할 수 있습니다. 따라서 친구를 최소 한 명 투입하면 됩니다.

```python
def solution(n, weak, dist):
    answer = 0
    return answer

n = 12
weak = [1, 5, 6, 10]
dist = [1, 2, 3, 4]
print(solution(n, weak, dist))

n = 12
weak = [1, 3, 4, 9, 10]
dist = [3, 5, 7]
print(solution(n, weak, dist))
```

----


## 과제7. 2019년 LINE 인턴 채용 코딩테스트 문제

----
연인 코니와 브라운은 광활한 들판에서 ‘나 잡아 봐라’ 게임을 한다. 이 게임은 브라운이 코니를 잡거나, 코니가 너무 멀리 달아나면 끝난다. 게임이 끝나는데 걸리는 최소 시간을 구하시오.

- 조건
  - 코니는 처음 위치 C에서 1초 후 1만큼 움직이고, 이후에는 가속이 붙어 매 초마다 이전 이동 거리 + 1만큼 움직인다. 즉 시간에 따른 코니의 위치는 C, C + 1, C + 3, C + 6, …이다.
  - 브라운은 현재 위치 B에서 다음 순간 B – 1, B + 1, 2 * B 중 하나로 움직일 수 있다.
  - 코니와 브라운의 위치 p는 조건 0 <= x <= 200,000을 만족한다.
  - 브라운은 범위를 벗어나는 위치로는 이동할 수 없고, 코니가 범위를 벗어나면 게임이 끝난다.

- 출력 형식
  - 브라운이 코니를 잡을 수 있는 최소시간 N초를 표준 출력한다. 단 브라운이 코니를 잡지 못한 경우에는 -1을 출력한다.

- 예제 입력


  |C|B|출력|
  |-|-|---|
  |11|2|5|

- 예제 설명

  - 코니의 위치: 11 → 12 → 14 → 17 → 21 → 26
  - 브라운의 위치: 2 → 3 → 6 → 12 → 13 → 26
  - 브라운은 코니를 5초 만에 잡을 수 있다.

```python
def solution(C, B):
    result = 0
    return result

print(solution(11, 2))
```

----

## 과제8. 삼성 SW 역량 테스트 유사 문제

----
'Dummy' 라는 도스게임이 있다. 이 게임에는 뱀이 나와서 기어다니는데, 사과를 먹으면 뱀 길이가 늘어난다. 뱀이 이리저리 기어다니다가 벽 또는 자기자신의 몸과 부딪히면 게임이 끝난다.

게임은 NxN 정사각 보드위에서 진행되고, 몇몇 칸에는 사과가 놓여져 있다. 보드의 상하좌우 끝에 벽이 있다. 게임이 시작할때 뱀은 맨위 맨좌측에 위치하고 뱀의 길이는 1 이다. 뱀은 처음에 오른쪽을 향한다.

뱀은 매 초마다 이동을 하는데 다음과 같은 규칙을 따른다.

- 먼저 뱀은 몸길이를 늘려 머리를 다음칸에 위치시킨다.
- 만약 이동한 칸에 사과가 있다면, 그 칸에 있던 사과가 없어지고 꼬리는 움직이지 않는다.
- 만약 이동한 칸에 사과가 없다면, 몸길이를 줄여서 꼬리가 위치한 칸을 비워준다. 즉, 몸길이는 변하지 않는다.
- 사과의 위치와 뱀의 이동경로가 주어질 때 이 게임이 몇 초에 끝나는지 계산하라.

- 입력
  - 보드의 크기 N (2 ≤ N ≤ 100)
  - 사과의 개수 K (0 ≤ K ≤ 100)
  - 뱀의 방향 변환 횟수 L (1 ≤ L ≤ 100)
  - 사과의 위치가 담긴 리스트 apples
    - 첫 번째 정수는 행, 두 번째 정수는 열 위치를 의미한다. 사과의 위치는 모두 다르며, 맨 위 맨 좌측 (1행 1열) 에는 사과가 없다.
  - 뱀의 방향 변환 정보 moves
    - 정수 X와 문자 C로 이루어져 있으며. 게임 시작 시간으로부터 X초가 끝난 뒤에 왼쪽(C가 'L') 또는 오른쪽(C가 'D')로 90도 방향을 회전시킨다는 뜻이다. X는 10,000 이하의 양의 정수이며, 방향 전환 정보는 X가 증가하는 순으로 주어진다.

- 예시입력1
  - 입력
    ```python
    N = 6
    K = 3
    L = 3
    apples = [(3, 4), (2, 5), (5, 3)]
    moves = [(3, 'D'), (15, 'L'), (17, 'D')]
    ```
  - 출력: 9

- 예시입력2
  - 입력
    ```python
    N = 10
    K = 4
    L = 4
    apples = [(1, 2), (1, 3), (1, 4), (1, 5)]
    moves = [(8, 'D'), (10, 'D'), (11, 'D'), (13, 'L')]
    ```
  - 출력: 21
 
- 예시입력3
  - 입력
    ```python
    N = 10
    K = 5
    L = 4
    apples = [(1, 5), (1, 3), (1, 2), (1, 6), (1, 7)]
    moves = [(8, 'D'), (10, 'D'), (11, 'D'), (13, 'L')]
    ```
  - 출력: 13

```python
def solution(N, K, L, apples, moves):
    result = 0
    return result

N = 6
K = 3
L = 3
apples = [(3, 4), (2, 5), (5, 3)]
moves = [(3, 'D'), (15, 'L'), (17, 'D')]
print(solution(N, K, L, apples, moves))

N = 10
K = 4
L = 4
apples = [(1, 2), (1, 3), (1, 4), (1, 5)]
moves = [(8, 'D'), (10, 'D'), (11, 'D'), (13, 'L')]
print(solution(N, K, L, apples, moves))

N = 10
K = 5
L = 4
apples = [(1, 5), (1, 3), (1, 2), (1, 6), (1, 7)]
moves = [(8, 'D'), (10, 'D'), (11, 'D'), (13, 'L')]
print(solution(N, K, L, apples, moves))

```

----

## 과제9. 2020 카카오 인턴십

----
IT 벤처 회사를 운영하고 있는 라이언은 매년 사내 해커톤 대회를 개최하여 우승자에게 상금을 지급하고 있습니다.

이번 대회에서는 우승자에게 지급되는 상금을 이전 대회와는 다르게 다음과 같은 방식으로 결정하려고 합니다.

해커톤 대회에 참가하는 모든 참가자들에게는 숫자들과 3가지의 연산문자(`+`, `-`, `*`) 만으로 이루어진 연산 수식이 전달되며, 참가자의 미션은 전달받은 수식에 포함된 연산자의 우선순위를 자유롭게 재정의하여 만들 수 있는 가장 큰 숫자를 제출하는 것입니다.

단, 연산자의 우선순위를 새로 정의할 때, 같은 순위의 연산자는 없어야 합니다. 즉, `+` > `-` > `*` 또는 `-` > `*` > `+` 등과 같이 연산자 우선순위를 정의할 수 있으나 `+`,`*` > `-` 또는 `*` > `+`,`-`처럼 2개 이상의 연산자가 동일한 순위를 가지도록 연산자 우선순위를 정의할 수는 없습니다. 수식에 포함된 연산자가 2개라면 정의할 수 있는 연산자 우선순위 조합은 2! = 2가지이며, 연산자가 3개라면 3! = 6가지 조합이 가능합니다.

만약 계산된 결과가 음수라면 해당 숫자의 절댓값으로 변환하여 제출하며 제출한 숫자가 가장 큰 참가자를 우승자로 선정하며, 우승자가 제출한 숫자를 우승상금으로 지급하게 됩니다.

예를 들어, 참가자 중 네오가 아래와 같은 수식을 전달받았다고 가정합니다.

```
"100-200*300-500+20"
```

일반적으로 수학 및 전산학에서 약속된 연산자 우선순위에 따르면 더하기와 빼기는 서로 동등하며 곱하기는 더하기, 빼기에 비해 우선순위가 높아 `*` > `+`,`-` 로 우선순위가 정의되어 있습니다.

대회 규칙에 따라 `+` > `-` > `*` 또는 `-` > `*` > `+` 등과 같이 연산자 우선순위를 정의할 수 있으나 `+`,`*` > `-` 또는 `*` > `+`,`-` 처럼 2개 이상의 연산자가 동일한 순위를 가지도록 연산자 우선순위를 정의할 수는 없습니다.

수식에 연산자가 3개 주어졌으므로 가능한 연산자 우선순위 조합은 3! = 6가지이며, 그 중 `+` > `-` > `*` 로 연산자 우선순위를 정한다면 결괏값은 22,000원이 됩니다.

반면에 `*` > `+` > `-` 로 연산자 우선순위를 정한다면 수식의 결괏값은 `-60,420` 이지만, 규칙에 따라 우승 시 상금은 절댓값인 `60,420`원이 됩니다.

참가자에게 주어진 연산 수식이 담긴 문자열 expression이 매개변수로 주어질 때, 우승 시 받을 수 있는 가장 큰 상금 금액을 return 하도록 solution 함수를 완성해주세요.

- 제한사항
  - expression은 길이가 3 이상 100 이하인 문자열입니다.
  - expression은 공백문자, 괄호문자 없이 오로지 숫자와 3가지의 연산자(+, -, \*) 만으로 이루어진 올바른 중위표기법(연산의 두 대상 사이에 연산기호를 사용하는 방식)으로 표현된 연산식입니다. 잘못된 연산식은 입력으로 주어지지 않습니다.
    - 즉, `"402+-561*"`처럼 잘못된 수식은 올바른 중위표기법이 아니므로 주어지지 않습니다.
  - expression의 피연산자(operand)는 0 이상 999 이하의 숫자입니다.
    - 즉, `"100-2145*458+12"`처럼 999를 초과하는 피연산자가 포함된 수식은 입력으로 주어지지 않습니다.
  - `"-56+100"`처럼 피연산자가 음수인 수식도 입력으로 주어지지 않습니다.
  - expression은 적어도 1개 이상의 연산자를 포함하고 있습니다.
  - 연산자 우선순위를 어떻게 적용하더라도, expression의 중간 계산값과 최종 결괏값은 절댓값이 `2^63 - 1` 이하가 되도록 입력이 주어집니다.
  - 같은 연산자끼리는 앞에 있는 것의 우선순위가 더 높습니다.

- 입출력 예

|expression|result|
|----------|------|
|`"100-200*300-500+20"`| 60420|
|`"50*6-3*2"`|300|

- 입출력 예에 대한 설명
  - 입출력 예 #1
    - `*` > `+` > `-` 로 연산자 우선순위를 정했을 때, 가장 큰 절댓값을 얻을 수 있습니다.
    - 연산 순서는 아래와 같습니다.
    
      ```
      100-200*300-500+20
      = 100-(200*300)-500+20
      = 100-60000-(500+20)
      = (100-60000)-520
      = (-59900-520)
      = -60420
      ```
      
    - 따라서, 우승 시 받을 수 있는 상금은 |-60420| = 60420 입니다.

  - 입출력 예 #2
    - `-` > `*` 로 연산자 우선순위를 정했을 때, 가장 큰 절댓값을 얻을 수 있습니다.
    - 연산 순서는 아래와 같습니다.(expression에서 `+` 연산자는 나타나지 않았으므로, 고려할 필요가 없습니다.)
      
      ```
      50*6-3*2
      = 50*(6-3)*2
      = (50*3)*2
      = 150*2
      = 300
      ```
      
    - 따라서, 우승 시 받을 수 있는 상금은 300 입니다.

```python
def solution(expression):
     return 0
    
print(solution("100-200*300-500+20"))
print(solution("50*6-3*2"))
```

----

## 과제10. 2020 카카오 인턴십

----
개발자 출신으로 세계 최고의 갑부가 된 어피치는 스트레스를 받을 때면 이를 풀기 위해 오프라인 매장에 쇼핑을 하러 가곤 합니다.
어피치는 쇼핑을 할 때면 매장 진열대의 특정 범위의 물건들을 모두 싹쓸이 구매하는 습관이 있습니다.
어느 날 스트레스를 풀기 위해 보석 매장에 쇼핑을 하러 간 어피치는 이전처럼 진열대의 특정 범위의 보석을 모두 구매하되 특별히 아래 목적을 달성하고 싶었습니다.

```
진열된 모든 종류의 보석을 적어도 1개 이상 포함하는 가장 짧은 구간을 찾아서 구매
```

예를 들어 아래 진열대는 4종류의 보석(RUBY, DIA, EMERALD, SAPPHIRE) 8개가 진열된 예시입니다.

|진열대 번호|1|2|3|4|5|6|7|8|
|---------|-|-|-|-|-|-|-|-|
|보석 이름|DIA|RUBY|RUBY|DIA|DIA|EMERALD|SAPPHIRE|DIA|

진열대의 3번부터 7번까지 5개의 보석을 구매하면 모든 종류의 보석을 적어도 하나 이상씩 포함하게 됩니다.

진열대의 3, 4, 6, 7번의 보석만 구매하는 것은 중간에 특정 구간(5번)이 빠지게 되므로 어피치의 쇼핑 습관에 맞지 않습니다.

진열대 번호 순서대로 보석들의 이름이 저장된 배열 gems가 매개변수로 주어집니다. 이때 모든 보석을 하나 이상 포함하는 가장 짧은 구간을 찾아서 return 하도록 solution 함수를 완성해주세요.
가장 짧은 구간의 시작 진열대 번호와 끝 진열대 번호를 차례대로 배열에 담아서 return 하도록 하며, 만약 가장 짧은 구간이 여러 개라면 시작 진열대 번호가 가장 작은 구간을 return 합니다.

- 제한사항
  - gems 배열의 크기는 1 이상 100,000 이하입니다.
  - gems 배열의 각 원소는 진열대에 나열된 보석을 나타냅니다.
  - gems 배열에는 1번 진열대부터 진열대 번호 순서대로 보석이름이 차례대로 저장되어 있습니다.
  - gems 배열의 각 원소는 길이가 1 이상 10 이하인 알파벳 대문자로만 구성된 문자열입니다.
  
- 입출력 예

|gems|result|
|----|------|
|["DIA", "RUBY", "RUBY", "DIA", "DIA", "EMERALD", "SAPPHIRE", "DIA"]|[3, 7]|
|["AA", "AB", "AC", "AA", "AC"]|[1, 3]|
|["XYZ", "XYZ", "XYZ"]|[1, 1]|
|["ZZZ", "YYY", "NNNN", "YYY", "BBB"]|[1, 5]|

- 입출력 예에 대한 설명
  - 입출력 예 #1
    - 문제 예시와 같습니다.

  - 입출력 예 #2
    - 3종류의 보석(AA, AB, AC)을 모두 포함하는 가장 짧은 구간은 [1, 3], [2, 4]가 있습니다.
    - 시작 진열대 번호가 더 작은 [1, 3]을 return 해주어야 합니다.

  - 입출력 예 #3
    - 1종류의 보석(XYZ)을 포함하는 가장 짧은 구간은 [1, 1], [2, 2], [3, 3]이 있습니다.
    - 시작 진열대 번호가 가장 작은 [1, 1]을 return 해주어야 합니다.

  - 입출력 예 #4
    - 4종류의 보석(ZZZ, YYY, NNNN, BBB)을 모두 포함하는 구간은 [1, 5]가 유일합니다.
    - 그러므로 [1, 5]를 return 해주어야 합니다.

```python
def solution(gems):
    return []

gems = ["DIA", "RUBY", "RUBY", "DIA", "DIA", "EMERALD", "SAPPHIRE", "DIA"]
print(solution(gems))

gems = ["AA", "AB", "AC", "AA", "AC"]
print(solution(gems))

gems = ["XYZ", "XYZ", "XYZ"]
print(solution(gems))

gems = ["ZZZ", "YYY", "NNNN", "YYY", "BBB"]
print(solution(gems))
```

----
