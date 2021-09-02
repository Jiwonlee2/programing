```
square = [1, 'four', 9, 16, 25]
print(square)
print(square[0])
print(square[1])
print(len(square))
```
###### list에서도 string과 마찬가지로 len을 통해 전체 길이를 알 수 있으며, 0부터 센다.

---

```
square[1] = 4
print(square)
```
###### [1]은 list의 두번째 자리를 말하며, 그 값을 4로 바꾸게 할 수 있다.

---
```
del square[2]
print(square)
```
###### list에서 3번째 자리의 값을 삭제하기 위해선, del의 기능을 이용할 수 있다.

---
```
square.append('jiwon')
print(square)
```
###### .append()를 사용하여, list의 마지막 자리에 값을 추가할 수 있다.
