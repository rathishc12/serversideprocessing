# Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:

### Step 1:
Create a new django project and app.

### Step 2:
Make on changes in settings and create templates folder.

### Step 3:
Create a code for frontend of calculation using HTML and CSS and save it in templates.

### Step 4:
Give an url mapping and write a python code for calculation in views.

### Step 5:
Take a screenshotof the site and upload it.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
    <head>
        
        <Title>Calculate area of rectangle</Title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
        body{background-color: violet;
        }
        .edge{
            width:1080px;
            margin-left:auto;
            margin-right: auto;
            padding-top: 200px;
            padding-left: 300px;
        }
        .box{
            display: block;
            border: darkslateblue;
            width:500px;
            min-height: 300px;
            font-size: 20px;
            background-color:cyan;
            text-align:center;
            margin-left:auto;
            margin-right: auto;
        }
        .formelt{
            color:red;
            text-align: center;
            margin-top: 5px;
            margin-bottom: 5px;
        }
        .h1{
            color:red;
            text-align: center;
            padding-top: 20px;
        }

        </style>

    </head>
    <body>
        <div class="edge">
            <div class="box">
                <h1>Area of Rectangle</h1>
                <form method="POST">
                {% csrf_token%}
                <div class="formelt">
                    Length: <input type="text" name="length" value="{{length}}"></input>(in m)<br/>
                </div>
                <div class="formelt">
                    Breadth: <input type="text" name="breadth" value="{{breadth}}"></input>(in m)<br/>
                </div>
                <div class="formelt">
                    <input type="submit" value="Calculate"></input><br/>
                </div>
                <div class="formelt">
                    Area: <input type="text" name="area" value="{{area}}"></input>m<sup>2</sup><br/>
                </div>
                </form>
            </div>

        </div>

    </body>
</html>
```
## OUTPUT:

### Home Page:
![8 (1)](https://github.com/rathishc12/serversideprocessing/assets/120539398/bfd43d2d-548a-44d5-8ab6-cd27246613eb)
### server output
![8 (2)](https://github.com/rathishc12/serversideprocessing/assets/120539398/3c4b9259-f426-4d82-8272-a0ad52bf2ea3)

## Result:
Hence the programme executed sucessfully..
