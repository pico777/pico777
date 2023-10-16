<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Camera</title> <script type="text/javascript" src="https://unpkg.com/webcam-easy/dist/webcam-easy.min.js"></script>

<style>

a {

padding: 10px;

background-color: orange;

color: white;

text-decoration: none;

}

</style>

</head>

<body>

<video id="webCam" autoplay playsinine width="800" height="600"></video>

<canvas id="canvas"></canvas>

<a download>SNAP</a>

<script>

const webCamElement = document.getElementById("webCam");

const canvasElement = document.getElementById("canvas");

const webcam = new Webcam(webCamElement, "user", canvasElement); webcam.start();

</script>

</body>

</html>
