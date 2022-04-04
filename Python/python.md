# Python

## 💡 인덴트

파이썬의 대표적인 특징이기도 한 인덴트(들여쓰기)는 PEP 8에 따라 공백4칸을 원칙으로 한다.

> PEP
> <br>
> PEP(Python Enhancement Proposals) 파이썬 개선 제안서

공백 4칸이 강제는 아니라 선택적으로 적용할 수 있지만 PEP 8 이후에는 4칸을 준수한다.

<br><br>

## 💡 네이밍 컨벤션

파이썬의 변수명 네이밍 컨벤션은 스네이크 케이스를 따른다. 파이썬은 카멜 케이스로 코딩하는 것을 지양한다.

<br>

> ### 스네이크 케이스, 카멜 케이스
>
> 스네이크 케이스는 뱀과 같은 모양에서 유래했으며 각 단어를 언더스코어(\_)로 구분한다.
> #snake_case : int = 1
> <br><br>
> 카멜 케이스는 낙타(Camel)처럼 생긴 것에 유래해 부른 이름이며 단어를 대소문자 구분하여 섞어서 작명한는 방식이다. 자바의 대표적인 표기방식이다.
> #camelCase: int = 1

<br>

## 💡 함수

똑같은 내용을 반복해서 작성해야할 때 함수가 필요하다.

### 함수 구조

```
def 함수명(매개변수):
    <수행할 문장>
```

def는 함수를 만들 때 사용하는 예약어이며, 함수 이름은 함수를 만드는 사람이 임의로 만들 수 있다. 함수 이름 뒤 괄호 안의 매개변수는 이 함수에 입력으로 전달되는 값을 받는 변수이다.

```
def add(a, b):
    return a+b
```

입력으로 a,b 두개를 입력받으면 두개를 더해주는 함수이다.
return은 함수의 결과값을 돌려주는 명령어이다.

<br>

### 매개변수와 인수

매개변수(parameter)와 인수(arguments)는 혼용해서 사용되는 헷갈리는 용어이다.

> 매개변수는 함수에 입력으로 전달된 값을 받는 변수를 의미하고 인수는 함수를 호출할 때 전달하는 입력값을 의미한다.

```
def add(a, b): # a, b는 매개변수
    return a+b

print(add(1, 2)) # 1, 2는 인수
```

<br>

## 💡 lambda

lambda는 함수를 생성할 때 사용하는 예약어로 def와 동일한 역할을 한다. 보통 함수를 한줄로 간결하게 만들 때 사용한다. 우리말로는 "람다"라고 읽는다.

<br>

### lambda 구조

```
lambda 매개변수 : 표현식
```

```
def add(a, b):
    return a+b
```

두 수를 더하는 함수를 lambda 형식으로 표현

```
(lambda a,b: a + b)(1, 2)
-> 3
```

<br>

## 💡 클래스

<br>

클래스란 똑같은 무엇인가를 계속해서 만들어 낼 수 있는것이고, 객체란 클래스로 만들어진 것을 의미한다.<br>
클래스로 만든 객체는 객체마다 고유한 성격을 가진다. 즉 동일한 클래스로 만든 객체들은 서로 전혀 영향을 주지 않는다.

<br>

### 클래스 구조

```
class name:
    pass
```

아무 기능도 갖고 있지 않는 클래스이다.
객체는 클래스로 만들며 1개의 클래스로도 많은 객체를 만들 수 있다.
위의 name 클래스로 객체를 만드는 방법이다.

```
a = name()
```

name()의 결과값을 받은 a가 객체이다.

<br>

### 객체에 숫자 지정할 수 있게 하기

```
class FourCal:
    def setdata(self, first, second):
        self.first = first
        self.second = second
```

FourCal 클래스 안에 setdata라는 함수를 만들었다.
클래스 안에 구현된 함수는 메서드(Method)라고 부른다.

<br>

#### setdata 메서드의 매개변수

setdata 메서드는 매개변수로 self,first,second 3개 입력값을 받는다. 첫번째 매개변수인 self에는 setdata메서드를 호출한 객체가 자동으로 전달된다.

```
a = FourCal()
a.setdata(4, 2)
```

a가 self에 전달되고 4는 first, 2sms second에 전달된다.

즉 self.first = 4, self.second = 2이고
self는 전달된 객체 a이므로 a.first = 4, a.second = 2로 해석이된다.

```
a = FourCal()
a.setdata(4, 2)
print(a.first)
-> 4
print(a.second)
-> 2
```

### 더하기 기능을 가진 클래스

```
class FourCal():
    def setdata(self, first, second):
        self.first = first
        self.second = second
    def add(self):
        result = self.first + self.second
        return result
```

FourCal 클래스에 add메서드를 추가했다.

```
a = FourCal()
a.setdata(4, 2)

print(a.add())
-> 6
```

a 객체의 first, second에 4 와 2가 저장되고 add메서드를 호출하여 6이 나왔다.

a.add()와 같이 a 객체에 의해 add메서드가 수행되어 add 메서드의 self에는 객체 a가 자동으로 전달된다.

```
result = a.first + a.second
```

그래서 result = 4 + 2가 된다.

<br>

## 💡 생성자

<br>
생성자란 객체가 생성될 때 자동으로 호출되는 메서드를 의미한다. 파이썬 메서드 이름으로 __init__를 사용하면 이 메서드는 생성자가 된다.

```
def __init__(self, first, second):
    self.first = first
    self.second = second
```

메서드 이름을 **init**으로 했기 때문에 객체가 생성되는 시점에서 자동으로 호출이 된다.

<br>

```
a = FourCal(4, 2)
```

위와 같이 실행하면 **init**메서드가 자동으로 호출이되서 self = a, firts = 4, second = 2가 전달된다.
