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
<html>
<head>
    <title>My Timetable</title>
</head>
<body style="font-family: Arial; text-align: center;">

    <img src="images.png">
    <h2> Timetable</h2>
    

    <table border="1" cellspacing="0" cellpadding="10" align="center">
        <tr style="background-color: #d0e0ff;">
            <th>Time</th>
            <th>Monday</th>
            <th>Tuesday</th>
            <th>Wednesday</th>
            <th>Thursday</th>
            <th>Friday</th>
            <th>Saturday</th>
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
    <br>
    <br>
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

</body>
</html>

# OUTPUT
<img width="1720" height="930" alt="image" src="https://github.com/user-attachments/assets/03daebc9-01c9-4875-8da1-df10b334a377" />

# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
