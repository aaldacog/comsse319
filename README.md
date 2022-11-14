# comsse319
Construction of User Interfaces
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Here it start my Tutorial</title>
</head>
<body>
    <h1>HTML Tutorial</h1>
    
    <h2>JavaScript Geolocation</h2>

    <p>Click the button to get your coordinates.</p>

    <button onclick="getLocation()">Try It</button>
    
    
    <p id="demo"></p>

    <script>
    const x = document.getElementById("demo");

    function getLocation() {
      try {
        navigator.geolocation.getCurrentPosition(showPosition);
      } catch {
        x.innerHTML = err;
      }
    }

    function showPosition(position) {
      x.innerHTML = "Latitude: " + position.coords.latitude + 
      "<br>Longitude: " + position.coords.longitude;
    }
    </script>
    
</body>
</html>
