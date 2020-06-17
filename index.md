<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device width, initial-scale=1">
	<title>Interface Cormiers</title>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
	<link rel="stylesheet" type="text/css" href="style.css">
	<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
	<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.0/jquery.min.js"></script>

	

</head>

<body>
	<div class="row justify-content-center">
		<div class="divmar">
			<div class="grid-container1">
				<div class="grid-div0 grid-cursor" id="ic1"><img class="itsize1" src="Images/b40.jpg"></div>
				<div class="grid-div1 grid-cursor" id="ic2"><img class="itsize1" src="Images/b39.jpg"></div>
				<div class="grid-div1 grid-cursor" id="ic3"><img class="itsize1" src="Images/b38.jpg"></div>
				<div class="grid-div1 grid-cursor" id="ic4"><img class="itsize1" src="Images/b41.jpg"></div>
				<div class="blank1 grid-div1"></div>
				<div class="grid-div1 grid-cursor" id="mode1" data-value="on"><img class="itsize1" id="imgm1" src="Images/b03.jpg"></div>
				<div class="grid-div1 grid-cursor" id="mode2" data-value="off"><img class="itsize1" id="imgm2" src="Images/b02.jpg"></div>
				<div class="grid-div1 grid-cursor" id="mode3" data-value="off"><img class="itsize1" id="imgm3" src="Images/b01.jpg"></div>
				<div class="blank2 grid-div2"></div>
				<div class="grid-ti" id="title"><img class="itsize2" src="Images/bin5.jpg"></div>
				<div class="grid-mode texts grid-div3" id="modev">Mode manuel</div>
			</div>
			<div class="grid-container2">
				<div class="grid-div1 grid-cursor" id="btn1" data-value="off"><img class="itsize1" id="img1" src="Images/b24.jpg"></div>
				<div class="grid-div1" id="btn3"><img class="itsize1" id="img3" src="Images/b06.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn4"><img class="itsize1" src="Images/b34.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn5" data-value="disr"><img class="itsize1" id="img5" src="Images/b59.jpg"></div>
				<div class="grid-div1" id="btn7"><img class="itsize1" id="img7" src="Images/b14.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn8"><img class="itsize1" src="Images/b33.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn9" data-value="dis0"><img class="itsize1" id="img9" src="Images/b61.jpg"></div>
				<div class="grid-bar grid-div4" id="btn10"><img class="itsize3" src="Images/bin4.jpg"></div>
				<div class="grid-div1" id="btn11"><img class="itsize1" id="img11" src="Images/b18.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn12"><img class="itsize1" src="Images/b35.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn13" data-value="col"><img class="itsize1" id="img13" src="Images/b26.jpg"></div>
				<div class="grid-div1" id="btn14"></div>
				<div class="grid-div1 grid-cursor" id="btn15"><img class="itsize1" id="img15" src="Images/b30.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn16"><img class="itsize1" id="img16" src="Images/b31.jpg"></div>
				<div class="grid-div1 grid-cursor" id="btn17"><img class="itsize1" id="img17" src="Images/b32.jpg"></div>
				<div class="grid-div1" id="btn18"></div>
				<div class="grid-div1" id="btn19"><img class="itsize1" id="img19" src="Images/b09.jpg"></div>
				<div class="grid-off grid-div1 grid-cursor" id="btn20"><img class="itsize1" src="Images/b36.jpg"></div>
				<div class="itemscreen grid-div1" id="screen"><img class="itsize4" id="imscreen" src="Images/bin6.jpg"></div>
			</div>
		</div>
	</div>

</body>
</html>

