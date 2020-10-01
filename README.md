<!DOCTYPE html>
<html lang="en">

<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Calculator using JavaScript</title>
	<style>
		* {
			margin: 0;
			padding: 0;
			box-sizing: border-box;

		}

		body {
			display: flex;
			justify-content: center;
			align-items: center;
			min-height: 100vh;
			background-color: rgb(28, 28, 61);
		}
		.calculator{
			position: relative;
			display: grid;


		}
		.calculator .value{
			grid-column: span 4;
			height: 100px;
			text-align: right;
			border: none;
			outline: none;
			padding: 10px;
			font-size: 18px;
			background-color: aquamarine;

		}
		.calculator span{
			display: grid;
			height: 60px;
			width: 60px;
			color: white;
			background-color:#0c2835;
		    place-items: center;
			border: 1px solid rgba(0, 0,0, .1);
		}
		.calculator span:active{
			background-color: #74ff3b;
			color: #111;
		}
		.calculator span.clear{
			grid-column: span 2;
		    width: 120px;
			background-color:#ff3077;
		}
		.calculator span.plus{
			grid-row: span 2;
			height: 120px;
		}
		.calculator span.equal{
			background:#03b1ff;

		}

	</style>
</head>

<body>
	<form class="calculator" name="calc">
		<input class="value" type="text" name="text" readonly="">
		<span class="num clear" onclick="document.calc.text.value =''">c</span>
		<span class="num" onclick="document.calc.text.value +='/'">/</span>
		<span class="num" onclick="document.calc.text.value +='*'">*</span>
		<span class="num" onclick="document.calc.text.value +='7'">7</span>
		<span class="num" onclick="document.calc.text.value +='8'">8</span>
		<span class="num" onclick="document.calc.text.value +='9'">9</span>
		<span class="num" onclick="document.calc.text.value +='-'">-</span>
		<span class="num" onclick="document.calc.text.value +='4'">4</span>
		<span class="num" onclick="document.calc.text.value +='5'">5</span>
		<span class="num" onclick="document.calc.text.value +='6'">6</span>
		<span class="num plus" onclick="document.calc.text.value +='+'">+</span>
		<span class="num" onclick="document.calc.text.value +='3'">3</span>
		<span class="num" onclick="document.calc.text.value +='2'">2</span>
		<span class="num" onclick="document.calc.text.value +='1'">1</span>
		<span class="num" onclick="document.calc.text.value +='0'">0</span>
		<span class="num" onclick="document.calc.text.value +='00'">00</span>
		<span class="num" onclick="document.calc.text.value +='.'">.</span>
		<span class="num equal" onclick="document.calc.text.value =eval(calc.text.value)">=</span>


	</form>

</body>

</html>
