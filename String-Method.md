### Without JSX 
# String Methods
I do like using string methods 

`let len = basic.length` -Length() method

`let search = basic.charAt(20)` -CharAt() string method 

`let letter = basic.indexOf('s')` -IndexOf() gets the 1st occurrence of letter s 

`lastIndexOf() last occurrence of a` -This get rid of empty spaces in between strings

`document.querySelector('#app').innerHTML = ` -Document from the Dom? I guess, But the #app is the id from <div id="app"> 

`let cut = basic.trim()` -Trim() any space in-between strings like: `let letters = "   A computer requires   "`

`let replace = basic.replace('A', sym.key)` -This replace First letter A with an emoji `sym.key`

```js
const sym = {leftMagnify: `&#128269`, rightMagnify:`&#128270`, lockpen:`&#128271`, 
lockKey: `&#128272`, key:`<h1>&#128273</h1>`, lock: `&#128274`, telescope: `&#128301`}
 
// 
const basic = "A computer requires both 519-318-4909 hardware and software to work.\
 The four basic functions of the microcomputer are input, output, processing,\
and storage of data."

let len = basic.length 
let search = basic.charAt(20) 
let letter = basic.indexOf('s')

let lastLetter = basic.lastIndexOf('a') 
let cut = basic.trim() 

let upper = basic.toUpperCase()
let lower = basic.toLowerCase()

let replace = basic.replace('A', sym.key)



document.getElementById('roll').onclick = function () {

  document.getElementById('A').innerHTML = search
  document.getElementById('B').innerHTML = letter
  document.getElementById('C').innerHTML = upper
}
```

# HTML
```html
  <label id="A">A</label>
    <label id="B">B</label>
    <label id="C">C</label><br><br>
    <button type="button" id="roll">Roll</button>
```
