<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Finalizar Compra | GlowMist</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0; padding: 0;
      background: #f9f9fb;
      color: #333;
    }
    header {
      background: #f48fb1;
      padding: 20px;
      text-align: center;
      color: #fff;
    }
    header h1 {
      margin: 0;
      font-weight: 700;
      font-size: 2rem;
    }
    main {
      max-width: 500px;
      margin: 40px auto;
      background: #fff;
      padding: 30px 25px;
      border-radius: 12px;
      box-shadow: 0 10px 20px rgba(244, 143, 177, 0.2);
    }
    h2 {
      color: #f48fb1;
      margin-bottom: 25px;
      font-weight: 700;
      text-align: center;
    }
    form label {
      display: block;
      margin-bottom: 8px;
      font-weight: 600;
      color: #555;
    }
    form input, form select {
      width: 100%;
      padding: 12px 10px;
      margin-bottom: 20px;
      border: 2px solid #f48fb1;
      border-radius: 8px;
      font-size: 1rem;
      outline: none;
      transition: border-color 0.3s ease;
    }
    form input:focus, form select:focus {
      border-color: #d81b60;
    }
    .price-summary {
      font-size: 1.3rem;
      font-weight: 700;
      margin-bottom: 25px;
      text-align: center;
      color: #d81b60;
    }
    button {
      width: 100%;
      padding: 15px;
      background: #f48fb1;
      color: white;
      font-weight: 700;
      font-size: 1.2rem;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #d81b60;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: #f48fb1;
      color: #fff;
      font-weight: 600;
      margin-top: 50px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Finalize sua compra</h1>
  </header>

  <main>
    <h2>GlowMist — Mini Nebulizador Facial</h2>
    <p class="price-summary">Preço: R$ 29,90</p>

    <form id="checkoutForm">
      <label for="name">Nome completo</label>
      <input type="text" id="name" name="name" required placeholder="Seu nome completo" />

      <label for="email">E-mail</label>
      <input type="email" id="email" name="email" required placeholder="seu@email.com" />

      <label for="address">Endereço para entrega</label>
      <input type="text" id="address" name="address" required placeholder="Rua, número, bairro, cidade" />

      <label for="payment">Forma de pagamento</label>
      <select id="payment" name="payment" required>
        <option value="" disabled selected>Escolha uma opção</option>
        <option value="cartao">Cartão de crédito</option>
        <option value="boleto">Boleto bancário</option>
        <option value="pix">Pix</option>
      </select>

      <button type="submit">Finalizar Compra</button>
    </form>
  </main>

  <footer>
    © 2025 GlowMist. Todos os direitos reservados.
  </footer>

  <script>
    document.getElementById('checkoutForm').addEventListener('submit', function(e) {
      e.preventDefault();
      alert('Compra finalizada com sucesso! Em breve entraremos em contato pelo seu e-mail.');
      // Aqui você pode adicionar integração com sistema real de pagamentos ou redirecionar
      window.location.href = 'index.html';
    });
  </script>
</body>
</html>
