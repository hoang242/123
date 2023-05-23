<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Đổi màu nền</title>
    <style>
      body {
        background-color: pink;
        transition: background-color 0.5s ease;
      }

      button {
        padding: 10px 20px;
        font-size: 16px;
        background-color: #4CAF50;
        color: white;
        border: none;
        cursor: pointer;
        border-radius: 4px;
        transition: background-color 0.5s ease;
      }

      button:hover {
        background-color: #3e8e41;
      }
    </style>
  </head>
  <body>
    <h1>Đổi màu nền</h1>
    <button onclick="changeBackgroundColor()">Click để đổi màu</button>

    <script>
      function changeBackgroundColor() {
        let backgroundColor = document.body.style.backgroundColor;
        if (backgroundColor === "pink") {
          document.body.style.backgroundColor = "blue";
        } else {
          document.body.style.backgroundColor = "pink";
        }
      }
    </script>
  </body>
</html>
