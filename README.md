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
                </div>
            </div>
        </section>
    </main>
    <footer>
        <p>Termos de Uso | Política de Privacidade</p>
    </footer>
</body>
</html>
"""

# CSS (mantido igual)
css_content = """
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #fff;
    color: #111;
}
/* ... (restante do CSS permanece idêntico) ... */
"""

# Salvar arquivos
with open(f"{output_dir}/index.html", "w", encoding="utf-8") as f:
    f.write(html_content)
with open(f"{output_dir}/style.css", "w", encoding="utf-8") as f:
    f.write(css_content)
