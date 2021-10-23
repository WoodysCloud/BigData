# 10. 19. 21

<hr />

## 제어문



### 1. if문

`if / else`

`if / elif / else`







### 2. while문

`while [condition]:`

```python
treeHit = 0
while treeHit < 10:
    treeHit += 1
    print("나무를 %d번 찍었습니다." %treeHit)
    if treeHit == 10:
        print("나무 넘어갑니다.")
```



`break`

```python
coffee = 10
money = 300
while money:
    print("돈을 받았으니 커피를 줍니다.")
    coffee -= 1
    print("남은 커피의 양이 %d개입니다.\n" %coffee)
    if coffee == 0:
        print("커피가 다 떨어졌습니다. 판매를 중지합니다.")
        break
```



`continue`

```python
a = 0
while a < 10:
    a = a + 1
    if a % 2 == 0: continue
    print(a)
```





### 3. for문

`for (variable) in (list/tuple/string)`

```python
test_list = ['one', 'two', 'three']
for i in test_list:
    print(i)
```



`range(start, end)`

![Screen Shot 2021-10-19 at 10.16.06 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2010.16.06%20AM.png)



구구단

![Screen Shot 2021-10-19 at 10.17.57 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2010.17.57%20AM.png)



list comprehension

![Screen Shot 2021-10-19 at 10.22.08 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2010.22.08%20AM.png)



<hr />

<br />



## 함수

### 1. 함수

`def`: 함수를 만들 때 사용하는 "예약어"

```python
def function_name(parameters):
  result = parameters + parameters
  return result
```

```python
def add(a, b): # a, b: parameters(매개변수)
  return a + b

print(add(3, 4)) # 3, 4: arguments(인수)
```

```python
def say():
    return "Hi"

a = say()
print(a)

# Hi
```

```python
def say_myself(name, old, man=True):
    print("나의 이름은 %s입니다." %name)
    print("나이는 %d살입니다." %old)
    if man:
        print("남자입니다.")
    else:
        print("여자입니다.")
        
say_myself("송우제", 26)

# 나의 이름은 송우제입니다.
# 나이는 26살입니다.
# 남자입니다.
```



`lambda`: `def` 와 동일한 역할

```python
add = lambda a, b: a+b
result = add(3, 4)
print(result)

# 7
```





### 2. 사용자 입력과 출력

`input()`





### 3. 파일 읽고 쓰기

![Screen Shot 2021-10-19 at 11.38.24 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2011.38.24%20AM.png)

![Screen Shot 2021-10-19 at 11.38.44 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2011.38.44%20AM.png)

![Screen Shot 2021-10-19 at 11.38.53 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2011.38.53%20AM.png)

![Screen Shot 2021-10-19 at 11.39.04 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2011.39.04%20AM.png)

![Screen Shot 2021-10-19 at 11.39.10 AM](/Users/Woody/Desktop/bigdata_github/screenshots/Screen%20Shot%202021-10-19%20at%2011.39.10%20AM.png)





## 파이썬 날개 달기

### 1. 클래스

클래스로 만든 객체의 특징

- 객체마다 고유한 성격을 가짐
- 동일한 클래스로 만든 객체들은 서로 전혀 영향을 주지 않음



### 2. 모듈

.py 확장자로 다운받아서 import

`from module_name import module_function`



### 3. 패키지

도트(.)를 사용하여 파이썬 모듈을 계층적으로 관리 가능

- ex) 모듈 이름이 A.B인 경우에 A는 패키지 이름, B는 A 패키지의 모듈



### 4. 





