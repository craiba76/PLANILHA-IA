<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Login</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f5f7fa;
      margin: 0;
      padding: 40px;
      color: #333;
    }
    h1 {
      text-align: center;
      color: #004080;
      margin-bottom: 30px;
    }
    .login-container {
      width: 300px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }
    .login-container input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .login-btn {
      width: 100%;
      padding: 10px;
      background-color: #004080;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .login-btn:hover {
      background-color: #003060;
    }
    .error-msg {
      color: red;
      text-align: center;
      margin-top: 10px;
    }
    .welcome-msg {
      text-align: center;
      font-size: 24px;
      color: #004080;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <!-- Login Form -->
  <div class="login-container" id="loginForm">
    <h2>Login</h2>
    <input type="text" id="username" placeholder="Usuário" />
    <input type="password" id="password" placeholder="Senha" />
    <button class="login-btn" onclick="login()">Entrar</button>
    <div class="error-msg" id="errorMsg"></div>
  </div>

  <!-- Boas-Vindas após o login -->
  <div class="welcome-msg" id="welcomeContainer" style="display: none;">
    <p>Seja Bem-Vindo à Planilha Inteligente com IA em 5D!</p>
  </div>

  <script>
    function login() {
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;
      const errorMsg = document.getElementById('errorMsg');

      if (username === "admin" && password === "1005") {
        document.getElementById('loginForm').style.display = 'none';
        document.getElementById('welcomeContainer').style.display = 'block';
      } else {
        errorMsg.textContent = 'Credenciais inválidas. Tente novamente.';
      }
    }
  </script>

</body>
</html>


    // Adiciona eventos para todas as linhas existentes após o carregamento
    document.querySelectorAll('#priceTable tbody tr').forEach(row => aplicarEventos(row));
  </script>

</body>
</html>
