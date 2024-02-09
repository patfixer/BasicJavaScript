
# firstElementChild
You can see here that i need to get element id first then i have access to firstElementChild, and with firsChild i can add a backgroundColor `firstChild.style.backgroundColor = "lightblue"`...

```js
const element1 = document.getElementById('question1')
const firstChild = element1.firstElementChild

firstChild.style.backgroundColor = "lightblue"
```

# querySelectorAll()
This adds green to the first element in the ordered list, adds color looping through
with the `forEach()` method and inside is an arrow function `ol =>{}`, change the background color `first.style.backgroundColor = "green"`.
```js
const element1 = document.getElementById('question1')
const firstChild = element1.firstElementChild

const orderElements = document.querySelectorAll('ol')

orderElements.forEach(ol => {
    const first = ol.firstElementChild
    first.style.backgroundColor = "green"

})
```

# lastElementChild 
```js
const orderElements = document.querySelectorAll('ol')

orderElements.forEach(orderElements => {
    const lastChild = orderElements.lastElementChild
    lastChild.style.backgroundColor = "green"
})
```
