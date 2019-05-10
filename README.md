```javascript

function a(callback){
   for(let i=0;i<2;i++){      
       callback()
   }
}
a(function(){console.log("A")})
// "A"
// "A"

```
