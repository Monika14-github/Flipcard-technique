# Flipcard-technique
.....html......
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="wrap">
		<div class="side-a"></div>
		<div class="side-b"></div>
	</div>
  </body>
</html>
.....css.....
body {
	padding-top: 100px;
	background: rgb(6, 98, 121)
}
.wrap {
	position: relative;
	margin: 0 auto;
	width: 250px;
	height: 350px;
	cursor: pointer;
}
.wrap div {
	width: 100%;
	height: 100%;
	border-radius: 10px;
	background-position: 50% 50%;
	background-size: 250px;
	background-repeat: no-repeat;
	box-shadow: inset 0 0 45px rgba(22, 183, 189, 0.3), 0 12px 20px -10px rgba(121, 8, 93, 0.4);
	color: rgb(19, 158, 42);
	text-align: center;
	text-shadow: 0 1px rgba(32, 2, 2, 0.3);
	font: bold 3em sans-serif;
	line-height: 350px;
}
.side-a {
	background: rgb(219, 213, 213) url(https://tse1.mm.bing.net/th?id=OIP.fEdll0qAVAZWt1yvxC6yFAAAAA&pid=Api&P=0&w=300&h=300);
}
.side-b {
	background: rgba(12, 18, 31, 0.712) url(https://tse2.mm.bing.net/th?id=OIP.spvtEnHGNxKpLn8GABSQFQHaLA&pid=Api&P=0&w=300&h=300);
}
body {
	-webkit-perspective: 800px;
}

.wrap {
	transition: -webkit-transform 1s ease-in;
	-webkit-transform-style: preserve-3d;
}

.wrap div {
	position: absolute;
	-webkit-backface-visibility: hidden;
}

.side-a {
	z-index: 100;
}
.side-b {
	-webkit-transform: rotateY(-250deg);
}
.wrap:hover {
	-webkit-transform: rotateY(250deg);
}
