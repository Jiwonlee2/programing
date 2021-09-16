# LIST 
* 대괄호[]로 데이터들을 감싸며 표현하며, []안의 데이터를 요소(element)라고 한다.
* List는 여러 element로 구성되어 있으며, 문자열처럼 각 element들에 순서가 있다.   
따라서 indexing을 통해 각 element들을 불러들어 올 수 있다.
* element들의 생성, 삭제, 수정이 가능하다.
* element가 없는 비어있는 list도 표현가능하다.   
element의 type이 Integer 인 경우 그대로 표현하고, string 일 경우 따옴표로 감싸서 표현한다.
* indexing을 통해 출력한 element들의 value를 연산하여 출력도 가능하다.
* list의 맨 마지막 index는 '-1'이다.


```
a = [1, 2, 3, ['a' ,'b' ,'c']]

a[0] = 1

a[-1] = ['a' ,'b' ,'c']

a[3] = ['a' ,'b' ,'c']

a[-1][0] = 'a'

a[-1][1] = 'b'

a[-1][2] = 'c'

a[0] + a[2] = 4
```
```
<sliding>
a = [1, 2, 3, 4, 5]

a[0:2] = [1, 2]

a[:5] = [1, 2, 3, 4, 5]

a[:4:2] = [1, 3]
```

### list 함수
* count(원소) : 리스트 내 특정 원소가 몇 개 포함되어 있는지 반환
* index(원소) : 리스트 내 특정 원소의 인덱스를 반환
* append(원소) :리스트의 뒤쪽에 새로운 원소를 삽입
* sort() : 리스트를 오름차순으로 정렬
* extend(리스트) : 리스트의 뒤쪽에 다른 리스트를 삽입
* insert(인덱스, 원소) : 특정한 위치(인덱스)에 원소를 삽입
* remove(원소) : 리스트 내 특정 원소를 삭제
* pop(인덱스) : 리스트 내 특정 인덱스의 원소를 삭제
* reverse() : 리스트의 순서를 뒤집기

```
a = [1,2,3,1]

a.count(1) = 2

a.index(2) =3

a.append(2) = [1,2,3,1,2]

a.sort() = [1,1,2,3]

a.extend([4,5]) = [1,2,3,1,4,5]

a.index(0,4) = [4,1,2,3,1]

a.remove(1) = [2,3,1]

a.pop(1) = [1,3,1]

a.reverse() = [1,3,2,1]
```

---
# TUPLE
* Tuple은 element들을 '()'로 감싸고 있어 List와 비슷한 역할을 하지만, 다른 특성을 가지고 있다.
* Tuple은 List처럼 elemnet들의 순서가 있지만 element들의 생성, 삭제, 수정이 불가능하다.

### Tuple 함수
* indexing
* sliding
* 더하기
* 곱하기

```
t = (1,2,'a','b')
t1 = (3,4)

t[0] = 1

t[3] = 'b'

t[1:] = (2,'a','b')

t + t1 = (1,2,'a','b',3,4)

t1 *2 = (3,4,3,4)

len(t) = 4
```
---

# DICTIONARY
* 데이터가 다양해지고 속성과 값들의 표현들이 많아져 단순 List나 tuple로 데이터를 표현하기가 힘들다.     
데이터들의 대응관계(속성과 값)를 잘 나타낼 수 있는 자료형이 Dictionary이다.
* 사전이라는 의미로 예를들어 "people"이라는 단어에 "사람"그리고 "baseball"이라는 단어에는 "야구"라는 뜻을 부합시키듯,     
Dictionary에서도 Key와 Value로 한 쌍을 이루어 element를 갖는다.
* element들은 순서를 갖지 않고, dictionary에서 원하는 element를 찾고자하면 element의 key를 통해 value를 얻을 수 있다. 

### Dictionary 표현
```
{Key1:Value1, Key2:Value2, Key3:Value3, ...}
dic = {'name':'jiwon', 'phone':'0123456789', 'birth': '0924'}
```

### Dictionary element 추가, 삭제
```
a = { 1 : 'a' }
a[2] = 'b'
a['name'] = 'jiwon'
a[3] = [1,2,3]

a = {1: 'a', 2: 'b', 'name': 'jiwon', 3: [1, 2, 3]}
```
```
del a[1]
a = {2: 'b', 'name': 'jiwon', 3: [1, 2, 3]}
```
_value에 list를 넣을 수 있다._

### Dictionary Key-Value 확인
```
dic = {'name':'jiwon', 'phone':'0123456789', 'birth': '0924'}
grade['name'] = 'jiwon'
grade['birth'] = '0924'
```

**Key에는 list를 사용할 수 없지만, tuple은 사용할 수 있다. list는 값이 변할 수 있기 때문에 Key로 쓸 수 없다.**

### Dictionary 함수
* keys()
* values()
* items() : Key와 Value의 쌍을 튜플로 묶은 값을 dict_items 객체로 돌려준다.
* clear() : dictionary 안의 모든 요소를 삭제한다
* get() :  ()안의 Key에 대응되는 Value를 돌려준다.


```
a = {'name':'jiwon', 'phone':'0123456789', 'birth': '0924'}

a.keys() = dict_keys(['name', 'phone', 'birth'])

a.values() = dict_values(['jiwon', '0123456789', '0924'])

a.items() = dict_items([('name', 'jiwon'), ('phone', '0123456789'), ('birth', '0924')])

a.clear() = a {}

a.get('name') = 'jiwon'
```
