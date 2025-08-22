   <!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Xác minh robot</title>
  <style>
    body { font-family: Arial; display: flex; justify-content: center; align-items: center; height: 100vh; }
    .box { border: 1px solid #ccc; padding: 30px; border-radius: 10px; box-shadow: 0 0 10px #ddd; text-align: center; }
    input[type="text"] { width: 40px; padding: 5px; text-align: center; }
    button { padding: 10px 20px; margin-top: 10px; }
    #continue-btn { display: none; background: #28a745; color: white; }
  </style>
</head>
<body>
  <div class="box">
    <h3>XÁC MINH ROBOT 🤖</h3>
    <p>1 + 1 = <input id="answer" type="text"></p>
    <button onclick="verify()">XÁC MINH</button>
    <div id="success" style="display:none; color:green;">✅ Xác minh thành công!</div>
    <button id="continue-btn" onclick="redirect()">TIẾP TỤC</button>
  </div>

  <script>
    function verify() {
      var val = document.getElementById("answer").value;
      if (val == "2") {
        document.getElementById("success").style.display = "block";
        document.getElementById("continue-btn").style.display = "inline-block";
      } else {
        alert("Sai rồi, hãy thử lại!");
      }
    }

    function redirect() {
      window.location.href = "https://baosting79.top";
    }
  </script>
</body>
</html>
