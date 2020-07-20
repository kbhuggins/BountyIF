<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="bountyStyle.css">
    <title>New User Registration</title>
</head>

<style>
 .buttons {
    background-color: white;
    color: black;
    border: 2px solid rgb(115, 185, 133);
    border-radius: 0px;
    height: 80px;
    width: 250px;
    padding: 10px 15px 10px 15px;
    font-size: medium;
    }

.buttons:hover, .existingUserBtn:hover{
    background-color: rgb(157, 250, 180);
    transition-duration: 0.9s;
}

.existingUserBtn{
    background-color: white;
    color: black;
    border: 3px solid rgb(157, 250, 180);
    border-radius: 4px;
    height: 40px;
    width: 160px;
    padding: 10px 15px 10px 15px;
    font-size: medium;
}


.ng-hide {
    height:0;
}

#Charity, #Volunteer, #Restaurant {
    padding-top: 20px;
    transition: all linear 0.5s;
    background-color: white;
    height:350px;
}

#tableDiv {
    width: 75%;
    margin-left: 13%;
}

.parallax, .parallaxHidden {
    /* The image used */
    background-image: url("bountyBgrnd.jpg");
  
    /* Set a specific height */
    height: 500px;
    padding: 50px;
    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }

#pageContent, .charityContentBtn{
    align:center;
    margin-left: 70px;
    width:70%;
    background-color: rgb(219, 255, 228);
    padding: 100px;
}

.topnav {
    background-color: #333;
    overflow: hidden;
  }
  
  /* Style the links inside the navigation bar */
  .topnav a {
    float: left;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 17px;
  }
  
  /* Change the color of links on hover */
  .topnav a:hover {
    background-color: rgb(188, 252, 204);
    color: black;
  }
  
  /* Add a color to the active/current link */
  .topnav a.active {
    background-color: rgb(188, 252, 204);
    color: rgb(82, 104, 87);
  }


a, a:visited {
    text-decoration:none;
    color: black;
}


body {
    font-family: Arial, Helvetica, sans-serif;
}

html{
    scroll-behavior: smooth;
}

table {
    font-family: arial, sans-serif;
    border-collapse: collapse;
    width: 100%;
  }
  
  td, th {
    border: 1px solid  rgb(135, 177, 145);
    text-align: left;
    padding: 8px;
  }
  
  tr:nth-child(even) {
    background-color:  whitesmoke;
  }
</style>
<body>

    <img div class="gallery" src="deliveryStock.jpg" alt="stock1" style="display:block; margin-left:auto; margin-right:auto; width:50%;"> 
    <h2 align="center">Register as a: </h2>

    <div id ="content" align="center">
        <button class="buttons" name="charityBtn" onclick="showCharity()">Charity</button>
        <button class="buttons" name="restaurantBtn" onclick="showRestaurant()">Restaurant</button>
    </div>

    <div id="Existing" align="center">
       <br><br>
        <button class="existingUserBtn" name="existingUserBtn"><a href="logIn.html">Existing User?</a></button>
    </div>

    <div id="Restaurant" align="center" style="display:none;">
      <h3>Restaurant Registration</h3>
        <form action="welcome.php">
            <label for="rName">Restaurant Name: </label>
            <input type="text" id="rName" name="rName"><br><br>
            <label for="rAddress">Address Line 1: </label>
            <input type="text" id="rAddress" name="rAddress"><br><br>
            <label for="rAddress">Address Line 2: </label>
            <input type="text" id="rAddress2" name="rAddress2"><br><br>
            <label for="cityName">City: </label>
            <input type="text" id="cityName" name="cityName"><br><br>
            <label for="state">State: </label>
            <input type="text" id="state" name="state">
            <br style=“height:200px”;><br>
            <input type="submit" value="Submit">
            <input type="reset">
        </form>
    </div>


    <div id="Charity" align="center" style="display:none;">
      <h3>Charity Registration</h3>
        <form action="welcome.php">
            <label for="cName">Charity Name: </label>
            <input type="text" id="cName" name="cName"><br><br>
            <label for="cAddress">Address: </label>
            <input type="text" id="cName" name="cName"><br><br>
            <label for="cAddress2">Address Line 2: </label>
            <input type="text" id="cAddress2" name="cAddress2"><br><br>
            <label for="charityCity">City: </label>
            <input type="text" id="charityCity" name="charityCity"><br><br>
            <label for="cState">State: </label>
            <input type="text" id="cState" name="cState">
            <br style=“height:200px”;><br>
            <input type="submit" value="Submit">
            <input type="reset">
        </form>
    </div>

    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular-animate.js"></script>

    <script type="text/javascript">

      
          function showCharity() {
              var x = document.getElementById("Charity");
              if (x.style.display === "none") {
                x.style.display = "block";
              } else {
                x.style.display = "none";
              }
            }
      

      
            function showRestaurant() {
              var x = document.getElementById("Restaurant");
              if (x.style.display === "none") {
                x.style.display = "block";
              } else {
                x.style.display = "none";
              }
            }
      

     
          function showVolunteer() {
            var x = document.getElementById("Volunteer");
            if (x.style.display === "none") {
              x.style.display = "block";
            } else {
              x.style.display = "none";
            }
          }
        

    </script>
</body>
</html>

