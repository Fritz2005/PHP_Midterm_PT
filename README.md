‎<!DOCTYPE html>
‎<html>
‎<head>
‎    <title>Registration Form</title>
‎</head>
‎<body>
‎<?php
‎// check if the form is already submitted
‎if ($_SERVER["REQUEST_METHOD"] == "POST") {
‎    // get the data from the form
‎    $firstname = $_POST["firstname"];
‎    $age = $_POST["age"];
‎    $gender = $_POST["gender"];
‎    $motto = $_POST["motto"];
‎
‎    // check if all fields have value
‎    if (!empty($firstname) && !empty($age) && !empty($gender) && !empty($motto)) {
‎        // show the result if all inputs are filled
‎        echo "You are $firstname, a $age-year-old $gender. Your motto in life is: $motto.";
‎    } else {
‎        // show message if some fields are empty
‎        echo "<p style='color:red;'> </p>
‎    
‎
‎
‎<!-- simple registration form -->
‎<form method="POST" action="">
‎    <h2>Registration Form</h2>
‎
‎    <!-- input for first name -->
‎    <label>First Name:</label>
‎    <input type="text" name="firstname" value="Frich"><br><br>
‎
‎    <!-- input for age -->
‎    <label>Age:</label>
‎    <input type="number" name="age" value="20"><br><br>
‎
‎    <!-- dropdown for gender -->
‎    <label>Gender:</label>
‎    <select name="gender">
‎        <option value="">--Select--</option>
‎        <option value="Male" selected>Male</option>
‎        <option value="Female">Female</option>
‎    </select><br><br>
‎
‎    <!-- textarea for quote or motto -->
‎    <label>Quote in Life:</label><br>
‎    <textarea name="motto">Never give up</textarea><br><br>
‎
‎    <!-- button to submit the form -->
‎    <input type="submit" value="Submit">
‎</form>
‎</body>
‎</html>
‎
