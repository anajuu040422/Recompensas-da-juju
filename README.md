<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Recompensas da Juju</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff8f2;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    .container {
      padding: 30px;
    }
    h1 {
      color: #ff66b2;
    }
    input {
      margin: 10px 0;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      width: 80%;
    }
    button {
      background-color: #ff66b2;
      color: white;
      border: none;
      border-radius: 8px;
      padding: 12px 24px;
      font-size: 16px;
      cursor: pointer;
      margin-top: 10px;
    }
    .painel {
      margin-top: 30px;
      background: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 0 10px #eee;
    }
    .link {
      margin-top: 15px;
      display: block;
      font-size: 14px;
      color: #ff66b2;
      text-decoration: underline;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🎀 Recompensas da Juju 🎀</h1>

    <div id="cadastro">
      <input type="text" id="nome" placeholder="Seu nome" /><br />
      <input type="password" id="senha" placeholder="Sua senha" /><br />
      <input type="text" id="pix" placeholder="Sua chave Pix" /><br />
      <button onclick="criarConta()">Criar Conta</button>
      <a class="link" onclick="mostrarRegrinhas()">📜 Regrinhas do jogo da Juju</a>
    </div>

    <div id="painel" style="display: none;">
      <h2>Bem-vindo, <span id="usuarioNome"></span>!</h2>
      <p>Saldo de moedas: <strong><span id="saldo">0</span></strong></p>
      <button onclick="ganharMoedas()">Ganhar moedas</button><br />
      <button onclick="assistirVideo()">Assistir vídeo 🎬</button><br />
      <button onclick="sacarPix()">Sacar via Pix</button>
    </div>

    <div id="regrinhas" style="display: none;">
      <h2>📜 Regrinhas do jogo da Juju</h2>
      <p>Seja gentil, jogue limpo e não use bots! 💖</p>
      <p>Acumule moedas e troque por prêmios reais via Pix.</p>
      <p>Se trapace
