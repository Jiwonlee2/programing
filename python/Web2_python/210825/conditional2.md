
```
#!python
print("Content-Type: text/html")
print()
import cgi
form = cgi.FieldStorage()
if 'id' in form:
    pageId = form["id"].value
    description = open('data/'+pageId, 'r').read()
else:
    pageId = 'Welcome'
    description ='Hello, web'
print('''
<!doctype html>
<html>
<head>
  <title>WEB1 - Welcome</title>
  <meta charset="utf-8">
</head>
<body>
  <h1><a href="index.py">WEB</a></h1>
  <ol>
    <li><a href="index.py?id=HTML">HTML</a></li>
    <li><a href="index.py?id=CSS">CSS</a></li>
    <li><a href="index.py?id=JavaScript">JavaScript</a></li>
    <li><a href="index.py?id=Python">python</a></li>
  </ol>
  <h2>{title}</h2>
  <p>{desc}</p>
</body>
</html>
'''.format(title=pageId,desc=description))
```

---

###### if 'id' in form: / pageId = form["id"].value / description = open('data/'+pageId, 'r').read() 
###### else: pageId = 'Welcome' / description ='Hello,
###### web'만약 form에 id가 존재할 경우에는, pageId는 id 그대로, description은 data 파일에 있는 것을 읽도록 하는 것이다. 
###### 그렇지 않을 경우에는 pageId는 Welcome으로, 설명은 Hello, web으로 나타난다.

###### (format기능을 통해 식을 간소화함)