<script>
	$(document).ready(function(){
		$('#btn1').click(function(){
			var value = document.getElementById('btn1').getAttribute('data-value');
			var value2 = document.getElementById('btn5').getAttribute('data-value');
			if (value == "off") {
				$('#img1').attr('src','Images/b23.jpg');
				document.getElementById('btn1').setAttribute('data-value','on');
				if (value2 == "disr") {
					$('#img5').attr('src','Images/b19.jpg');
					document.getElementById('btn5').setAttribute('data-value','r');
				} else {
					$('#img5').attr('src','Images/b20.jpg');
					document.getElementById('btn5').setAttribute('data-value','l');
				}	
				$('#img9').attr('src','Images/b22.jpg');
				document.getElementById('btn9').setAttribute('data-value','0');
			} else {
				$('#img1').attr('src','Images/b24.jpg');
				document.getElementById('btn1').setAttribute('data-value','off');
				if (value2 == "r") {
					$('#img5').attr('src','Images/b59.jpg');
					document.getElementById('btn5').setAttribute('data-value','disr');
				} else {
					$('#img5').attr('src','Images/b60.jpg');
					document.getElementById('btn5').setAttribute('data-value','disl');
				}	
				$('#img9').attr('src','Images/b61.jpg');
				document.getElementById('btn9').setAttribute('data-value','dis0');
			}
		});

		$('#btn5').click(function(){
			var value = document.getElementById('btn5').getAttribute('data-value');
			if (value == "r") {
				$('#img5').attr('src','Images/b20.jpg');
				document.getElementById('btn5').setAttribute('data-value','l');
			} else {
				$('#img5').attr('src','Images/b19.jpg');
				document.getElementById('btn5').setAttribute('data-value','r');
			}
		});

		$('#btn13').click(function(){
			var value = document.getElementById('btn13').getAttribute('data-value');
			if (value == "col") {
				$('#img13').attr('src','Images/b27.jpg');
				$('#imscreen').attr('src','Images/bin7.jpg');
				document.getElementById('btn13').setAttribute('data-value','blk');
			} else {
				$('#img13').attr('src','Images/b26.jpg');
				$('#imscreen').attr('src','Images/bin6.jpg');
				document.getElementById('btn13').setAttribute('data-value','col');
			}
		});

		$('#mode1').click(function(){
			var value = document.getElementById('mode1').getAttribute('data-value');
			if (value == "off") {
				$('#imgm1').attr('src','Images/b03.jpg');
				$('#imgm2').attr('src','Images/b02.jpg');
				$('#imgm3').attr('src','Images/b01.jpg');
				$('#modev').text('Mode manuel');
				document.getElementById('mode1').setAttribute('data-value','on');
				document.getElementById('mode2').setAttribute('data-value','off');
				document.getElementById('mode3').setAttribute('data-value','off');
			}
		});

		$('#mode2').click(function(){
			var value = document.getElementById('mode2').getAttribute('data-value');
			if (value == "off") {
				$('#imgm1').attr('src','Images/b00.jpg');
				$('#imgm2').attr('src','Images/b05.jpg');
				$('#imgm3').attr('src','Images/b01.jpg');
				$('#modev').text('Mode caméra');
				document.getElementById('mode1').setAttribute('data-value','off');
				document.getElementById('mode2').setAttribute('data-value','on');
				document.getElementById('mode3').setAttribute('data-value','off');
			} else {
				$('#imgm1').attr('src','Images/b03.jpg');
				$('#imgm2').attr('src','Images/b02.jpg');
				$('#imgm3').attr('src','Images/b01.jpg');
				$('#modev').text('Mode manuel');
				document.getElementById('mode1').setAttribute('data-value','on');
				document.getElementById('mode2').setAttribute('data-value','off');
				document.getElementById('mode3').setAttribute('data-value','off');
			}
		});

		$('#mode3').click(function(){
			var value = document.getElementById('mode3').getAttribute('data-value');
			if (value == "off") {
				$('#imgm1').attr('src','Images/b00.jpg');
				$('#imgm2').attr('src','Images/b02.jpg');
				$('#imgm3').attr('src','Images/b04.jpg');
				$('#modev').text('Mode palpeur');
				document.getElementById('mode1').setAttribute('data-value','off');
				document.getElementById('mode2').setAttribute('data-value','off');
				document.getElementById('mode3').setAttribute('data-value','on');
			} else {
				$('#imgm1').attr('src','Images/b03.jpg');
				$('#imgm2').attr('src','Images/b02.jpg');
				$('#imgm3').attr('src','Images/b01.jpg');
				$('#modev').text('Mode manuel');
				document.getElementById('mode1').setAttribute('data-value','on');
				document.getElementById('mode2').setAttribute('data-value','off');
				document.getElementById('mode3').setAttribute('data-value','off');
			}
		});

		$('#ic3').click(function(){
			window.open('cam.html','_self');
		});

	});
</script>
