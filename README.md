<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{
            box-sizing: border-box;
        }
        body{
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            margin:15px,30px;
            font-size: 17px;
            padding: 8px;
        }
        .container {
            background-attachment: #ffff;
            padding: 5px,20px,15px,20px;
            border: 1px solid lightgrey;
            border-radius: 4px;
        }
        input[type="text"],
        input[type="email"],
        input[type="number"],
        input[type="password"],
        input[type="date"],
        select,
        textarea{
            width:100%;
            padding:12px;
            border: 1px  solid #ccc;
            border-radius:5px;
            margin: 1px;
        }
        fieldset{
            background-color: #ffff;
            border:1px solid #ccc;
        }
        .main.heading{
            text-align: center;
        }
        input[type="submit"]{
            background-color: royalblue;
            color: white;
            padding: 12px,20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;

        }
        input[type="submit"]:hover{
           background-color: royalblue;
        }
    </style>
   
</head>
<body>  
        <div class="container">
            <form action="" method="get">
        <h1>Payment Forms</h1>
        <hr>
        <h2>User information</h2>
        <p>Names:* 
            <input type="text" required><input="text" name="name" placeholder="Srasti tripathi" required>
        </p>
            <fieldset>
                <legend>Gender</legend> 
                Male<input type="radio" name="gender" id="Male" vale="M" required> Female<input type="radio" names="gender" id="Female">
         </fieldset> 
        </p>
        <p>
            Address:
            <textarea placeholder="Enter your address" name ="address" id="address" cols="100" rows="8" required="enter valid address"></textarea>
        </p>
        <p>
            Email:* 
            <input type="email" name="email" id="email" required placeholder="@ is required">
        </p>
        <p>
            Pincode:
             <input type="number" name="pincode" id="pincode" placeholder="123456">
            </p>
        
        <h2>Payment Information</h2>
        <p>Card Type: 
            <select name="card_type" id="card_type">
                <option value="">--Select a Card Type--</option>
                <option value="visa">Visa</option>
                <option value="rupay">Mastercard</option>
                <option value="mastercard">Rupay</option>
            </select>
        </p>
         <p>
            Card Number: *
            <input type="number" name="card_number" id="card_number" required="enter card number">
         </p>
         <p>
            Expiration Date:* 
            <input type="date" name="exp_date" id="exp_date" required="enter expiry date">
         </p> 
         <p>
            CVV*
            <input type="password" name="CVV" id="CVV" required="cvv number is required">
        </p>
         <input type="submit" value="Pay Now">
        <a href="first.htm">Click here to go second pages</a>
       </form>
       </div> 
        <script>
             function focusFunction(element){
        blur.style.background="lime";
    }
    function blurFunction(element)
        element.style.background="";

    function inputFunction(element){
        var x=element.value;
        document.getElementById("test").innnerHTML=x;
    }
    function changeFunction(){
        var x=element.value;
    }
            function paynowFunction(){
             console.log("You have submitted a form")
             alert("Hello" +x);
            }
            
         </script>
         
</body>
</html>
