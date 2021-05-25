변수 선언
===
### 1. 문장의 마무리는 ";"

```javascript
let a = 221;        
let b = a - 5;      
a = 4;             
console.log(b, a);  // 출력... 216, 4
```

### 2. var, let, const
```javascript
//var은 여러번 선언할 수 있고, 값을 바꿀 수 있음.
  var a = 1; //(O)
  var a = 2; //(O)
  a = 1;     //(O)
  
//let은 한번만 선언할 수 있고, 값을 바꿀 수 없음.
  let b = 1; //(O)
  let b = 2; //(X)
  b = 2;     //(O)
  
//const는 한번만 선언할 수 있고, 값을 바꿀 수 없음.
  const c = 1; //(O)
  const c = 2; //(X)
  c = 2;       //(O)
```
