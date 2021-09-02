###### python 프로그램을 시작할 때 id, pwd 순서대로 물어보는 작업
```
user_id = input('id?')
user_pwd = input('password?')
```

---

```
if user_pwd == '111111':
    print("Hello Master")
else:
    print('Who are you?')
```

```
if user_id == 'egoing':
    if user_pwd == '111111':
        print("Hello Master")
    else:
        print("Who are you?")
else:
    print("Who are you?")
```

```
if user_id == 'egoing' and user_pwd == '111111':
    print("Hello Master")
elif user_id == 'jiwon' and user_pwd == '222':
    print("Hello Jiwon")
else:
    print("Who are you?")
```

---

###### id가 틀릴경우 pwd를 물어보지 않고 바로 who are you?를 출력하는 방법

```
user_id=input('id?')

if user_id == 'jiwon'
    user_pwd = input('password?')
        if user_pwd == '111111':
        print("Hello Master")
    else:
        print("Who are you?")
else:
    print("Who are you?")
```
