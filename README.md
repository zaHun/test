```javascript

function test(name){
   let output = "Hello :"+name
   return function(){
       console.log(output)
   }
}
test("JS")()
// Hello : JS

```
