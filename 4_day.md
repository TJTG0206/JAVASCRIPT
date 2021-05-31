DOM & JAVASCRIPT CONTROL
===

### 1. HTML에 javascript/css 문서넣기
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
  const title = document.getElementById("title"); // id가 title인 값을 상수 title에 저장함
  
  console.log(title); // title의 DOM을 출력
  title.innerHTML = "Hi! There!" // title 태그에 내용을 바꾼다
```

### 2. javascript의 문자열처리 방식과 return!!
```javascript
  function sayHello(name, age){
    console.log("Hello" + name + 'you are' + age + "years old"); //'' "" 방식
    console.log(`Hello" ${name} you are ${age} years old`); // `` 백틱방식
  }
  
  function sayHello(name, age){
    console.log(`Hello" ${name} you are ${age} years old`);
  }
  
  const greet = sayHello("alphaka",11); // sayHello의 리턴값이 됨! 
  
  console.log(greet); //greet는 undefined가 됨!
```

```javascript
  function sayHello(name, age){
    return `Hello" ${name} you are ${age} years old`;
  }
  
  console.log(sayhello); // 콘솔 로그를 뱉어냄
```


### 3.계산기
```javascript
  const calculator = {
    plus: function(a,b){
      return a + b;
    }
  }
  
  const plus = calculator.plus(5, 5);
  console.log(plus);
```
