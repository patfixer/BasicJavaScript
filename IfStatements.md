
# IF Statement
Remember This Is Not JSX
Short way to right an if statement
```js

const sym = {key:`<h1>&#128273</h1>`, lock: `<h1>&#128274</h1>`}
let user = "Jack Black"

document.getElementById('roll').onclick = function () {
  let age = user
  age = 20
  age >= 18 ? document.querySelector('#app').innerHTML = `<h1>Your Of Age</h1>`: document.querySelector('#app').innerHTML = `<h1>Your Not</h1>`
  
}

// Basic way to right an if statement

document.getElementById('roll').onclick = function () {
  let age = user
  age = 20
  if (age >= 18){
    document.querySelector('#app').innerHTML = `<h1>${sym.key}</h1>`
  }else{
    document.querySelector('#app').innerHTML = `<h1>${sym.telescope}</h1>`
  }
}
```
# If Else statement 
```js
let user = "Jack Black"

document.getElementById('roll').onclick = function () {
  let age = user
  age = 20
  if (age >= 18){
    document.querySelector('#app').innerHTML = `<h1>${sym.key}</h1>`
  }else{
    document.querySelector('#app').innerHTML = `<h1>${sym.telescope}</h1>`
  }
}
```

# The && Operator
```js
const hand = {thumbUp: `&#128077`, thumbDown:`&#128078`, whatup:`&#128074`}
 // The && and operator useful for range checking over 30 thumb up, thumb down
document.getElementById('roll').onclick = function () {
  let temp = 31
  if (temp > 0 && temp < 30){
    document.querySelector('#app').innerHTML = `<h1>${hand.thumbUp}</h1>`
  }else{
    document.querySelector('#app').innerHTML = `<h1>${hand.thumbDown}</h1>`
  }
}
```

