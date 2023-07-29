<!DOCTYPE html>
<meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">  
  <style>
    body {
      margin: 0;
      padding: 0;
      overflow: hidden;
    }
    #video-background {
      position: fixed;
      top: 0;
      left: 0;
      width: 119%;
      height: 100%;
      z-index: -1;
    }
    #content {
      position: relative;
      z-index: 1;
      text-align: center;
      padding: 20px;
      color: #fff;
    }
  </style>
</head>
<body>
  <video id="video-background" autoplay muted loop>
    <source src="1.mp4" type="video/mp4">
  </video>
  <div id="content">
  </div>
</body>
</html>
  <video id="v3" width="222" src=""> 
  </video> 
  <audio src="她.mp3"  autoplay="" loop=""></audio>
<html>
<head>
  <title>密码界面</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }
    .container {
      max-width: 400px;
      margin: 0 auto;
      padding: 50px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .input-group {
      margin-bottom: 10px;
    }
    .input-group label {
      display: block;
      margin-bottom: 5px;
    }
    .input-group input[type="password"] {
      width: 100%;
      padding: 5px;
      border: 1px solid #ccc;
      border-radius: 3px;
    }
    .input-group button {
      padding: 5px 10px;
      background-color: #4caf50;
      color: #fff1;
      border: none;
      border-radius: 3px;
      cursor: pointer;
    }
    .input-group button:hover {
      background-color: #45a049;
    }
    .error-message {
      color: red;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>卡密</h2>
    <div class="input-group">
      <label for="password">卡密:</label>
      <input type="password" id="password" placeholder="请输入卡密">
    </div>
    <div class="input-group">
      <button id="login-button" >登录</button>
    </div>
    <div id="error-message" class="error-message"></div>
  </div>

  <script >
    document.getElementById("login-button").addEventListener("click", function() {
      var password = document.getElementById("password").value;
      if (password === "520CY") {
        //密码正确时，跳转下一个界面
          window.location.href="1.html"
        alert("登录成功！");
      } else {
        document.getElementById("error-message").innerHTML = "密码错误，请重试。";
      }
    });
  </script>
</body>
</html>
