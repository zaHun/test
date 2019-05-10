```javascript

let a = setTimeout(function(){
   console.log("A")
}, 1000)
clearTimeout(a)
// 실행이 중단되어 아무것도 출력되지 않는다.
```
