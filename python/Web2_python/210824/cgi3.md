```
#!python
print("Content-Type: text/html")
print()
import cgi
cgi.test()
```
###### cgi.test()을 통해 웹 서버가 python에게 주는 정보를 출력할 수 있다.
---

```
<?php
print_r($_SERVER);
?>
```
###### python과 php의 query string이 모두 
###### cgi의 핵심은 웹서버가 사용자의 요청을 받았을 때 요청과 관련하여 웹이 처리할 수 있도록 약속되어 있는 이름의 데이터를 환경변수라는 형태로 전달한다는 것임.
