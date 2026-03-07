<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>

body{
    margin:0;
    min-height:100vh;
    display:flex;
    flex-direction:column;
    overflow-x:hidden;
}

/* contenedor principal */
.escena{
    position: relative;
    width: 100%;
    max-width: 1920px;
    margin: auto;
    flex:1;
}

/* imagen base */
.fondo{
    width:100%;
    display:block;
}

/* elemento encima del fondo */
.objeto{
    position:absolute;
    top:40%;
    left:30%;
    transform: translate(-50%, -50%);
}

/* footer */
footer{
    width:100%;
    background:#2b2b2b;
    color:white;
    text-align:center;
    padding:12px;
    font-family:Arial, sans-serif;
    font-size:14px;
}

/* texto animado */
.footer-text{
    display:inline-block;
    transition: 
        transform 0.7s ease,
        opacity 0.7s ease,
        filter 0.7s ease;
}

/* efecto humo */
.footer-text:hover{
    transform: scale(1.8);
    opacity:0;
    filter: blur(10px);
}

</style>
</head>

<body>

<div class="escena">

    <img src="pic.jpeg" class="fondo">

    <!-- elemento encima -->
    <img src="boton.png" class="objeto">

</div>

<footer>
    <span class="footer-text">@@ ™ - All rights reserved.</span>
</footer>

</body>
</html>
