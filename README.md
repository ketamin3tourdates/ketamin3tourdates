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
    position:relative;

    background-image: url("RECURSOS/Fondo WEB.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

/* LOGO TITULO */
.logo{
    width:320px;
    height:auto;
    margin:30px auto 10px auto;
    display:block;

    transition: transform 0.3s ease;
}

.logo:hover{
    transform: scale(1.15);
}

/* contenedor principal */
.escena{
    position: relative;
    width:100%;
    max-width:1920px;
    margin:auto;
    flex:1;
}

/* SOL detrás del pasto */
.sol{
    position:absolute;
    bottom:160px;
    left:50%;
    transform:translateX(-50%);
    width:350px;
    height:auto;
    z-index:0;
}

/* contenedor del pasto */
.pasto-contenedor{
    position:relative;
    width:100%;
    height:150px;
    overflow:hidden;
    z-index:2;
}

/* imagen del pasto */
.pasto{
    width:100%;
    height:auto;
    display:block;
}

/* stickmans sobre el pasto */
.stickmans{
    position:absolute;
    bottom:10px;
    left:50%;
    transform:translateX(-50%) scaleX(1.5);
    transform-origin:center bottom;
    width:250px;
    height:auto;
    z-index:5;
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

<a href="https://www.instagram.com/shako2b/" target="_blank">
    <img src="RECURSOS/SHAKO logo.png" class="logo">
</a>

<div class="escena"></div>

<img src="RECURSOS/Sol.png" class="sol">

<div class="pasto-contenedor">

    <img src="RECURSOS/Pasto.png" class="pasto">

    <img src="RECURSOS/Stickmans.png" class="stickmans">

</div>

<footer>
<span class="footer-text">@@ ™ - All rights reserved.</span>
</footer>

</body>
</html>
