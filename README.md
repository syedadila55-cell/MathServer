# Ex.04 Design a Website for Server Side Processing
## Date:

## AIM:
To create a web page to calculate total bill amount with GST from price and GST percentage using server-side scripts.

## FORMULA:
Bill = P + (P * GST / 100)
<br> P --> Price (in Rupees)
<br> GST --> GST (in Percentage)
<br> Bill --> Total Bill Amount (in Rupees)

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create a HTML file to implement form based input and output.

### Step 5:
Create python programs for views and urls to perform server side processing.

### Step 6:
Receive input values from the form using request.POST.get().

### Step 7:
Calculate the total bill amount (including GST).

### Step 8:
Display the calculated result in the server console.

### Step 9:
Render the result to the HTML template.

### Step 10:
Publish the website in Localhost.

## PROGRAM:
~~~
<html>
<head>
    <title>GST Calculator</title>
</head>
<body>

    <h2>GST Bill Calculator</h2>

    Price: 
    <input type="number" id="price"><br><br>

    GST %: 
    <input type="number" id="gst"><br><br>

    <button onclick="calculate()">Calculate</button>

    <p id="result"></p>

    <script>
        function calculate() {
            var price = document.getElementById("price").value;
            var gst = document.getElementById("gst").value;

            var total = Number(price) + (Number(price) * Number(gst) / 100);

            document.getElementById("result").innerHTML =
                "Total Bill Amount = ₹ " + total;
        }
    </script>

</body>
</html>
~~~

## OUTPUT - SERVER SIDE:
<img width="360" height="218" alt="Screenshot 2026-02-26 153530" src="https://github.com/user-attachments/assets/5efe75f5-fff8-4ac6-b56a-d5ac39789140" />


## OUTPUT - WEBPAGE:
<img width="330" height="299" alt="Screenshot 2026-02-26 153615" src="https://github.com/user-attachments/assets/cd6aff69-cb90-4819-a240-a0b16022ed81" />


## RESULT:
The a web page to calculate total bill amount with GST from price and GST percentage using server-side scripts is created successfully.
