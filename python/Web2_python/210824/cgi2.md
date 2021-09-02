```
#!python
{
print("Content-Type: text/html")
print()
import cgi 
form = cgi.FieldStorage()
pageId = form["id"].value
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
  </ol>
  <h2>{title}</h2>
  <p>The World Wide Web (abbreviated WWW or the Web) is an information space where documents and other web resources are identified by Uniform Resource Locators (URLs), interlinked by hypertext links, and can be accessed via the Internet.[1] English scientist Tim Berners-Lee invented the World Wide Web in 1989. He wrote the first web browser computer program in 1990 while employed at CERN in Switzerland.[2][3] The Web browser was released outside of CERN in 1991, first to other research institutions starting in January 1991 and to the general public on the Internet in August 1991.
  </p>
</body>
</html>
'''.format(title=pageId))
}
```

---


###### CGI는 common gateway interface의 약자로, 홈페이지와 PYTHON SCRIPT를 서로 연동해주는 기능을 한다.
###### import cgi는 cgi module을 사용하기 위해 불러온 것.
###### index.py?id=xxx의 주소를 각각 만들었기에 홈페이지에서 xxx의 버튼을 누르면 xxx의 이름이 출력된 웹주소가 만들어진다.
