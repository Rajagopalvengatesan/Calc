# Ex.08 Design of a Standard Calculator
## Date:21/12/2023

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html


<html>
<head>

    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="text"> 
        <h1 align="center"> <b>  CALCULATOR  </b></h1>
        <br>
       
        <h2 align="center">RAJAGOPAL (23002920)</h2>
    </div>
    <div class="container"> 
        <div class="calculator">
            <input type ="text" placeholder="0" id="output-screen">
            <button onclick="Clear()">AC</button>
            <button onclick="Del()">DEL</button>
            <button onclick="display('%')">%</button>
            <button onclick="display('/')">/</button>
            <button onclick="display('7')">7</button>
            <button onclick="display('8')">8</button>
            <button onclick="display('9')">9</button>
            <button onclick="display('*')">*</button>
            <button onclick="display('4')">4</button>
            <button onclick="display('5')">5</button>
            <button onclick="display('6')">6</button>
            <button onclick="display('-')">-</button>
            <button onclick="display('1')">1</button>
            <button onclick="display('2')">2</button>
           <button onclick="display('3')">3</button>
            <button onclick="display('+')">+</button>
            <button onclick="display('.')">.</button>
            <button onclick="display('0')">0</button>

            <button onclick="calculate()" class="equal">=</button>


        </div>

    </div>
   

    <script>
        let outputScreen = document.getElementById("output-screen");

        function display(num){
            outputScreen.value += num;
        }
        function calculate()
     {
            try{
                outputScreen.value = eval(outputScreen.value);
  }
            catch(err)
            {
                alert("invaild ")
            }
     }
        
            function Clear(){
                outputScreen.value ="";
            }
        
        function Del(){
            outputScreen.value = outputScreen.value.slice(0,-1);
        }
    
        
    </script>
    
</body>
</html>

style.html

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-color: rgba(13, 238, 201, 0.412);
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    outline: none;
}

.container{
    height: 50vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.calculator{
    background-color: rgba(183, 231, 8, 0.712);
    box-shadow: inset 5px 5px 12px #fafafa,
                      5px 5px 12px rgba(0, 0, 0, 0.16);
    display: grid;
    grid-template-columns: repeat(4,68px);
}
input{
    grid-column: span 4;
    width: 70px;
    width: 260px;
    background-color: rgb(255, 255, 255);
    box-shadow: inset -5px -5px 12px
                inset  5px 5px 12px rgba(0, 0, 0, 0.16);
    border: none;
    border-radius: 30px;
    color: rgb(70, 70, 70);
    font-size: 50px;
    text-align: end;
    margin: auto;
    margin-top : 40px;
    margin-bottom: 30px;
    padding : 20px;

}

button{
    height: 48px;
    width: 48px;
    background-color: rgb(255, 255, 255);
    box-shadow: -5px -5px 12px #ffff
                    5px 5px 12px rgba(0, 0, 0, 0.16);
    border: none;
    border-radius: 50px;
    margin: 8px;
    font-size: 16px;
}

.equal{
    width: 115px;
    border-radius: 40px;
    background-color: rgb(255, 255, 255);
    box-shadow: -5px -5px 12px #ffff
                    5px 5px 12px rgba(0, 0, 0, 0.16);

}

.text{ 
font-weight: bolder;
color: black;
text-align: center;
margin-left: 30px;
font-size: 100px;
 
}
```

## OUTPUT:
![Alt text](<Screenshot (60).png>)
![Alt text](<Screenshot (61).png>)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
