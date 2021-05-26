Data Type
===
정렬
===
### 1. Object[객체]

```javascript
  const Info = {
    name      : "Alphaka" ,
    age       : "1"       ,
    gender    : "Male"    ,
    isHansome : true      ,
    favFoods  : ["Pizza","Hambuger","Chicken"],
    favMovies : [
      {
        name:"Oldboy",
        isFun:false
      },
      {
        name:"LOTR",
        isFun:true
      },
      {
        name:"ASK",
        isFun:false
      }
      ],
  }
  
  // Original 
  console.log(Info);
  
  Info.gender = "Female";
  
  // Changed Object
  console.log(Info.favMovies[0].isFun);
```

### 2. function[함수]
```javascript
  // 파라메터가 없을때
  function sayHello(){
    console.log("Hello!!");
  }
  
  sayHello();           //출력...Hello!!
```

```javascript
  // 파라메터가 1개
  function sayHello(potato){
    console.log("Hello!!", potato);
  }
  
  sayHello("Alphaka!"); //출력...Hello!! Alphaka!
  console.log("Hi");    //출력...Hi!
```

```javascript
  // 파라메터가 2개
  function sayHello(potato, juice){
    console.log("Hello!!", potato, "you have ", juice);
  }
  
  sayHello("Alphaka!", "juice"); //출력...Hello!! Alphaka! you have juice
```
