조건문
===

### 1. if - else

```javascript
  // 1. 일반적인 if-else 
  if(true){
    console.log("Hi!!");
  }else{
    console.log("HELLO!!");
  }
  
  // 2. && 와 ||
  if(true && true){
    console.log("Hi!!");
  }else{  
    console.log("HELLO!!");
  }
  
  /*
   * true && true = true;   
   * true && false = false;
   * false && true = false;
   * false && false = false;   
   */
   
   /*
   * true || true = true;   
   * true || false = true;
   * false || true = true;
   * false || false = false;   
   */
   
   prompt("오오오오오오!! 옛날꺼!");
```

### 2. DOM pratice
```javascript
  const title = document.querySelector("#title");
  
  const BASE_COLOR = "rgb(52, 73, 94)";
  const OTHER_COLOR = "#7f8c8cd";
  
  function handleClick() {
    const currentColor = title.style.color;
    if(currentColor === BASE_COLOR){
      title.style.color = OTHER_COLOR;
    } else {
      title.style.color = BASE_COLOR;
    }
  }
  
  function init() {
    title.style.color = BASE_COLOR;
    title.addEventListener("click",handelClick);
  }
  
  init();
```
이벤트 관련한 정보를 찾으려면 : https://developer.mozilla.org/en-US/docs/Web/API/EventListener
