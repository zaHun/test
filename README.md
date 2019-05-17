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

var testVar = 2483
console.log(window.testVar)
// 2483

window.open([URL], [name], [features], [replace])
// 새 window 객체를 생성 (새 창 열기)

console.log(screen.width)
// 화면의 너비
console.log(screen.height)
// 화면의 높이
console.log(screen.availWidth)
// 실제 화면에서 사용 가능한 너비
console.log(screen.availHeight)
// 실제 화면에서 사용 가능한 높이
console.log(screen.colorDepth)
// 사용 가능한 색상 

location.assign( link )
// 해당 link 로 강제 이동
location.reload()
// 페이지 새로고침
location.replace( link )
// 해당 link 로 이동 (assing 과 다르게 뒤로가기 불가)

window.onload = function(){ }
// window 객체의 Load Complete 시점 

console.log(navigator.appCodeName)
// "Mozilla"  (Browser Code)
console.log(navigator.appName)
// "Netscape"  (Browser Name)
console.log(navigator.appVersion)
// "5.0 (Windows ~~~~) (Browser Version)
console.log(navigator.platform)
// "Win32" (Using OS)


window.onload = function(){
   let wrap = document.getElementById("wrap")
}

let h1 = document.createElement("h1");
// h1 tag 생성
let textNode = document.createTextNode("Hello Create");
// Text Node 생성 
h1.appendChild(textNode)
// h1 tag 에 생성한 Text Node 연결
document.body.append(h1)
// document.body 태그에 h1 를 연결

let tit = document.createElement("h1")
tit.setAttribute("width", 500)
tit.setAttribute("height", 300)
console.log(tit.getAttribute("width"))
// 500


``'
