<!DOCTYPE html>
<html>
<head>
<title>Library Management System</title>

<style>
body{
    font-family: Arial;
    background:#f2f2f2;
}

.container{
    width:400px;
    margin:120px auto;
    padding:30px;
    background:white;
    border:2px solid #000;
    text-align:center;
}

h2{
    margin-bottom:30px;
}

.row{
    margin:15px 0;
}

label{
    display:inline-block;
    width:100px;
    text-align:left;
}

input{
    padding:8px;
    width:200px;
    border:2px solid black;
}

button{
    padding:10px 30px;
    margin:20px 10px;
    border:none;
    background:linear-gradient(#6fa8dc,#3d85c6);
    color:white;
    font-size:16px;
    border-radius:6px;
    cursor:pointer;
}

button:hover{
    background:#2b6cb0;
}

.top-links{
    display:flex;
    justify-content:space-between;
    margin-bottom:20px;
}

.top-links a{
    color:blue;
    text-decoration:underline;
    cursor:pointer;
}
</style>

<script>

function login(){
    var user=document.getElementById("userid").value;
    var pass=document.getElementById("password").value;

    if(user=="adm" && pass=="adm"){
        alert("Login Successful");
    }
    else{
        alert("Invalid User ID or Password");
    }
}

function cancel(){
    document.getElementById("userid").value="";
    document.getElementById("password").value="";
}

</script>

</head>

<body>

<div class="container">

<div class="top-links">
<a href="#">Chart</a>
<a href="#">Back</a>
</div>

<h2>Library Management System</h2>

<div class="row">
<label>User ID</label>
<input type="text" id="userid" value="adm">
</div>

<div class="row">
<label>Password</label>
<input type="password" id="password" value="adm">
</div>

<div>
<button onclick="cancel()">Cancel</button>
<button onclick="login()">Login</button>
</div>

</div>

</body>
</html>
