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

console.log(NaN == NaN)
// false
console.log(NaN === NaN)
// false
console.log(isNaN(NaN))
// true

console.log(typeof Number("5"))
// "number"
console.log(typeof String(5))
// "string"
console.log(parseInt("5.32"), typeof parseInt("5.32"))
// 5 true
console.log(Boolean(0))
// false
console.log(parseFloat("5.32"))
// 5.32

window.open([URL], [name], [features], [replace])
// 새 window 객체를 생성 (새 창 열기)

``'
