변수 선언
===
### 1.HTML 태그를 선택해서 속성변경하기

```javascript
  const title = document.getElementById("title"); // ID로 태그를 선택함
  const queries = document.querySelector("#title"); //CSS방식으로 태그를 선택함
  title.innerHTML = "Hi, From JS";
  title.style.color = "red"; //css속성중 color를 red로 변경함
  console.log(title); // title의 html태그를 보여줌
  console.dir(title); // title의 DOM 목록을 보여줌
```

### 2. EventListener 사용하기

```javascript
  const title = document.querySelector("#title"); 
  
  function handleResize(){
    console.log("I have been resized");
  }
  
  window.addEventListener("resize", handleResize()); // 함수를 바로 실행함!!
  
  window.addEventListener("resize", handleResize); // 이벤트가 발생할때만 실행함!!
```

```javascript
  const title = document.querySelector("#title"); 
  
  function handleResize(event){
    console.log(event); // resize event를 호출함
  }
  
   function handleTitle(){
    title.style.color = 'red'; // 빨간색을 title 속성값으로 변경함
  }
  
  title.addEventListener("click",handleTitle); // 클릭할때 handleTitle 함수를 실행함
```
