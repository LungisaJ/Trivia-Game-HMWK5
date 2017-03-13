<!DOCTYPE html>

<html lang="en-us">

<head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

    
    <title>Trivia Game</title>

    <link rel="stylesheet" type="text/css" href="Triviagame.css">

	<script src="http://code.jquery.com/jquery-2.1.3.min.js"></script>

    <script type="text/javascript">
	</script>
</head>

<body>
<div id="container">




<p>Main content</p>


<div class="header"><strong>Totally Trivial Trivia!<strong>
<br>

	<div id="main">

		<button class= "button">START</button>

		<br>
		

<!--Timer function here-->
Time Remaining: <p id="time"></p> Seconds

<div class= "questions">

	<h2>Which country is Nelson Mandela from? </h2>
		<input type="radio">South Africa
		<input type="radio"> Ghana
		<input type="radio">Mozambique
		<input type="radio">Botswana

	<h2><strong>How long was Nelson Mandela in prison?</strong></h2>
		<input type="radio">27 years
		<input type="radio">7 years
		<input type="radio">27 months
		<input type="radio">From age 27 to age 72

	<h2>Which one of the 11 official South African languages was Mandela mother tongue?</h2>
		<input type="radio">Zulu
		<input type="radio">Xhosa
		<input type="radio">Twsana
		<input type="radio">Ndebele

		</div>


	</div>

</div>

		<script>
		var input = $( "form input:radio" )
  		.wrap( "<span></span>" )
  		.parent()
    	.css({
      		background: "yellow",
      		border: "3px red solid"
    });

 }
var countDownDate = new Date(" 00:00:59").getTime();

var x = setInterval(function() {

	var now = new Date().getTime();
	var distance = countDownTime - now;
	var seconds = Math.floor((distance % (1000 * 60)) / 1000);

document.getElementById("time").innerHTML = seconds + "s ";
});
}

 <button onClick="clearInterval(myTimer)">Stop counter!</button>
		</script>

</body>

   	<footer>
		<script src="file:///C:/Users/Lungisa/Desktop/Homework/HMWK5\Triviagame.css"></script>
 	</footer>
 

  <link rel="stylesheet" href="./Triviagame_files/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<!-- Optional theme -->
<link rel="stylesheet" href="./Triviagame_files/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

<!-- Latest compiled and minified JavaScript -->
<script src="Triviagame_files/bootstrap.min.js.download" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous">
  
</script>

</body>

</html>
