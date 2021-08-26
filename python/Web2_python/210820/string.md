## string

#### 'print'는 ()안의 값을 출력하는 함수이다.
---
```
{
print('Hello world')
print("Hello world")
print("Hell'o' world")
}
```
###### *따옴표는 어느 것을 사용하든지 상관은 없으나, 출력하는 값에 따옴표를 넣고 싶을 경우에는 각각 다른 따옴표를 구별하여 사용한다.*

---
[escape]
```
{
print("Hell'o' \"w\"orld")
}
```
###### *\는 \바로 다음에 나오는 명령어를 문자로 취급한다.*

---
[newline]
```
{
print('H')
print('e')
print('l')
print('l')
print('o')
print('H\ne\nl\nl\no')
}
```
###### *하나의 단어를 각각의 알파벳으로 나누어야 한다면, 하나씩 출력하는 방법도 있지만 \n을 사용할 수 있다.*

---
#docstring
```
{
print('''
H
e
l
l
o
''')
}
```
###### *가장 간편하게 알파벳으로 나눌 수 있는 방법은 작은 따옴표 세개를 맨 처음과 끝에 붙여주는 방법이다.*
