# Google It!
프로그래밍을 하다 보면 오류가 발생하거나, 모르는 정보를 찾아보고 싶을 때가 종종 생깁니다.
이럴 때, 구글의 힘을 빌려보면 어떨까요?

## 1. 왜 구글인가?
사실, 다른 검색엔진도 상관이 없긴 하지만, 많은 프로그래머들이 `구글링 해라` 라고 말하는 데에는 다 이유가 있는 법이죠.
일단, 초록창으로 유명한 네이버를 쓰지 않는 이유부터 알아봅시다.
프로그래밍 관련 정보들은 영어권 자료들에 좋은 정보들이 많습니다.
그러나, 네이버 검색엔진은 기본적으로 네이버 블로그, 카페 등의 글들을 우선적으로 보여줍니다.
그 결과, 우리가 정말 필요로 하는 영어권 자료들은 네이버의 자료에 묻혀 찾기 어려워 찾기 어려워집니다.
이외에도 bing, 다음 등 여러 검색엔진이 있지만, 가장 대중적이고 간결한 만큼 구글이 자주 쓰입니다.

## 2. 왜 영어를 써야 하는가?
영어로 된 긴 글들을 읽는건, 영어가 모국어가 아닌 사람들에게는 대체로 고된 일일지도 모릅니다.
그러나, 슬프게도 프로그래밍 자료들 중에는 한글로 된 자료들이 많지 않습니다.
원하는 정보를 보다 빨리 찾기 위해서, 그리고 더 질 좋은 강좌를 찾기 위해서는 영어로 자료를 찾아보는 편이 더 좋습니다.

## 3. 어떻게 구글에서 정보를 찾아야 하는가?
찾고자 하는 정보의 키워드만 적어도, 충분히 원하는 정보를 얻어낼 수 있습니다.
예를 들어, 파이썬의 함수에 대해서 알아보고자 한다면 다음과 같은 검색어를 쓸 수 있습니다 : 
[python function](https://www.google.com/search?q=python+function) (눌러서 검색해보세요!)
![검색 결과 이미지](./google_python_function.png)

만약 작성 중인 코드에서 오류가 발생한다고요? 구글링을 통해 오류를 해결해봅시다.
예를 들어, 아래와 같은 코드를 작성했다고 해보죠.
```python
a = 'Hello'
print(int(a))
```
위 코드를 실행하면, 아래와 같은 오류가 발생합니다.
```
Traceback (most recent call last):
  File "D:/Study/Python/영훈고 파이썬 강좌/Projects/01-기본기_복습/project01_369_hard.py", line 66, in <module>
    print(int(a))
ValueError: invalid literal for int() with base 10: 'Hello'
```

우선, 이 오류의 내용을 하나씩 분석해봅시다.
```
File "D:/Study/Python/영훈고 파이썬 강좌/Projects/01-기본기_복습/project01_369_hard.py", line 66, in <module>
```
이 부분은 오류가 발생한 파일과 줄 번호를 알려주는 부분입니다. 오류를 해결하기 위해 고쳐야 할 코드의 위치를 찾기 위해서는 이 정보를 참고하면 됩니다.

```
ValueError: invalid literal for int() with base 10: 'Hello'
```
이게 우리의 코드에서 발생한 오류의 내용입니다.
이 오류를 해결하는 방법을 구글에서 찾는 방법은 간단합니다. 이 오류 내용을 그대로 구글의 검색창에다가 붙여넣고 검색해보죠!

[ValueError: invalid literal for int() with base 10: 'Hello](https://www.google.com/search?q=ValueError:+invalid+literal+for+int()+with+base+10:+'Hello') (눌러서 검색해보세요!)
어때요, 바로 수많은 자료들이 이 오류의 해결법을 알려주고 있네요.
![검색 결과 이미지](./google_valueerror.png)
이렇게 찾은 자료들을 읽고, 오류를 고치면 됩니다.

구글링은 이처럼 간단한 방법으로, 원하는 정보를 찾을 수 있는 프로그래머들의 최강의 무기 중 하나입니다.
모르는 내용이 있다면, 두려워하지 마세요! 구글을 키고, 알고자 하는 내용을 찾아보세요. 스스로 찾아보고 탐구하는 과정을 통해, 더 많은 정보를 스스로 배우게 되고 성장하게 됩니다 :D