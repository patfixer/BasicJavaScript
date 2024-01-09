# Dice Game
When I have a function rollDice() This gives me an error saying 
that the rollDice() function is not defined. 
And I do like writing it this way by getting the element by id
```js
/**/
document.getElementById('rollDice').onclick = function () {
    const numOfDice = document.getElementById('numOfDice').value;
    const diceResult = document.getElementById('diceResult');
    const diceImages = document.getElementById('diceImages');
    const values = []
    const images = []

    for (let i = 0; i < numOfDice; i++) {
        const value = Math.floor(Math.random() * 6) + 1;
        values.push(value)
        images.push(`<img src="./images/${value}.png">`)
    }

    diceResult.textContent = `dice: ${values.join(',')}`;
    diceImages.innerHTML = images.join('');
}
```

# HTML 
```html
    <div id="container">
    <h1>Dice Roller</h1>
    <label># Dice</label>
    <br>
    <input type="number" id="numOfDice" value="1" min="1"/>
    <br>
    <br>
    <button id="rollDice">Roll Dice</button>
    <br>
    <div id="diceResult"></div>
    <div id="diceImages"></div>
  </div>
```

# CSS PART
```css
:root {
  font-family: Inter, system-ui, Helvetica, Arial, sans-serif;
  line-height: 1.5;
  font-weight: bold;
  text-align: center;

  color-scheme: light dark;
  color: rgba(255, 255, 255, 0.87);
  background-color: #242424;
  margin: 0;
}

button {
  border: 0;
  line-height: 2.5;
  padding: 0 20px;
  font-size: 1rem;
  text-align: center;
  color: #f7d40a;
  text-shadow: 1px 1px 1px #fb0606;
  border-radius: 10px;
  background-color: rgb(0, 205, 220);
  background-image: linear-gradient(
    to top left,
    rgba(0, 0, 0, 0.2),
    rgba(0, 0, 0, 0.2) 30%,
    rgba(0, 0, 0, 0)
  );
  box-shadow:
    inset 2px 2px 3px rgba(255, 255, 255, 0.6),
    inset -2px -2px 3px rgba(0, 0, 0, 0.6);
}


button:hover {
  background-color: rgb(26, 255, 0);
  cursor: pointer;
}

button:active {
  box-shadow:
    inset -2px -2px 3px rgba(255, 255, 255, 0.6),
    inset 2px 2px 3px rgba(0, 0, 0, 0.6);
}

#diceResult {
  margin: 25px;
}

#diceImages img{
  width: 80px;
}
```


# This give me an error 
Uncaught ReferenceError: rollDice is not defined
at HTMLButtonElement.onclick
```js
function rollDice() {
    const numOfDice = document.getElementById('numOfDice').value;
    const diceResult = document.getElementById('diceResult');
    const diceImages = document.getElementById('diceImages');
    const values = []
    const images = []

    for (let i = 0; i < numOfDice; i++) {
        const value = Math.floor(Math.random() * 6) + 1;
        values.push(value)
        images.push(`<img src="./images/${value}.png alt="images">`)
    }

    diceResult.textContent = `dice: ${values.join(', ')}`;;
}

rollDice()
```

```js

```
