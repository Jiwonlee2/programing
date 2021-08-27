## string3

name = 'apple'
age = 'one'

---

```
print('to '+name+'. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim apple veniam, quis nostrud exercitation
ullamco laboris nisi ut aliquip ex ea commodo consequat. '+name+' Duis aute irure dolor in '+age+' 
reprehenderit apple computer in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur
sint occaecat cupidatat non proident, sunt in culpa qui '+name+' officia deserunt mollit anim id est laborum.')
```
###### +기호는 앞과 뒤를 연결해주는 기능을 한다.
###### name과 age라는 변수를 미리 만들었으므로, 각각의 자리에 각각의 값을 넣는다.
---

[positional formatting]
###### format은 값을 출력하기 위해 사용하는 함수이다. 

```
print('to '+name+'. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim apple veniam, quis nostrud exercitation
ullamco laboris nisi ut aliquip ex ea commodo consequat. '+name+' Duis aute irure dolor in '+age+' 
reprehenderit apple computer in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur
sint occaecat cupidatat non proident, sunt in culpa qui '+name+' officia deserunt mollit anim id est laborum.'
.format('egoing', 12, 'egoing', 'egoing'))
```

---

[named placeholder]
###### 위 부분보다 더욱 간편하게 출력할 수 있는 방법은 각각의 자리에 named placeholder를 작성한 후 .format 기능을 사용하여 값을 출력할 수 있다.

```
print('to '+name+'. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim apple veniam, quis nostrud exercitation
ullamco laboris nisi ut aliquip ex ea commodo consequat. '+name+' Duis aute irure dolor in '+age+' 
reprehenderit apple computer in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur
sint occaecat cupidatat non proident, sunt in culpa qui '+name+' officia deserunt mollit anim id est laborum.'
.format(name="egoing", age=12))
```
