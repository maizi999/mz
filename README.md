<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>随机抽奖页面</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-image: url('https://source.unsplash.com/1600x900/?background'); /* 替换为你的背景图片链接 */
      background-size: cover;
      color: white;
      margin: 0;
      padding: 0;
    }
    .container {
      padding-top: 15%;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }
    button {
      font-size: 1.5em;
      padding: 10px 20px;
      color: white;
      background-color: #007bff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
    #result {
      margin-top: 20px;
      font-size: 2em;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🎉 随机抽奖 🎉</h1>
    <p>点击按钮生成一个1到100的随机数字</p>
    <button onclick="generateRandom()">开始抽奖</button>
    <div id="result"></div>
  </div>
  <script>
    function generateRandom() {
      const randomNumber = Math.floor(Math.random() * 100) + 1;
      document.getElementById('result').innerText = `抽中的数字是：${randomNumber}`;
    }
  </script>
</body>
</html>
