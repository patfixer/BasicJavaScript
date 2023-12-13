# Getting Lenght With If Statement
Not the Lenght of basic is 152 but ${both} comes up this should be ${hand.thumbUp} but is not ???
```js
const basic = "A computer requires both hardware and software to work.\
 The four basic functions of the microcomputer are input, output, processing,\
and storage of data."

const hand = {thumbUp: `&#128077`, thumbDown:`&#128078`, whatup:`&#128074`}
let first = basic.slice(0, basic.indexOf(" "))
let last = basic.slice(basic.indexOf(" ") + 1)
let len = basic.length

document.getElementById('roll').onclick = function () {
  let both = first + last
  if (both == 152){
    document.querySelector('#app').innerHTML = `<h1>${hand.thumbUp}</h1>`
  }else{
    document.querySelector('#app').innerHTML = `<h1>${both}</h1>`
  }
}
```
'&#128078;' Can only render in HTML dynamically.  <h1>&#128078;</h1>