# calculator

Project Description:

This project is a standard calculator built using HTML, CSS, and JavaScript. The calculator is designed to perform basic arithmetic operations such as addition, subtraction, multiplication, and division. The goal of this project is to create a user-friendly, functional calculator that mimics the behavior of a physical calculator.

Features:

Basic Arithmetic Operations: Supports addition, subtraction, multiplication, and division.

Clear and Responsive UI: Designed with a clean and intuitive user interface for easy interaction.

Real-Time Display: Shows the current input and results in real-time.

Error Handling: Includes error handling for division by zero and invalid inputs.

Keyboard Support: Allows users to perform calculations using keyboard input.

Technologies Used:

HTML: Structure and layout of the calculator.

CSS: Styling and appearance of the calculator.

JavaScript: Functionality and logic for performing calculations.

Code Structure:

calc.html: Contains the HTML structure of the calculator.

calc.css: Contains the CSS styles for the calculator.

calc.js: Contains the JavaScript logic for the calculator functionality.


## calc.html:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Calculator</title>
    <link rel="stylesheet" href="calc.css" />
  </head>
  <body>
    <h1 class="text-center">CALCULATOR!</h1>
    <div class="container">
      <div class="row">
        <form>
          <div class="display">
            <input type="text" name="display" />
          </div>
          <div>
            <input
              type="button"
              value="AC"
              onclick="display.value = '' "
              class="operator"
            />
            <input
              type="button"
              value="DE"
              onclick="display.value = display.value.toString().slice(0,-1) "
              class="operator"
            />
            <input
              type="button"
              value="."
              onclick="display.value += '.' "
              class="operator"
            />
            <input
              type="button"
              value="/"
              onclick="display.value += '/' "
              class="operator"
            />
          </div>
          <div>
            <input type="button" value="7" onclick="display.value += '7' " />
            <input type="button" value="8" onclick="display.value += '8' " />
            <input type="button" value="9" onclick="display.value += '9' " />
            <input
              type="button"
              value="*"
              onclick="display.value += '*' "
              class="operator"
            />
          </div>
          <div>
            <input type="button" value="4" onclick="display.value += '4' " />
            <input type="button" value="5" onclick="display.value += '5' " />
            <input type="button" value="6" onclick="display.value += '6' " />
            <input
              type="button"
              value="-"
              onclick="display.value += '-' "
              class="operator"
            />
          </div>
          <div>
            <input type="button" value="1" onclick="display.value += '1' " />
            <input type="button" value="2" onclick="display.value += '2' " />
            <input type="button" value="3" onclick="display.value += '3' " />
            <input
              type="button"
              value="+"
              onclick="display.value += '+' "
              class="operator"
            />
          </div>
          <div>
            <input type="button" value="00" onclick="display.value += '00' " />
            <input type="button" value="0" onclick="display.value += '0' " />
            <input
              type="button"
              value="="
              onclick="display.value=eval(display.value)"
              class="equal operator"
            />
          </div>
        </form>
      </div>
    </div>
  </body>
</html>

```

## calc.css:

```
.text-center{
    text-align: center;
}
.container{
    width: 100%;
    height: 100vh;
    background: #e3f9ff;
    display: flex;
    align-items: center;
    justify-content: center;
}
.row{
    background: #3a4452;
    padding: 20px;
    border-radius: 10px;
}

.row form input{
    border: 0;
    outline: 0;
    width: 60px;
    height: 60px;
    border-radius: 10px;
    box-shadow: -8px -8px 15px rgba(255,255,255,0.1),5px 5px 15px rgba(0, 0, 0, 0.2);
    background: transparent;
    font-size: 20px;
    color: #fff;
    cursor: pointer;
    margin: 10px;
}
form .display{
    display: flex;
    justify-content: flex-end;
    margin: 20px 0;
}
form .display input{
    text-align: right;
    flex:1;
    font-size: 45px;
    box-shadow: none;
}
form input.equal{
    width: 145px;
}
form input.operator
{
    color: #33ffd8;
}
```

## OUTPUT:

![Screenshot (121)](https://github.com/Niteeshmohan/CALCULATOR/assets/119575445/2d6f92ba-857c-4545-8293-80fca0564406)

![Screenshot (122)](https://github.com/Niteeshmohan/CALCULATOR/assets/119575445/b62887dc-5ba8-4c95-90a7-09e0e7acdb7c)

![Screenshot (123)](https://github.com/Niteeshmohan/CALCULATOR/assets/119575445/7b61fd36-3237-4116-af9c-cfdd502314a5)


