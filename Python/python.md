# Python

## π‘ μΈλ΄νΈ

νμ΄μ¬μ λνμ μΈ νΉμ§μ΄κΈ°λ ν μΈλ΄νΈ(λ€μ¬μ°κΈ°)λ PEP 8μ λ°λΌ κ³΅λ°±4μΉΈμ μμΉμΌλ‘ νλ€.

> PEP
> <br>
> PEP(Python Enhancement Proposals) νμ΄μ¬ κ°μ  μ μμ

κ³΅λ°± 4μΉΈμ΄ κ°μ λ μλλΌ μ νμ μΌλ‘ μ μ©ν  μ μμ§λ§ PEP 8 μ΄νμλ 4μΉΈμ μ€μνλ€.

<br><br>

## π‘ λ€μ΄λ° μ»¨λ²€μ

νμ΄μ¬μ λ³μλͺ λ€μ΄λ° μ»¨λ²€μμ μ€λ€μ΄ν¬ μΌμ΄μ€λ₯Ό λ°λ₯Έλ€. νμ΄μ¬μ μΉ΄λ© μΌμ΄μ€λ‘ μ½λ©νλ κ²μ μ§μνλ€.

<br>

> ### μ€λ€μ΄ν¬ μΌμ΄μ€, μΉ΄λ© μΌμ΄μ€
>
> μ€λ€μ΄ν¬ μΌμ΄μ€λ λ±κ³Ό κ°μ λͺ¨μμμ μ λνμΌλ©° κ° λ¨μ΄λ₯Ό μΈλμ€μ½μ΄(\_)λ‘ κ΅¬λΆνλ€.
> #snake_case : int = 1
> <br><br>
> μΉ΄λ© μΌμ΄μ€λ λν(Camel)μ²λΌ μκΈ΄ κ²μ μ λν΄ λΆλ₯Έ μ΄λ¦μ΄λ©° λ¨μ΄λ₯Ό λμλ¬Έμ κ΅¬λΆνμ¬ μμ΄μ μλͺνλ λ°©μμ΄λ€. μλ°μ λνμ μΈ νκΈ°λ°©μμ΄λ€.
> #camelCase: int = 1

<br>

## π‘ ν¨μ

λκ°μ λ΄μ©μ λ°λ³΅ν΄μ μμ±ν΄μΌν  λ ν¨μκ° νμνλ€.

### ν¨μ κ΅¬μ‘°

```
def ν¨μλͺ(λ§€κ°λ³μ):
    <μνν  λ¬Έμ₯>
```

defλ ν¨μλ₯Ό λ§λ€ λ μ¬μ©νλ μμ½μ΄μ΄λ©°, ν¨μ μ΄λ¦μ ν¨μλ₯Ό λ§λλ μ¬λμ΄ μμλ‘ λ§λ€ μ μλ€. ν¨μ μ΄λ¦ λ€ κ΄νΈ μμ λ§€κ°λ³μλ μ΄ ν¨μμ μλ ₯μΌλ‘ μ λ¬λλ κ°μ λ°λ λ³μμ΄λ€.

```
def add(a, b):
    return a+b
```

μλ ₯μΌλ‘ a,b λκ°λ₯Ό μλ ₯λ°μΌλ©΄ λκ°λ₯Ό λν΄μ£Όλ ν¨μμ΄λ€.
returnμ ν¨μμ κ²°κ³Όκ°μ λλ €μ£Όλ λͺλ Ήμ΄μ΄λ€.

<br>

### λ§€κ°λ³μμ μΈμ

λ§€κ°λ³μ(parameter)μ μΈμ(arguments)λ νΌμ©ν΄μ μ¬μ©λλ ν·κ°λ¦¬λ μ©μ΄μ΄λ€.

> λ§€κ°λ³μλ ν¨μμ μλ ₯μΌλ‘ μ λ¬λ κ°μ λ°λ λ³μλ₯Ό μλ―Ένκ³  μΈμλ ν¨μλ₯Ό νΈμΆν  λ μ λ¬νλ μλ ₯κ°μ μλ―Ένλ€.

```
def add(a, b): # a, bλ λ§€κ°λ³μ
    return a+b

print(add(1, 2)) # 1, 2λ μΈμ
```

<br>

## π‘ lambda

lambdaλ ν¨μλ₯Ό μμ±ν  λ μ¬μ©νλ μμ½μ΄λ‘ defμ λμΌν μ­ν μ νλ€. λ³΄ν΅ ν¨μλ₯Ό νμ€λ‘ κ°κ²°νκ² λ§λ€ λ μ¬μ©νλ€. μ°λ¦¬λ§λ‘λ "λλ€"λΌκ³  μ½λλ€.

<br>

### lambda κ΅¬μ‘°

```
lambda λ§€κ°λ³μ : ννμ
```

```
def add(a, b):
    return a+b
```

λ μλ₯Ό λνλ ν¨μλ₯Ό lambda νμμΌλ‘ νν

```
(lambda a,b: a + b)(1, 2)
-> 3
```

<br>

## π‘ ν΄λμ€

<br>

