# Ex03 Time Table
# Date:28/11/2025
# AIM
To write a html webpage page to display your slot timetable.

# ALGORITHM
## STEP 1
Create a Django-admin Interface.

## STEP 2
Create a static folder and inert HTML code.

## STEP 3
Create a simple table using `<table>` tag in html.

## STEP 4
Add header row using `<th>` tag.

## STEP 5
Add your timetable using `<td>` tag.

## STEP 6
Execute the program using runserver command.

# PROGRAM

{% load static %}

<!DOCTYPE html>

<html>
    <head>
        <title>SLOT TIMETABLE</title>

        <link rel="stylesheet" href="{% static 'CSS.css' %}">

        <link rel="icon" href="{% static 'SEC-Logo-1.png'%}">

    </head>

    <body>
        <center>
            <img src = "{% static 'SAVEETHA.png' %}" height="100" width="700">
        </center>    
        <h2>SLOT TIMETABLE</h2>
        <h3>carlton maximus-25006709</h3>
        <center>
        <table>
        <tr>
            <th> DAY/TIME</th>
            <th> MONDAY</th>
            <th> TUESDAY</th>
            <th> WEDNESDAY</th>
            <th> THURSDAY</th>
            <th> FRIDAY</th>
            <th> SATURDAY</th>
        </tr>
        <tr>
            <td><b>8:00 - 10:00</b></td>
            <td colspan="3"style="text-align:center";>web</td>
            <td rowspan="2"text-align="center";>free</td>
            <td>free</td>
            <td>pyt</td>
         </tr>
         <tr>
            <td><b>10:00 - 12:00</b></td>
            <td>eng</td>
            <td>pyt</td>
            <td>free</td>
            <td>eng</td>
            <td>eng</td>
        </tr>
        <tr style="background-color: #ffe4b5;">
            <td><b>12:00 - 1:00</b></td>
            <td colspan="6"style="text-align:center";><b>LUNCH</b></td>
        </tr>
        <tr>
            <td><b>1:00 - 3:00</b></td>
            <td>web</td>
            <td>free</td>
            <td>mentor meet</td>
            <td>free</td>
            <td>web</td>
            <td>eng</td>
            </tr>
            <tr>
               <td><b>3:00 - 5:00</b></td>
            <td>free</td>
            <td colspan="3"style="text-align:center";>pyt</td>
            <td colspan="3"style="text-align:center";>free</td>
            </tr>
        </table>
        <h3></h3>
        <table border="1" cellspacing="0" cellpadding="10" align="center">
        <tr style="background-color: #ffe4b5;">
            <th>S.no</th>
            <th>sub code</th>
            <th>subject</th>
        </tr>
        <tr>
            <td>1</td>
            <td>19AI301</td>
            <td>python</td>
        </tr>
        <tr>
            <td>2</td>
            <td>19AI404</td>
            <td>web development</td>
        </tr>
        <tr>
            <td>3</td>
            <td>19EN101</td>
            <td>communicative English</td>
        </tr>
        </table>
    </center>
</body> 
</html>


CSS


            table{
                background-color:rgb(127, 180, 244);
                border:2px solid black;
                width:50%;
                text-align:center;
                border-collapse:collapse;
                padding:10px;
            }
            th{
                border: 2px solid black;
                text-align:center;
                padding:10px;
                font-family:"Footlight MT Light";
            }
            td{
                text-align:center;
                padding:10px;
                border:2px solid black;
                background-color:rgb(206, 231, 252);
                font-family: "Palatino Linotype";
            }
            h3{
                text-align:center;
                font-family: "Lucida Calligraphy";
            }
            h2{
                text-align: center;
                font-family:"Eras Medium ITC" ;
            }
            body {
                 font-family: "Montserrat Bold";
                 background-color: rgb(215, 234, 255);
            }

views.py

from django.shortcuts import render

def home(request):
    return render(request, 'timetable.html')

urls.py

from django.contrib import admin
from django.urls import path
from slot_app import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.home)
    
]


# OUTPUT
<img width="1611" height="949" alt="image" src="https://github.com/user-attachments/assets/dabcb58f-6b83-45fd-9f9b-5a841b98e03d" />


# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
