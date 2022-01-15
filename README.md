# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 7:

Publish the website in the given URL.

## PROGRAM :
```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mathematical Calculations</title>
    <style>
        *{
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }
        body{
            background-color:#dfe0e9;
            color:yelloww;
        }
        .container{
            width: 1080px;
            margin-left: auto;
            margin-right: auto;
            background-color: #c9d1d1;
            border:#5f4688;
        }
        .content{
            display: block;
            width: 100%;
            background-color:#58aa;
            margin-top: 40px;
            min-height: 400px;
        }
        .text{
            text-align: center;
            padding-top: 50px;
            text-decoration: underline;
        }
        .formelement{
            text-align: center;
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 25px;
            margin-top: 5px;
            margin-bottom: 5px;

        }
        .content2{
            display: block;
            width: 100%;
            background-color:#72B4E6;
            margin-top: px;
            min-height: 400px;
        }
        .by{
            text-align: center;
            color: black(245, 240, 240);
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
        }
    </style>

</head>

<body>
    <div class="container">
        <div class="content">
            <h1 class="text"><B>Area of paralelogram</B></h1>
            <form>
                <div class="formelement"><label for="aEdit">Base:</label>
                    <input type="number" id="aEdit" value="0"/>
                    <lable for="aedit">Meters</lable>
                </div><br>
                
                <div class="formelement">
                    <label for="bEdit">Height:</label>
                    <input type="number" id="bEdit" value="0"/>
                    <lable for="aedit">Meters</lable>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="AddButton"/>
                </div>
                
                <div class="formelement">
                    <label for="cEdit">Area:</label>
                    <input type="text" id="cEdit" value="0" readonly />
                    <lable for="aedit">Meter<sup>2</sup></lable>
                </div><br>
                <div class=formelement>
                   
                </div>
            </form>

        </div>
        <div class="content2">
            <h1 class="text">Area of rectangle</h1>
            <form>
                <div class="formelement"><label for="hEdit">Length:</label>
                    <input type="number" id="hEdit" value="0"/>
                    <lable for="aedit">Meters</lable>
                </div><br>
                
                <div class="formelement">
                    <label for="rEdit">Width:</label>
                    <input type="number" id="rEdit" value="0"/>
                    <lable for="aedit">Meters</lable>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="AddButton1"/>
                </div>
                
                <div class="formelement">
                    <label for="vEdit">Volume:</label>
                    <input type="number" id="vEdit" value="0" readonly />
                    <lable for="aedit">Meter<sup>3</sup></lable>
                </div><br>
                <div class="formelement">
                 
                    </div><br>
                   
            </form>

        </div>
    </div>
    <script>
        function validate(){
            var user1=document.getElementById("aedit").value;
            var user2=document.getElementById("bedit").value;
            var user3=document.getElementById("redit").value;
            var user4=document.getElementById("hedit").value;
            var re = /^[0-9]+$/;
            if (re.test(user1)){
                return true;
      }
            else if (re.test(user2)){
                return true;
         }
         else if (re.test(user3)){
                return true;
         }
         else if (re.test(user4)){
                return true;
         }
            else {
                alert('Please input numeric characters only');
                return false;
        }
       
        }
    </script>
    <script type="text/javascript">
        var button,button1;
        button = document.querySelector("#AddButton");
        
        button.addEventListener("click",function(){
            var aText,bText,cText;
            var aVal,bVal,cVal;
            aText=document.querySelector("#aEdit");
            bText=document.querySelector("#bEdit");
            cText=document.querySelector("#cEdit");

            aVal = parseInt(aText.value);
            bVal = parseInt(bText.value);
            cVal = (aVal*bVal)/2;
            cText.value = ""+cVal;
        });
        button1 = document.querySelector("#AddButton1");
        button1.addEventListener("click",function(){
            var aText,bText,cText;
            var aVal,bVal,cVal;
            hText=document.querySelector("#hEdit");
            rText=document.querySelector("#rEdit");
            vText=document.querySelector("#vEdit");

            hVal = parseInt(hText.value);
            rVal = parseInt(rText.value);
            vVal = (22/7*rVal*rVal)*(hVal/3);
            vText.value = ""+vVal;
        });

    </script>
    <footer> <p class="by"><B>Developed by : K.M.Swetha </B></p></footer>
</body>
</html>
```

## OUTPUT:
![image](https://user-images.githubusercontent.com/94228215/149629231-37654f2f-6000-464c-9a3a-13e8ffdaf9fa.png)


## Result:

Thus a website is designed to perform mathematical calculations in the client side.