ν΄λμ€λ λκ°μ λ¬΄μμΈκ°λ₯Ό κ³μν΄μ λ§λ€μ΄ λΌ μ μλκ²μ΄κ³ , κ°μ²΄λ ν΄λμ€λ‘ λ§λ€μ΄μ§ κ²μ μλ―Ένλ€.<br>
ν΄λμ€λ‘ λ§λ  κ°μ²΄λ κ°μ²΄λ§λ€ κ³ μ ν μ±κ²©μ κ°μ§λ€. μ¦ λμΌν ν΄λμ€λ‘ λ§λ  κ°μ²΄λ€μ μλ‘ μ ν μν₯μ μ£Όμ§ μλλ€.

<br>

### ν΄λμ€ κ΅¬μ‘°

```
class name:
    pass
```

μλ¬΄ κΈ°λ₯λ κ°κ³  μμ§ μλ ν΄λμ€μ΄λ€.
κ°μ²΄λ ν΄λμ€λ‘ λ§λ€λ©° 1κ°μ ν΄λμ€λ‘λ λ§μ κ°μ²΄λ₯Ό λ§λ€ μ μλ€.
μμ name ν΄λμ€λ‘ κ°μ²΄λ₯Ό λ§λλ λ°©λ²μ΄λ€.

```
a = name()
```

name()μ κ²°κ³Όκ°μ λ°μ aκ° κ°μ²΄μ΄λ€.

<br>

### κ°μ²΄μ μ«μ μ§μ ν  μ μκ² νκΈ°

```
class FourCal:
    def setdata(self, first, second):
        self.first = first
        self.second = second
```

FourCal ν΄λμ€ μμ setdataλΌλ ν¨μλ₯Ό λ§λ€μλ€.
ν΄λμ€ μμ κ΅¬νλ ν¨μλ λ©μλ(Method)λΌκ³  λΆλ₯Έλ€.

<br>

#### setdata λ©μλμ λ§€κ°λ³μ

setdata λ©μλλ λ§€κ°λ³μλ‘ self,first,second 3κ° μλ ₯κ°μ λ°λλ€. μ²«λ²μ§Έ λ§€κ°λ³μμΈ selfμλ setdataλ©μλλ₯Ό νΈμΆν κ°μ²΄κ° μλμΌλ‘ μ λ¬λλ€.

```
a = FourCal()
a.setdata(4, 2)
```

aκ° selfμ μ λ¬λκ³  4λ first, 2sms secondμ μ λ¬λλ€.

μ¦ self.first = 4, self.second = 2μ΄κ³ 
selfλ μ λ¬λ κ°μ²΄ aμ΄λ―λ‘ a.first = 4, a.second = 2λ‘ ν΄μμ΄λλ€.

```
a = FourCal()
a.setdata(4, 2)
print(a.first)
-> 4
print(a.second)
-> 2
```

### λνκΈ° κΈ°λ₯μ κ°μ§ ν΄λμ€

```
class FourCal():
    def setdata(self, first, second):
        self.first = first
        self.second = second
    def add(self):
        result = self.first + self.second
        return result
```

FourCal ν΄λμ€μ addλ©μλλ₯Ό μΆκ°νλ€.

```
a = FourCal()
a.setdata(4, 2)

print(a.add())
-> 6
```

a κ°μ²΄μ first, secondμ 4 μ 2κ° μ μ₯λκ³  addλ©μλλ₯Ό νΈμΆνμ¬ 6μ΄ λμλ€.

a.add()μ κ°μ΄ a κ°μ²΄μ μν΄ addλ©μλκ° μνλμ΄ add λ©μλμ selfμλ κ°μ²΄ aκ° μλμΌλ‘ μ λ¬λλ€.

```
result = a.first + a.second
```

κ·Έλμ result = 4 + 2κ° λλ€.

<br>

## π‘ ν΄λμ€μ μμ

μμμ΄λ "λ¬Όλ €λ°λ€"λΌλ λ»μΌλ‘ μ΄λ€ ν΄λμ€κ° λ€λ₯Έ ν΄λμ€μ μ±μ§(κΈ°λ₯)μ λ¬Όλ €λ°λ κ²μ λ§νλ€.

μ΄λ€ ν΄λμ€λ₯΄ λ§λ€ λ μ²μλΆν° μλ‘ λ§λ€ νμ μμ΄, ν΅μ¬μ μΈ μ±μ§μ κ°κ³  μλ λ€λ₯Έ ν΄λμ€λ‘λΆν° μμμ λ°μμ ν΄λμ€λ₯Ό λ§λ€ μ μλ€.

```
class MoreFourCal(FourCal)
    pass
```

<br>

μμ MoreFourCal ν΄λμ€λ FourCal ν΄λμ€λ₯Ό μμλ°μμ΅λλ€.
MoreFourCal ν΄λμ€λ FourCal ν΄λμ€λ₯Ό μμνμΌλ―λ‘ FourCal ν΄λμ€μ λͺ¨λ  κΈ°λ₯μ μ¬μ©ν  μ μμ΄μΌ νλ€.

<br>

```
a = MoreFourCal(4, 2)
a.add()
-> 6
```

