<!DOCTYPE html>
<html>
	<head>
		<title>Random Number Generator</title>
		<script type="text/javascript">

			function generateRandomNumber(){
				var min = parseInt(document.getElementById('min').value);
				var max = parseInt(document.getElementById('max').value);
				var rand = Math.floor(Math.random() * (max - min + 1)) + min;
				document.getElementById('display').innerText = rand;
			}

		</script>
	</head>
	<body>
	<h2>Random Number Generator </h2>
	<br>
		<label>Min</label>
		<input id="min" name="text"><br>
		<label>Max</label>
		<input id="max" name="text"><br>
		<button onclick="generateRandomNumber();">Generate</button>
		<div id="display" style="font-size: 60px;"></div>
	</body>
</html>
