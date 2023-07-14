```html
<!DOCTYPE html>
<html>
<head>
  <title>Random Color on Mouse Move</title>
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      font-size: 24px;
      color: white;
    }
  </style>
</head>
<body>
  <script>
    document.addEventListener('mousemove', function(event) {
      var color = getRandomColor();
      document.body.style.backgroundColor = color;
    });

    function getRandomColor() {
      var letters = '0123456789ABCDEF';
      var color = '#';
      for (var i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
  </script>
  <h1>Move your mouse to change the background color!</h1>
</body>
</html>
```
<img width="889" alt="image" src="https://github.com/KrisanapongJaruenjanporn/Move_mouse_change_backgroun/assets/121858059/5e9a19dd-debe-4949-84e7-0742560a75e8">

