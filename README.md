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
                <div class="card">
                    <h3>100 Mega</h3>
                    <p>R$ 49,90</p>
                    <ul>
                        <li>Wi-Fi 5 incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>150 Mega</h3>
                    <p>R$ 59,90</p>
                    <ul>
                        <li>50% de desconto na 1ª parcela</li>
                        <li>Wi-Fi 5 incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
                <div class="card destaque">
                    <span class="badge">Mais Vendido</span>
                    <h3>300 Mega</h3>
                    <p>R$ 69,90</p>
                    <ul>
                        <li>50% de desconto na 1ª parcela</li>
                        <li>Wi-Fi 5 incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
                <div class="card destaque">
                    <span class="badge">Mais Vendido</span>
                    <h3>450 Mega</h3>
                    <p>R$ 79,90</p>
                    <ul>
                        <li>50% de desconto na 1ª parcela</li>
                        <li>Wi-Fi 5 incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>600 Mega</h3>
                    <p>R$ 99,90</p>
                    <ul>
                        <li>50% nas 4 primeiras parcelas</li>
                        <li>Wi-Fi 6 incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>1 Giga</h3>
                    <p>R$ 199,90</p>
                    <ul>
                        <li>Wi-Fi 6 incluso</li>
                        <li>2 câmeras com IA ou alarme incluso</li>
                        <li>Consulte taxa de instalação</li>
                    </ul>
                </div>
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

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background: white;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.logo {
    font-size: 1.8rem;
    font-weight: 700;
    color: var(--primary);
}

.logo span {
    font-weight: 400;
}

nav a {
    margin-left: 1.5rem;
    text-decoration: none;
    color: #333;
    font-weight: 500;
}

.whatsapp {
    background: var(--whatsapp);
    color: white !important;
    padding: 0.5rem 1rem;
    border-radius: 6px;
}

.hero {
    background: var(--secondary);
    color: white;
    text-align: center;
    padding: 4rem 1rem;
}

.hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.btn {
    display: inline-block;
    background: var(--primary);
    color: white;
    padding: 0.8rem 1.8rem;
    border-radius: 6px;
    text-decoration: none;
    font-weight: bold;
    transition: all 0.3s ease;
}

.btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.planos {
    padding: 4rem 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.planos h2 {
    text-align: center;
    font-size: 2rem;
    margin-bottom: 2rem;
}

.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}

.card {
    background: #f9f9f9;
    border-radius: 10px;
    padding: 2rem;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
    position: relative;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

.destaque {
    border: 2px solid var(--primary);
}

.badge {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: gold;
    color: black;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: bold;
}

.card h3 {
    color: var(--primary);
    font-size: 1.5rem;
    margin-bottom: 1rem;
}

.card p {
    font-size: 1.8rem;
    font-weight: bold;
    margin-bottom: 1.5rem;
}

.card ul {
    list-style: none;
}

.card li {
    margin-bottom: 0.8rem;
    position: relative;
    padding-left: 1.5rem;
}

.card li:before {
    content: "•";
    color: var(--primary);
    position: absolute;
    left: 0;
}

footer {
    background: #222;
    color: white;
    text-align: center;
    padding: 2rem;
    margin-top: 4rem;
}

footer p {
    margin: 0;
}

@media (max-width: 768px) {
    header {
        flex-direction: column;
        gap: 1rem;
    }
    
    nav {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 1rem;
    }
    
    nav a {
        margin: 0;
    }
    
    .hero h1 {
        font-size: 2rem;
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
