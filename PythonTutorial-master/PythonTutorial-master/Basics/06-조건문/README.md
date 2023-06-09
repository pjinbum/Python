# 6강 조건문
이번 시간에는 파이썬의 조건문에 대해서 알아봐요.

## 비교 연산자
이전 강의에서 사칙 연산자를 배웠다면, 이번 강의에서는 **비교 연산자**를 다뤄보도록 해요.

비교 연산자란, 두 데이터를 비교해서 이 비교의 결과가 **참인지 거짓인지**를 판단하는 연산자에요.
비교 연산자는 언제나 bool 타입의 값 (True 혹은 False) 를 반환해줘요.

### 1. 항등 연산자 `==`, `!=`
`==` 연산자는 두 데이터가 같은지 비교해줘요.
```python
print(5 == 5, 5 == 1, "5" == 5)
```
위 코드의 실행 결과에요 :
```css
True False False
```
`!=` 연산자는 두 데이터가 다른지 비교해줘요.
```python
print(5 != 3, 3 != 3, "5" != 5)
```
위 코드의 실행 결과에요 :
```css
True False True
```
### 2. 대소 비교 연산자 `>`, `<`, `>=`, `<=`
- `>` 연산자는 왼쪽의 데이터가 오른쪽의 데이터보다 큰지 (초과)
- `<` 연산자는 왼쪽의 데이터가 오른쪽의 데이터보다 작은지 (미만)
- `>=` 연산자는 왼쪽의 데이터가 오른쪽의 데이터보다 같거나 큰지 (이상)
- `<=` 연산자는 왼쪽의 데이터가 오른쪽의 데이터보다 같거나 작은지 (이하) 비교해줘요.
```python
print(5 > 3, 3 >= 3)
print(5 < 3, 3 <= 3)
```
위 코드의 실행 결과에요 :
```css
True True
False True
```

### 3. 포함 여부 연산자 `in`
`in` 연산자는 아래와 같이 사용해요.
```python
if 'a' in "abc":
    print("a는 abc 안에 있습니다!")
```
위 코드의 실행 결과에요 :
```css
a는 abc 안에 있습니다!
```
in 연산자는 iterable 한 객체(list, tuple, dict, str 등) 안에 주어진 값이 포함되어있는지 확인해줘요.

위 예제에서는 a라는 문자열은 abc라는 문자열 안에 포함되어 있기 때문에, if문의 조건이 True가 되죠.

### 4. 부정 연산자 `not`
`not` 연산자는 아래와 같이 사용해요.
```python
if not True:
    print("if문의 조건이 True입니다!")
```
위 코드의 실행 결과에요 :
```css

```
분명 if문의 조건에는 True가 있는데, if문이 실행되지 않았어요. 이는 not 연산자가 주어진 조건을 부정했기 때문이에요.

not 연산자는 자신의 뒤에 오는 조건의 값을 부정해요. 뒤에 오는 조건이 True이면 False로, False이면 True로 만들어 준답니다.

---
## 코드 블럭
조건문을 배우기 이전에, 앞으로 배우게 될 파이썬의 문법들에는 **코드 블럭**이 등장해요.
코드 블럭이란, 이 구문이 영향을 끼치는 코드의 범위를 말해요. 파이썬에서는 들여쓰기를 통해 각각의 코드 블럭을 구분해줘요.

## 조건문은 무엇일까?
프로그래밍 언어에서 **조건문**은 특정 코드를 조건을 만족하는 상황에서만 실행하도록 하는, 코드의 흐름을 제어하는 장치에요.

파이썬에서 조건문은 **`if`**, **`elif`**, **`else`** 라는 키워드를 통해 사용한답니다. 

### 1. if
if는 가장 기본적인 조건 키워드로, if 키워드 뒤에 오는 조건이 참(True) 일 때 if문 내부의 코드를 실행해요.

이때, if문은 고유의 코드 블럭 (들여쓰기로 구분되는 코드) 을 가지므로, if문 내부의 코드는 if 키워드보다 들여써야 해요.

### 2. elif
elif는 if문 뒤에 이어지는 조건문으로, 앞선 if 혹은 elif문의 조건이 False일 때 자신의 조건을 확인한 후 True 일때 실행해요.

elif문은 고유의 코드 블럭 (들여쓰기로 구분되는 코드) 을 가지므로, elif문 내부의 코드는 elif 키워드보다 들여써야 해요.

### 3. else
else문은 연결된 모든 if문과 elif문의 조건이 모두 False여서 실행되지 않았을 때, 마지막으로 실행되는 구문이에요.
별도의 실행 조건은 따로 가지지 않아요.

else문은 고유의 코드 블럭을 가지므로, else문 내부의 코드는 else 키워드보다 들여써야 해요.

```python
answer = input("원하는 조건문을 입력하세요 : ")

if answer == "if":
    # if문 등 : 로 끝나는 구문 내부에서 실행될 코드는, 들여써야 합니다.
    print("if문을 실행합니다.")
elif answer == "elif1":
    # elif문은 앞선 if문이 거짓일 때 이어서 진행되는 if문으로,
    print("첫 번째 elif문을 실행합니다.")
elif answer == "elif2":
    # elif문은 여러개 사용할 수 있습니다.
    print("두 번째 elif문을 실행합니다.")
else:
    # else문은 앞선 if, elif문이 모두 거짓일 때 실행되는 마지막 조건문입니다.
    print("else문을 실행합니다.")
```

위 코드의 실행 결과는 아래와 같아요 :
```css
원하는 조건문을 입력하세요 : if
if문을 실행합니다.
```
```css
원하는 조건문을 입력하세요 : elif1
첫 번째 elif문을 실행합니다.
```
```css
원하는 조건문을 입력하세요 : elif2
두 번째 elif문을 실행합니다.
```
```css
원하는 조건문을 입력하세요 : else
else문을 실행합니다.
```

### 4. and 연산자
and 연산자는 연결된 두개의 조건이 모두 True일 때 True를 반환해요.
```python
answer = input("영단어를 입력하세요 > ")
if 'a' in answer and 'e' in answer:
    print("입력받은 영단어에는 a와 e가 모두 포함됩니다!")
else:
    print("입력받은 영단어에는 a와 e가 모두 포함되는것은 아닙니다...")
```

### 5. or 연산자
or 연산자는 연결된 두개의 조건중 하나라도 True이면 True를 반환해요.
```python
answer = input("영단어를 입력하세요 > ")
if 'a' in answer or 'e' in answer:
    print("입력받은 영단어에는 a 또는 e가 포함됩니다!")
else:
    print("입력받은 영단어에는 a와 e가 모두 포함되지 않습니다...")
```

***

[예제 코드 보기](./condition.py)

[<- 이전 강좌](../05-타입%20변환과%20묶음%20타입들/README.md) /
[다음 강좌 ->](../07-반복문/README.md)