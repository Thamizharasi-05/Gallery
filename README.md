# Ex.08 Design of Interactive Image Gallery
# Date:17-05-2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
app.html

<html>
    <head>
        <title>Interactive Image Gallery</title>
        <style>
            h1
            {
                color: antiquewhite;
                text-shadow: 0 0 10px rgba(15, 2, 135, 0.364), 0 0 20px rgba(15, 2, 135, 0.364), 0 0 30px rgba(15, 2, 135, 0.364);
                position: relative;
                bottom: 0.5px;
                font-family: Verdana, Geneva, Tahoma, sans-serif;
                font-size: 60px;
                background-image: url("main1.png");
                border-radius: 20px;
            }
            .main
            {
                width: 99%;
                height: 99%;
                background-color: bisque;
                justify-content: center;
                border: 2px solid black;
                border-radius: 20px;
                background-image: url("main1.png");
                background-repeat: no-repeat;
                background-size: cover;
            }
            .m1 
            {
                border-radius: 20px;
                background-color: rgba(15, 2, 135, 0.364);
                position: relative;
                margin: 10px;
                height: 850px;
                width: 1500px;
                display: flex;
                flex-wrap: wrap;
                justify-content: center;
                align-items: center;
                transition: all 1.5s ease;
            }
            .m2
            {
                position: absolute;
                top: 50%;
                right: 10px;
                margin: 10px;
                opacity: 0;
                width: 0px;
                height: 0px;
                transition: all 1.5s ease, opacity 0.4s;
                visibility: hidden;
            }
            img 
            {
                margin: 10px;
                width: 300px;
                height: 300px;
                transition: transform 0.5s ease;
                cursor: pointer;
            }
            #i
            {
                border-radius: 10px;
            }
            #i:hover
            {
                transform: scale(1.1);
            }
            #ii
            {
                border-radius: 10px;
                width: 96%;
                height: auto;
            }

            .m1.shrink 
            {
                position: absolute;
                top: 10px;
                left: 10px;
                width: 350px;
                overflow: scroll;
                transition: all 1.5s ease;
            }
            .m2.grow
            {
            position: absolute;
            top: 10px;
            right: 10px;
            margin: 10px;
            width: 650px;
            height: 650px;
            opacity: 1; /* Fully visible */
            visibility: visible; /* Interactable */
            transition: all 1.5s ease, opacity 0.5s ease;  
            }
            footer{
                background-color: white;
                border-radius: 30px;
                width: 25%;
                position: absolute;
                bottom: 40px;
                left: 50%;
                translate: -50%;
            }
        </style>
    </head>
    <body>
        <h1 align="center">KISH CATTY</h1>
        <div class="main">
            <div class="m1">
                <img src= "c1.png" alt="" id="i" onclick="f(this)">
                <img src= "c2.png" alt="" id="i" onclick="f(this)">
                <img src= "c3.png" alt="" id="i" onclick="f(this)">
                <img src= "c6.png" alt="" id="i" onclick="f(this)">
                <img src= "c7.png" alt="" id="i" onclick="f(this)">
                <img src= "c8.png" alt="" id="i" onclick="f(this)">            
            </div>
            <div class="m2" id="iii" id="i" onclick="c()">
                <img src="" alt="" id="ii">
            </div>
        </div>
        <footer align="center">
            DESIGNED and DEVELOPED by THAMIZHARASI G
        </footer>

        <script>
            var a=document.getElementById('iii');
            var b=document.getElementById('ii');
            const d=document.querySelector('.m1');
            const d1=document.querySelector('.m2');
            function f(img) {
                d1.classList.add('grow');
                d.classList.add('shrink');
                a.style.display='flex';
                b.src=img.src;
            }
            function c(){
                d1.classList.remove('grow');
                d.classList.remove('shrink');
            }
        </script>
    </body>
</html>


```
# OUTPUT:

![alt text](<Screenshot 2025-05-17 073612.png>)
![alt text](<Screenshot 2025-05-17 073636.png>)

# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
