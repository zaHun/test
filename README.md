```javascript

function test(){
   let count = 0
   let in = function(){
      return ++count;
   }
   return in;
}
let increase = test();
console.log(increase());
// 1
console.log(increase());
// 2


console.log(typeof([]))
// object


let product = {
   name : "Mango",
   price : 2000,
   country_of_orgin : "Philippines",
   setPro : function(){  console.log(this.name) }
}

for(let key in window){
   console.log(key + " : " + window[key])
}

let person = {
   age : 15
}
console.log('age' in person)
// true
with(person){
   console.log(age)
   // 15
}

let person = { }
person.age = 17
person.gender = "male"
console.log(person)
// { age:17, gender:"male" } 

delete (person.age)
console.log(person)
// { gender : "male" }

console.log("String")
// "String"
console.log("true")
// "true"  typeof("true")  -> String
console.log(Boolean(""))
// false  typeof -> Boolean

console.log(10, typeof 10)
// 10 "number"
console.log(10.423, typeof 10.423)
// 10.423 "number"
console.log(NaN, typeof NaN)
// NaN "number"

if(true){
   console.log(a)
   // undefined
   var a = 10
}
let b;
console.log(b)
// undefined

console.log(null)
// null
console.log(typeof null)
// "object"

console.log("" == 0)
// true
console.log("5" == 5)
// true

console.log("5" === 5)
// false 자료형 불일치
console.log("" === 0)
// false 자료형 불일치
``'
