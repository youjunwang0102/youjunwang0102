<!DOCTYPE html>
<html>
<head>
    <title>Login Page</title>
</head>
<body>
    <h1>Login</h1>
    <form id="loginForm">
        <label for="username">帳號:</label>
        <input type="text" id="username" name="username" required><br><br>
        <label for="password">密碼:</label>
        <input type="password" id="password" name="password" required><br><br>
        <button type="button" onclick="checkLogin()">登入</button>
    </form>

    <p id="message"></p>

    <script>
        function checkLogin() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            if (username === "teacher123" && password === "123teacher") {
                window.location.href = 'https://sites.google.com/view/lrmc/%E9%A6%96%E9%A0%81';
            } else {
                document.getElementById("message").textContent = "帳號或密碼不正確。";
            }
        }
    </script>
</body>
</html>
