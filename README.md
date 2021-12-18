<html>
	<head>
		<script src='https://cdn.rawgit.com/BrainJS/brain.js/master/browser.js'></script>
	</head>

	<body>

	<h1>Resultado</h1>
	<div id='salida'>
		xxxx
	</div>

	<script>
		/* Red */
		var net = new brain.recurrent.LSTMTimeStep();

	
		/* Entrenamiento */
		net.train( [
			[1,2,3,4,5],
			[6,7,8,9,10],
			[11,12,13,14,15],
			] );

		/* Predicción */
		var result=net.run( [1,2,3] );
		document.getElementById( "salida" ).innerHTML=result;
	</script>

	</body>
</html>

