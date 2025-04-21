<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tellink Telecom</title>
    <link rel="stylesheet" href="style.css" />
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
                a>
            </div>
        </section>
    </main>
    <footer>
        <p>Termos de Uso | Política de Privacidade</p>
    </footer>
</body>
</html>
"""

# CSS base simples
css_content = """
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #fff;
    color: #111;
}
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #fff;
    padding: 1rem 2rem;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
.logo {
    font-weight: bold;
    font-size: 1.5rem;
    color: #b30000;
}
.logo span {
    font-weight: normal;
}
nav a {
    margin-left: 1rem;
    text-decoration: none;
    color: #000;
}
nav .whatsapp {
    background: #25D366;
    color: #fff;
    padding: 0.5rem 1rem;
    border-radius: 6px;
}
.hero {
    background: #c0392b;
    color: white;
    text-align: center;
    padding: 3rem 1rem;
}
.hero .btn {
    display: inline-block;
    margin-top: 1rem;
    background: #a30000;
    color: white;
    padding: 0.75rem 1.5rem;
    border-radius: 4px;
    text-decoration: none;
}
.planos {
    background: #fff;
    padding: 2rem;
    text-align: center;
}
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin-top: 2rem;
}
.card {
    background: #fafafa;
    padding: 1.5rem;
    border-radius: 12px;
    box-shadow: 0 0 8px rgba(0,0,0,0.05);
    position: relative;
}
.badge {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: yellow;
    color: black;
    font-weight: bold;
    padding: 0.2rem 0.5rem;
    border-radius: 5px;
}
footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 1rem;
}
"""
