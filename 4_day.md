DOM & JAVASCRIPT CONTROL
===

```HTML
<!DOCTYPE html>
<html>
  <head>
    <title>Something</title>
    <link rel="stylesheet" href="index.css" />
  </head>
  <body>
    <h1>This works!</h1>
    <script src="index.js" />
  </body>
</html>
```

```CSS
body{
 background-color:peru; 
}

h1{
  color:white;
}
```

```javascript
  const title = document.getElementById("title");
  
  console.log(title); // title의 DOM을 출력
  title.innerHTML = "Hi! There!" // title 태그에 내용을 바꾼다
```
