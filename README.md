<!DOCTYPE html>
<html>
<head>
  <title>Loading</title>
<link rel="stylesheet" href="main.css">
</head>

<body>
<div id="myProgress">
  <div id="myBar">10%</div>
</div>

<br>
<button onclick="move()">Click Me</button>
<script>
function move() {
    var elem = document.getElementById("myBar");
    var width = 10;
    var id = setInterval(frame, 10);
    function frame() {
        if (width >= 100) {
            window.location = "https://itk.ac.id/";
        } else {
            width++;
            elem.style.width = width + '%';
            elem.innerHTML = width * 1 + '%';
        }
    }
}
</script>
</body>
</html>
