```javascript

function test(){
   let number = 10
   return {
       getOutput : function(){
           return number
       },
       setOutput : function(value){
           number = value
       }
   }
}
let clo = test("JS")
console.log(clo.getOutput())
// 10
clo.setOutput(30)
console.log(clo.getOutput())
// 30

```
