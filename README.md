<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="utf-8" />
	<title>Generar Números Aleatorios dentro de un Rango</title>
	<script type="text/javascript">
	function aleatorio() {
		var min = parseInt(document.getElementById('min').value);
		var max = parseInt(document.getElementById('max').value);
		var res = Math.floor(Math.random() * (max - min + 1)) + min;
		document.getElementById('resultado').innerHTML = res.toString();
	}
	</script>
</head>
<body>
	<form >
		<label for="min">Valor mínimo: </label>
		<input id="min" />
		<label for="max">Valor máximo: </label>
		<input id="max" />
		<input type="button" value="Calcular" onClick="aleatorio();"/>
	</form>
	<p id="resultado"></p>
</body>
</html>
