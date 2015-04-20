<!doctype html>
<html>
<head>
<title>Teste Javascript</title>
<meta charset="UTF-8"/>
<style>
#nome{
font-family:Agency FB;
color:#333;
}
#barraright{
width:30px;
height:500%;
background:#333;
color:#fff;
position:right;
}
</style>
<script>
var quebrada = false;
function mudaLampada(tipo){
	if (tipo == 1){
		arquivo = "img/lampada-acesa.jpg";
	}
	if (tipo == 2){
		arquivo = "img/lampada-apagada.jpg";
	}
	if (tipo == 3){
		arquivo = "img/lampada-quebrada.jpg";
	}
	if (!quebrada){
	document.getElementById("luz"). src = arquivo;
	if (tipo == 3){
		quebrada = true;
	}
	}
	}
</script>
</head>
<body>
<center>
<label id="nome"><h1>Acenda a lampada</h1></label>
<img src="/img/lampada-apagada.jpg" id="luz" onclick="" onmousemove="mudaLampada(1)" onmouseout="mudaLampada(2)" onclick="mudaLampada(3)"/> 
<div id="barraright">
</div>
</center>
</body>
</html>
