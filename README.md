<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tellink Telecom</title>
    <link rel="stylesheet" href="/style.css">
    <meta name="description" content="Internet de alta velocidade para sua casa ou empresa">
</head>
<body>
    <header>
        <div class="logo">TELLINK <span>TELECOM</span></div>
        <nav>
            <a href="#planos">Planos</a>
            <a href="#contato">Contato</a>
            <a href="https://wa.me/5583981286950" class="whatsapp">Fale Conosco</a>
        </nav>
    </header>
    
    <main>
        <section class="hero">
            <h1>Conectando você ao futuro</h1>
            <p>Internet de alta velocidade para sua casa ou empresa</p>
            <a href="https://wa.me/5583981286950" class="btn">Assine pelo WhatsApp</a>
        </section>

        <section class="planos" id="planos">
            <h2>Nossos Planos de Internet</h2>
            <div class="cards">
                <!-- Todos os planos aqui (conforme seu código original) -->
            </div>
        </section>
    </main>

    <footer id="contato">
        <p>© 2023 Tellink Telecom | Termos de Uso | Política de Privacidade</p>
    </footer>
</body>
</html>
:root {
    --primary: #b30000;
    --secondary: #c0392b;
    --whatsapp: #25D366;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    color: #333;
}

/* [Todos os outros estilos do seu CSS original] */

/* Responsividade */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        text-align: center;
    }
    
    nav {
        margin-top: 1rem;
    }
    
    .cards {
        grid-template-columns: 1fr;
    }
}
{
  "version": 2,
  "builds": [
    {
      "src": "public/index.html",
      "use": "@vercel/static"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "public/index.html"
    }
  ]
}