μμλ°μ FourCal ν΄λμ€μ κΈ°λ₯μ λͺ¨λ μ¬μ©ν  μ μλ€.

<br>

## π‘ μμ±μ

<br>
μμ±μλ κ°μ²΄κ° μμ±λ  λ μλμΌλ‘ νΈμΆλλ λ©μλλ₯Ό μλ―Ένλ€. νμ΄μ¬ λ©μλ μ΄λ¦μΌλ‘ __init__λ₯Ό μ¬μ©νλ©΄ μ΄ λ©μλλ μμ±μκ° λλ€.

```
def __init__(self, first, second):
    self.first = first
    self.second = second
```

λ©μλ μ΄λ¦μ **init**μΌλ‘ νκΈ° λλ¬Έμ κ°μ²΄κ° μμ±λλ μμ μμ μλμΌλ‘ νΈμΆμ΄ λλ€.

<br>

```
a = FourCal(4, 2)
```

μμ κ°μ΄ μ€ννλ©΄ **init**λ©μλκ° μλμΌλ‘ νΈμΆμ΄λμ self = a, firts = 4, second = 2κ° μ λ¬λλ€.

<br>

## π‘ μμΈ μ²λ¦¬

### try, exceptλ¬Έ

<br>

try λΈλ‘ λΆλΆμ μν μ€ μ€λ₯κ° λ°μνλ©΄ except λΆλΆμ΄ μ€νλλ€.

```
try:
    ...
except:
    ...
```

μ΄ κ²½μ°λ μ€λ₯ μ’λ₯μ μκ΄μμ΄ μ€λ₯κ° λ°μνλ©΄ exceptκ° μ€νλλ€.

```
try:
    ...
except λ°μ μ€λ₯:
    ...
```

μ΄ κ²½μ°λ μ€λ₯κ° λ°μνμ λ exceptλ¬Έμ λ―Έλ¦¬ μ ν΄ λμ μ€λ₯ μ΄λ¦κ³Ό μΌμΉν  λλ§ except λΈλ‘μ μννλ€λ λ»μ΄λ€.

<br>

## π‘ μ κ· ννμ

μ κ· ννμ(Regular Expressions)μ λ³΅μ‘ν λ¬Έμμ΄μ μ²λ¦¬ν  λ μ¬μ©νλ κΈ°λ²μ΄λ€.

### μ κ· ννμμ λ©ν λ¬Έμ

<br>

> λ©ν λ¬Έμλ μλ κ·Έ λ¬Έμκ° κ°μ§ λ»μ΄ μλ νΉλ³ν μ©λλ‘ μ¬μ©νλ λ¬Έμλ₯Ό λ§νλ€.

```
. ^ $ * + ? { } [ ] \ | ( )
```

μ κ· ννμμμ μ¬μ©νλ λ©ν λ¬Έμ

<br>

### λ¬Έμ ν΄λμ€ [ ]

λ¬Έμ ν΄λμ€λ‘ λ§λ€μ΄μ§ μ κ·μμ [ ] μ¬μ΄μ λ¬Έμλ€κ³Ό λ§€μΉ λΌλ μλ―Έλ₯Ό κ°λλ€.

μ¦ μ κ· ννμμ΄ [abc]λΌλ©΄ μ΄ ννμμ μλ―Έλ "a, b, c μ€ ν κ°μ λ¬Έμμ λ§€μΉ"λ₯Ό λ»νλ€.

[ ] μμ λ λ¬Έμ μ¬μ΄μ νμ΄ν(-)μ μ¬μ©νλ©΄ λ λ¬Έμ μ¬μ΄μ λ²μ(From - To)λ₯Ό μλ―Ένλ€. μλ₯Ό λ€μ΄ [a-c]λΌλ μ κ· ννμμ [abc]μ λμΌνκ³  [0-5]λ [012345]μ λμΌνλ€.

> [a-zA-Z] : μνλ²³ λͺ¨λ
> <br>[0-9] : μ«μ

λ¬Έμ ν΄λμ€ μμ ^ λ©ν λ¬Έμλ₯Ό μ¬μ©νλ©΄ notμ μλ―Έλ₯Ό κ°λλ€. [^0-9]λ μ«μκ° μλ λ¬Έμλ§ λ§€μΉλλ€.

<br>

### μμ£Ό μ¬μ©νλ λ¬Έμ ν΄λμ€<br>

> \d : μ«μ [0-9]μ κ°λ€.<br>
> \D : λΉμ«μ [^0-9]μ κ°λ€.<br>
> \w : μ«μ + λ¬Έμ [a-zA-Z0-9]μ κ°λ€.<br>
> \W : μ«μ + λ¬Έμκ° μλ κ² [^a-za-z0-9]μ κ°λ€.<br>
> \s : κ³΅λ°± [ \t\n\r\f\v]μ κ°λ€.<br>
> \S : λΉκ³΅λ°± [^ \t\n\r\f\v]μ κ°λ€.<br>
> \b : λ¨μ΄ κ²½κ³ (`\w`μ `\W`μ κ²½κ³)<br>
> \B : λΉλ¨μ΄ κ²½κ³
