```
a=1
b=2
c=3
s=a+b+c
r=s/3
print(r)
```

---


```
def average():
    a=1
    b=2
    c=3
    s=a+b+c
    r=s/3
    print(r)

average()
```

###### def를 작성 후 함수를 작성한다.
###### 후에 함수식만 작성하면 값이 출력된다.

---

```
def average(a,b,c): #parameter
    s=a+b+c
    r=s/3
    print(r)

average(10,20,30) #argument
```
###### parameter(매개변수)는 a,b,c와 같이 정해지지 않은 값을 뜻한다. 
###### argument(인자)는 함수를 불러들일 때 사용하는 값을 의미한다.

---

```
def average(a,b,c):
    s=a+b+c
    r=s/3
    return r

print(average(10,20,30))
```

###### 하나의 함수는 하나의 값을 가지는 것이 좋기 때문에 return을 사용하여 값을 반환할 수 있다.
###### return은 다른 함수가 사용할 수 있게 그 값을 실제로 갖다 주는 것이다.
