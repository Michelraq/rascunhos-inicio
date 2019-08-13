<!DOCTYPE html>
<html lang="en" dir="ltr">

<head>
    <meta charset="utf 8">
    <title></title>
    <link rel="stylesheet" href="style.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
</head>

<body>
    
    <form action="Login.html" class="login-form">
        <h1>Sistema</h1>
        
        <div class="txtb">
            <input type="text">
            <span data-placeholder="Usuário"></span>
        </div>

        <div class="txtb">
            <input type="password">
            <span data-placeholder="Senha"></span>
        </div>

        <input type="submit" class="logbtn" value="Login">

        <div class="bottom-text">
            Não tem conta? <a href="#">Clique</a>
        </div>
</form>

       <script type="text/javascript">
       $(".text input").on("focus",function(){
        $(this).addClass("focus");
       });

       $(".text input").on("blur",function(){
       if ($(this).val()=="")
       $(this).removeClass("focus");
       });
       </script>
       
</body>
</html>
{
margin:0;
padding:0;
text decoration:none;
font-family:montsserrat;
box sizing:border-box;
}

body{
min-height: 100vh;
background-image:linear-gradient(#01c5cce1,#01c5cce1);
}

.login-form{
  background: #7b9bb9e1;
  height: 330px;
  padding: 30px 30 px;
  border-radius:20px;
  position:absolute;
  left:35%;
  top:30%;
  transform:translate(-20%-20%);
}

.login-form h1{
text-align: center;
margin-bottom: 10px;
}

.txtb{                                
border-bottom:2px  solid rgb(7, 6, 6);
position:relative;
margin: 30px 0;
}

.txtb input{
font-size: 30px;
color: rgb(2, 14, 15);
border:white;
width: 97%;
outline: wheat;
background: white;
padding: 0 5px;
height: 40px;
}

.txtb span::before{
  content: attr(data-placeholder);
  position:absolute;
  top:30%;
  left:0px;
  color: rgb(12, 3, 3);
  transform: translateY(-200%);
  
}

.txtb span::after{
content: "";
position: absolute;
width: 0%;
height: 2px;
background:linear-gradient(120deg,#b1cadb,#d3c4da);
transition: .5s;
}

.focus+span::before{
  top:-5px;
}
.focus+span::after{
  width: 100%;
}
