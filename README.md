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
