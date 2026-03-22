# Project-Latam
🤖 LATAM - Previsão de Demanda e Manutenção Preditiva Este repositório contém modelos de Machine Learning aplicados ao contexto operacional da LATAM Airlines. O projeto é dividido em duas frentes principais: previsão de demanda de passageiros para gestão de receitas (Revenue Management) e manutenção preditiva para redução de AOG.
### HTML (Estrutura do projeto do site)
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="description" content="LATAM Airlines - Voos e Destinos. Descubra a América Latina com a melhor experiência a bordo. Reserve seus voos para mais de 100 destinos.">
    <title>LATAM Airlines - Voos e Destinos</title>
    <link rel="stylesheet" href="Index.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

</head>
<body>
    <header class="header">
        <nav class="nav-container">
            <div class="logo">
                <img src="https://vetores.org/wp-content/uploads/latam.png" alt="LATAM Airlines" class="logo-img">
            </div>
            
            <button class="hamburger" aria-label="Menu">
                <span class="hamburger-line"></span>
                <span class="hamburger-line"></span>
                <span class="hamburger-line"></span>
            </button>

            <ul class="nav-menu">
                <li><a href="#home" class="nav-link active">Home</a></li>
                <li><a href="#destinos" class="nav-link">Destinos</a></li>
                <li><a href="#voos" class="nav-link">Voos</a></li>
                <li><a href="#servicos" class="nav-link">Serviços</a></li>
                <li><a href="#contato" class="nav-link">Contato</a></li>
            </ul>

            <div class="nav-buttons">
                <button class="btn-login" aria-label="Login">
                    <i class="fas fa-user"></i>
                    <span class="login-text">Entrar</span>
                </button>
                <button class="btn-signup">Cadastrar</button>
            </div>
        </nav>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="hero-content">
                <h1>Descubra a América Latina <span class="highlight">conosco</span></h1>
                <p>Voos para mais de 100 destinos com a melhor experiência a bordo</p>
                
                <form class="search-form" id="searchForm">
                    <div class="form-group">
                        <label for="from">Origem</label>
                        <input type="text" id="from" placeholder="Cidade de origem" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="to">Destino</label>
                        <input type="text" id="to" placeholder="Cidade de destino" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="date">Data</label>
                        <input type="date" id="date" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="passengers">Passageiros</label>
                        <select id="passengers">
                            <option value="1">1 passageiro</option>
                            <option value="2">2 passageiros</option>
                            <option value="3">3 passageiros</option>
                            <option value="4">4+ passageiros</option>
                        </select>
                    </div>
                    
                    <button type="submit" class="btn-search">
                        <i class="fas fa-search"></i>
                        Buscar Voos
                    </button>
                </form>
            </div>
        </section>

        <section id="destinos" class="destinos">
            <div class="container">
                <h2>Destinos em Destaque</h2>
                <p class="section-subtitle">Os lugares mais procurados da América Latina</p>
                
                <div class="destinos-grid">
                    <article class="destino-card">
                        <figure class="destino-image">
                            <img src="https://images.unsplash.com/photo-1518639192441-8fce0a366e2e?w=500" alt="Rio de Janeiro" loading="lazy">
                            <figcaption>Cristo Redentor</figcaption>
                        </figure>
                        <div class="destino-info">
                            <h3>Rio de Janeiro</h3>
                            <p class="destino-pais">Brasil</p>
                            <p class="destino-preco">A partir de R$ 599</p>
                            <button class="btn-detalhes">Ver detalhes</button>
                        </div>
                    </article>

                    <article class="destino-card">
                        <figure class="destino-image">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTPBdCcUemUTykE090-tXuRx65evSvNMyHlAg&s" alt="Sao Paulo" loading="lazy">
                            <figcaption>Estaiada-Sao Paulo</figcaption>
                        </figure>
                        <div class="destino-info">
                            <h3>São Paulo</h3>
                            <p class="destino-pais">Brasil</p>
                            <p class="destino-preco">A partir de R$ 899</p>
                            <button class="btn-detalhes">Ver detalhes</button>
                        </div>
                    </article>

                    <article class="destino-card">
                        <figure class="destino-image">
                            <img src="https://airesbuenosblog.com/wp-content/uploads/2016/03/obelisco-noite.jpg" alt="Buenos Aires" loading="lazy">
                            <figcaption>Obelisco</figcaption>
                        </figure>
                        <div class="destino-info">
                            <h3>Buenos Aires</h3>
                            <p class="destino-pais">Argentina</p>
                            <p class="destino-preco">A partir de R$ 699</p>
                            <button class="btn-detalhes">Ver detalhes</button>
                        </div>
                    </article>

                    <article class="destino-card">
                        <figure class="destino-image">
                            <img src="https://blog.123milhas.com/wp-content/uploads/2022/04/BANNER-TEM-IR-SANTIAGO-123MILHAS-1024x574.jpg" alt="Santiago" loading="lazy">
                            <figcaption>Cerro San Cristóbal</figcaption>
                        </figure>
                        <div class="destino-info">
                            <h3>Santiago</h3>
                            <p class="destino-pais">Chile</p>
                            <p class="destino-preco">A partir de R$ 799</p>
                            <button class="btn-detalhes">Ver detalhes</button>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <section id="voos" class="voos">
            <div class="container">
                <h2>Próximos Voos</h2>
                <p class="section-subtitle">Ofertas especiais para sua viagem</p>
                
                <div class="voos-tabs">
                    <button class="tab-btn active" data-tab="ida">Só ida</button>
                    <button class="tab-btn" data-tab="ida-volta">Ida e volta</button>
                    <button class="tab-btn" data-tab="multiplos">Múltiplos destinos</button>
                </div>

                <div class="voos-lista" id="voosLista">
                    <!-- Voos serão carregados via JavaScript -->
                </div>
            </div>
        </section>

        <section id="servicos" class="servicos">
            <div class="container">
                <h2>Nossos Serviços</h2>
                <p class="section-subtitle">Experiência completa para sua viagem</p>
                
                <div class="servicos-grid">
                    <div class="servico-card">
                        <i class="fas fa-plane-departure"></i>
                        <h3>Check-in Online</h3>
                        <p>Faça seu check-in com até 48h de antecedência</p>
                    </div>
                    
                    <div class="servico-card">
                        <i class="fas fa-suitcase"></i>
                        <h3>Bagagem</h3>
                        <p>Inclua bagagem despachada no seu bilhete</p>
                    </div>
                    
                    <div class="servico-card">
                        <i class="fas fa-utensils"></i>
                        <h3>Refeições a Bordo</h3>
                        <p>Cardápio especial preparado por chefs renomados</p>
                    </div>
                    
                    <div class="servico-card">
                        <i class="fas fa-wifi"></i>
                        <h3>Wi-Fi a Bordo</h3>
                        <p>Conexão de internet durante todo o voo</p>
                    </div>
                    
                    <div class="servico-card">
                        <i class="fas fa-couch"></i>
                        <h3>Assentos Confortáveis</h3>
                        <p>Mais espaço e conforto para sua viagem</p>
                    </div>
                    
                    <div class="servico-card">
                        <i class="fas fa-tv"></i>
                        <h3>Entretenimento</h3>
                        <p>Filmes, séries e músicas para todos os gostos</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contato" class="contato">
            <div class="container">
                <h2>Fale Conosco</h2>
                <p class="section-subtitle">Estamos aqui para ajudar você</p>
                
                <div class="contato-wrapper">
                    <form class="contato-form" id="contatoForm">
                        <div class="form-row">
                            <div class="form-group">
                                <label for="nome">Nome completo</label>
                                <input type="text" id="nome" required>
                            </div>
                            
                            <div class="form-group">
                                <label for="email">E-mail</label>
                                <input type="email" id="email" required>
                            </div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="telefone">Telefone</label>
                                <input type="tel" id="telefone">
                            </div>
                            
                            <div class="form-group">
                                <label for="assunto">Assunto</label>
                                <select id="assunto" required>
                                    <option value="">Selecione</option>
                                    <option value="Duvida">Dúvida</option>
                                    <option value="reclamacao">Reclamação</option>
                                    <option value="sugestao">Sugestão</option>
                                    <option value="outro">Outro</option>
                                </select>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label for="mensagem">Mensagem</label>
                            <textarea id="mensagem" rows="5" required></textarea>
                        </div>
                        
                        <button type="submit" class="btn-submit">Enviar mensagem</button>
                    </form>
                    
                    <div class="contato-info">
                        <h3>Outros canais de atendimento</h3>
                        
                        <div class="info-item">
                            <i class="fas fa-phone"></i>
                            <div>
                                <h4>Central de Vendas</h4>
                                <p>4002-8922 (capitais)</p>
                                <p>0800-123-4567 (demais localidades)</p>
                            </div>
                        </div>
                        
                        <div class="info-item">
                            <i class="fas fa-comment"></i>
                            <div>
                                <h4>WhatsApp</h4>
                                <p>+81 80 2740-6058</p>
                            </div>
                        </div>
                        
                        <div class="info-item">
                            <i class="fas fa-envelope"></i>
                            <div>
                                <h4>E-mail</h4>
                                <p>sac@latam.com.br</p>
                            </div>
                        </div>
                        
                        <div class="social-links">
                            <h4>Redes Sociais</h4>
                            <div class="social-icons">
                                <a href="https://www.facebook.com/fagnerjacob" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
                                <a href="https://www.instagram.com/fagner_jacob/" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                                <a href="https://www.youtube.com/@Canal_do_Fagner_Jacob" aria-label="YouTube"><i class="fab fa-youtube"></i></a>
                                <a href="https://www.linkedin.com/in/fagnerjacob/" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
                                <a href="https://www.tiktok.com/@fagner.jacob" aria-label="TikTok"><i class="fab fa-tiktok"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <h4>Sobre a LATAM</h4>
                    <ul>
                        <li><a href="#">Quem somos</a></li>
                        <li><a href="#">Sala de imprensa</a></li>
                        <li><a href="#">Trabalhe conosco</a></li>
                        <li><a href="#">Sustentabilidade</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h4>Serviços</h4>
                    <ul>
                        <li><a href="#">Check-in</a></li>
                        <li><a href="#">Status do voo</a></li>
                        <li><a href="#">Bagagem</a></li>
                        <li><a href="#">Programa de pontos</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h4>Ajuda</h4>
                    <ul>
                        <li><a href="#">Central de ajuda</a></li>
                        <li><a href="#">Perguntas frequentes</a></li>
                        <li><a href="#">Política de privacidade</a></li>
                        <li><a href="#">Termos de uso</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h4>Newsletter</h4>
                    <p>Receba ofertas exclusivas</p>
                    <form class="newsletter-form">
                        <input type="email" placeholder="onishi.fagner@gmail.com">
                        <button type="submit">Enviar</button>
                    </form>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; Projeto *Desenvolvido por Fagner Jacob -2026 LATAM Airlines. Todos os direitos reservados.</p>
                <div class="footer-payment">
                    <i class="fab fa-cc-visa"></i>
                    <i class="fab fa-cc-mastercard"></i>
                    <i class="fab fa-cc-amex"></i>
                    <i class="fab fa-cc-diners-club"></i>
                </div>
            </div>
        </div>
    </footer>

    <div class="modal" id="modal" aria-hidden="true">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar">&times;</button>
            <div class="modal-body" id="modalBody">
                <!-- Conteúdo do modal será inserido via JavaScript -->
            </div>
        </div>
    </div>

    <script src="Index.js"></script>
</body>
</html>

### CSS (Estilização do projeto)

/* Reset e Variáveis */
:root {
    --primary-color: #0a2b5e;
    --secondary-color: #d52b1e;
    --text-color: #333;
    --light-bg: #f5f5f5;
    --white: #ffffff;
    --shadow: 0 2px 10px rgba(0,0,0,0.1);
    --transition: all 0.3s ease;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
}

/* Header e Navegação */
.header {
    background: var(--white);
    box-shadow: var(--shadow);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo-img {
    height: 40px;
    width: auto;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-link {
    text-decoration: none;
    color: var(--text-color);
    font-weight: 500;
    transition: var(--transition);
    position: relative;
}

.nav-link:hover,
.nav-link.active {
    color: var(--secondary-color);
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--secondary-color);
    transition: var(--transition);
}

.nav-link:hover::after,
.nav-link.active::after {
    width: 100%;
}

.nav-buttons {
    display: flex;
    gap: 1rem;
    align-items: center;
}

.btn-login {
    background: none;
    border: none;
    cursor: pointer;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    font-size: 1rem;
    color: var(--text-color);
    transition: var(--transition);
}

.btn-login:hover {
    color: var(--secondary-color);
}

.btn-signup {
    background: var(--secondary-color);
    color: var(--white);
    border: none;
    padding: 0.5rem 1.5rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
    font-weight: 500;
}

.btn-signup:hover {
    background: #b22216;
    transform: translateY(-2px);
}

.hamburger {
    display: none;
    flex-direction: column;
    gap: 6px;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0.5rem;
}

.hamburger-line {
    width: 25px;
    height: 3px;
    background: var(--primary-color);
    transition: var(--transition);
}

/* Hero Section */
.hero {
    background: linear-gradient(rgba(10, 43, 94, 0.8), rgba(10, 43, 94, 0.8)),
                url('https://images.unsplash.com/photo-1436491865332-7a61a109cc05?w=1200');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: var(--white);
    margin-top: 60px;
}

.hero-content {
    max-width: 900px;
    padding: 2rem;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    animation: fadeInUp 1s ease;
}

.highlight {
    color: var(--secondary-color);
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    animation: fadeInUp 1s ease 0.2s both;
}

.search-form {
    background: rgba(255, 255, 255, 0.95);
    padding: 2rem;
    border-radius: 10px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
    animation: fadeInUp 1s ease 0.4s both;
}

.form-group {
    text-align: left;
}

.form-group label {
    display: block;
    color: var(--text-color);
    margin-bottom: 0.5rem;
    font-weight: 500;
    font-size: 0.9rem;
}

.form-group input,
.form-group select {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #ddd;
    border-radius: 5px;
    font-size: 1rem;
    transition: var(--transition);
}

.form-group input:focus,
.form-group select:focus {
    outline: none;
    border-color: var(--secondary-color);
}

.btn-search {
    background: var(--secondary-color);
    color: var(--white);
    border: none;
    padding: 0.75rem 1.5rem;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    font-weight: 500;
    transition: var(--transition);
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
    grid-column: 1 / -1;
}

.btn-search:hover {
    background: #b22216;
    transform: translateY(-2px);
}

/* Seções Gerais */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 1rem;
}

section {
    padding: 4rem 0;
}

section:nth-child(even) {
    background: var(--light-bg);
}

h2 {
    font-size: 2.5rem;
    color: var(--primary-color);
    text-align: center;
    margin-bottom: 1rem;
}

.section-subtitle {
    text-align: center;
    color: #666;
    margin-bottom: 3rem;
    font-size: 1.1rem;
}

/* Destinos Grid */
.destinos-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.destino-card {
    background: var(--white);
    border-radius: 10px;
    overflow: hidden;
    box-shadow: var(--shadow);
    transition: var(--transition);
}

.destino-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 5px 20px rgba(0,0,0,0.2);
}

.destino-image {
    position: relative;
    overflow: hidden;
    aspect-ratio: 16/9;
}

.destino-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: var(--transition);
}

.destino-card:hover .destino-image img {
    transform: scale(1.1);
}

.destino-image figcaption {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: linear-gradient(transparent, rgba(0,0,0,0.8));
    color: var(--white);
    padding: 1rem;
    transform: translateY(100%);
    transition: var(--transition);
}

.destino-card:hover .destino-image figcaption {
    transform: translateY(0);
}

.destino-info {
    padding: 1.5rem;
}

.destino-info h3 {
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
}

.destino-pais {
    color: #666;
    margin-bottom: 0.5rem;
}

.destino-preco {
    font-size: 1.2rem;
    font-weight: bold;
    color: var(--secondary-color);
    margin-bottom: 1rem;
}

.btn-detalhes {
    background: none;
    border: 2px solid var(--primary-color);
    color: var(--primary-color);
    padding: 0.5rem 1rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
    width: 100%;
    font-weight: 500;
}

.btn-detalhes:hover {
    background: var(--primary-color);
    color: var(--white);
}

/* Voos Section */
.voos-tabs {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 2rem;
}

.tab-btn {
    background: none;
    border: 2px solid var(--primary-color);
    color: var(--primary-color);
    padding: 0.75rem 2rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
    font-weight: 500;
}

.tab-btn.active,
.tab-btn:hover {
    background: var(--primary-color);
    color: var(--white);
}

.voos-lista {
    display: grid;
    gap: 1rem;
}

.voo-item {
    background: var(--white);
    border-radius: 10px;
    padding: 1.5rem;
    display: grid;
    grid-template-columns: auto 1fr auto;
    gap: 2rem;
    align-items: center;
    box-shadow: var(--shadow);
    transition: var(--transition);
}

.voo-item:hover {
    transform: translateX(5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.15);
}

.voo-horario {
    text-align: center;
}

.voo-horario .hora {
    font-size: 1.5rem;
    font-weight: bold;
    color: var(--primary-color);
}

.voo-horario .cidade {
    color: #666;
}

.voo-duracao {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #999;
}

.voo-duracao i {
    color: var(--secondary-color);
    margin-bottom: 0.5rem;
}

.voo-preco {
    text-align: right;
}

.voo-preco .preco {
    font-size: 2rem;
    font-weight: bold;
    color: var(--secondary-color);
}

.voo-preco .parcelamento {
    color: #666;
    font-size: 0.9rem;
}

.btn-comprar {
    background: var(--primary-color);
    color: var(--white);
    border: none;
    padding: 0.5rem 2rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
    font-weight: 500;
}

.btn-comprar:hover {
    background: var(--secondary-color);
}

/* Serviços */
.servicos-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.servico-card {
    background: var(--white);
    padding: 2rem;
    border-radius: 10px;
    text-align: center;
    box-shadow: var(--shadow);
    transition: var(--transition);
}

.servico-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(0,0,0,0.15);
}

.servico-card i {
    font-size: 3rem;
    color: var(--secondary-color);
    margin-bottom: 1rem;
}

.servico-card h3 {
    margin-bottom: 1rem;
    color: var(--primary-color);
}

.servico-card p {
    color: #666;
}

/* Contato */
.contato-wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    background: var(--white);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: var(--shadow);
}

.contato-form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.form-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
}

.contato-form .form-group {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.contato-form input,
.contato-form select,
.contato-form textarea {
    padding: 0.75rem;
    border: 1px solid #ddd;
    border-radius: 5px;
    transition: var(--transition);
}

.contato-form input:focus,
.contato-form select:focus,
.contato-form textarea:focus {
    outline: none;
    border-color: var(--secondary-color);
}

.btn-submit {
    background: var(--primary-color);
    color: var(--white);
    border: none;
    padding: 1rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
    font-weight: 500;
    font-size: 1rem;
}

.btn-submit:hover {
    background: var(--secondary-color);
}

.contato-info {
    padding-left: 2rem;
    border-left: 2px solid var(--light-bg);
}

.contato-info h3 {
    color: var(--primary-color);
    margin-bottom: 2rem;
}

.info-item {
    display: flex;
    gap: 1rem;
    margin-bottom: 1.5rem;
}

.info-item i {
    font-size: 1.5rem;
    color: var(--secondary-color);
}

.info-item h4 {
    margin-bottom: 0.5rem;
}

.info-item p {
    color: #666;
}

.social-links {
    margin-top: 2rem;
}

.social-icons {
    display: flex;
    gap: 1rem;
    margin-top: 1rem;
}

.social-icons a {
    color: var(--primary-color);
    font-size: 1.5rem;
    transition: var(--transition);
}

.social-icons a:hover {
    color: var(--secondary-color);
    transform: translateY(-3px);
}

/* Footer */
.footer {
    background: var(--primary-color);
    color: var(--white);
    padding: 4rem 0 2rem;
}

.footer-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 3rem;
    margin-bottom: 3rem;
}

.footer-col h4 {
    margin-bottom: 1.5rem;
    position: relative;
    padding-bottom: 0.5rem;
}

.footer-col h4::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 50px;
    height: 2px;
    background: var(--secondary-color);
}

.footer-col ul {
    list-style: none;
}

.footer-col ul li {
    margin-bottom: 0.5rem;
}

.footer-col a {
    color: #ccc;
    text-decoration: none;
    transition: var(--transition);
}

.footer-col a:hover {
    color: var(--secondary-color);
    padding-left: 5px;
}

.newsletter-form {
    display: flex;
    gap: 0.5rem;
    margin-top: 1rem;
}

.newsletter-form input {
    flex: 1;
    padding: 0.5rem;
    border: none;
    border-radius: 5px;
}

.newsletter-form button {
    background: var(--secondary-color);
    color: var(--white);
    border: none;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    cursor: pointer;
    transition: var(--transition);
}

.newsletter-form button:hover {
    background: #b22216;
}

.footer-bottom {
    border-top: 1px solid rgba(255,255,255,0.1);
    padding-top: 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
}

.footer-payment {
    display: flex;
    gap: 1rem;
    font-size: 2rem;
}

/* Modal */
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.5);
    z-index: 2000;
    align-items: center;
    justify-content: center;
}

.modal.active {
    display: flex;
}

.modal-content {
    background: var(--white);
    border-radius: 10px;
    max-width: 500px;
    width: 90%;
    max-height: 80vh;
    overflow-y: auto;
    position: relative;
    animation: modalIn 0.3s ease;
}

.modal-close {
    position: absolute;
    top: 1rem;
    right: 1rem;
    background: none;
    border: none;
    font-size: 1.5rem;
    cursor: pointer;
    color: #666;
    transition: var(--transition);
}

.modal-close:hover {
    color: var(--secondary-color);
}

.modal-body {
    padding: 2rem;
}

/* Mensagens de Feedback */
.success-message {
    background: #d4edda;
    color: #155724;
    padding: 1rem;
    border-radius: 5px;
    margin-bottom: 1rem;
    text-align: center;
    animation: slideIn 0.3s ease;
}

.error-message {
    background: #f8d7da;
    color: #721c24;
    padding: 1rem;
    border-radius: 5px;
    margin-bottom: 1rem;
    text-align: center;
    animation: slideIn 0.3s ease;
}

/* Loader */
.loader {
    border: 3px solid #f3f3f3;
    border-top: 3px solid var(--secondary-color);
    border-radius: 50%;
    width: 40px;
    height: 40px;
    animation: spin 1s linear infinite;
    margin: 2rem auto;
}

/* Animações */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes modalIn {
    from {
        opacity: 0;
        transform: translateY(-50px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes slideIn {
    from {
        opacity: 0;
        transform: translateX(-20px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

/* Media Queries - Responsividade */
@media (max-width: 1024px) {
    .hero h1 {
        font-size: 2.5rem;
    }
    
    .contato-wrapper {
        grid-template-columns: 1fr;
    }
    
    .contato-info {
        padding-left: 0;
        border-left: none;
        border-top: 2px solid var(--light-bg);
        padding-top: 2rem;
    }
}

@media (max-width: 768px) {
    .nav-menu {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: var(--white);
        flex-direction: column;
        padding: 2rem;
        text-align: center;
        box-shadow: var(--shadow);
    }
    
    .nav-menu.active {
        display: flex;
    }
    
    .hamburger {
        display: flex;
    }
    
    .hamburger.active .hamburger-line:nth-child(1) {
        transform: rotate(45deg) translate(8px, 6px);
    }
    
    .hamburger.active .hamburger-line:nth-child(2) {
        opacity: 0;
    }
    
    .hamburger.active .hamburger-line:nth-child(3) {
        transform: rotate(-45deg) translate(7px, -5px);
    }
    
    .nav-buttons {
        display: none;
    }
    
    .hero {
        height: auto;
        min-height: 100vh;
    }
    
    .hero h1 {
        font-size: 2rem;
    }
    
    .search-form {
        grid-template-columns: 1fr;
    }
    
    .voo-item {
        grid-template-columns: 1fr;
        text-align: center;
        gap: 1rem;
    }
    
    .voo-preco {
        text-align: center;
    }
    
    .form-row {
        grid-template-columns: 1fr;
    }
    
    .footer-grid {
        grid-template-columns: 1fr;
        text-align: center;
    }
    
    .footer-col h4::after {
        left: 50%;
        transform: translateX(-50%);
    }
    
    .footer-bottom {
        flex-direction: column;
        text-align: center;
    }
}

@media (max-width: 480px) {
    .hero h1 {
        font-size: 1.5rem;
    }
    
    .hero p {
        font-size: 1rem;
    }
    
    h2 {
        font-size: 2rem;
    }
    
    .voos-tabs {
        flex-direction: column;
    }
    
    .tab-btn {
        width: 100%;
    }
    
    .servicos-grid {
        grid-template-columns: 1fr;
    }
}

/* Acessibilidade */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
    }
}

.sr-only {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    white-space: nowrap;
    border-width: 0;
}

### Java Script (Cerebro do projeto)

// Classe principal do site
class LatamSite {
    constructor() {
        this.init();
    }

    init() {
        this.cacheElements();
        this.bindEvents();
        this.loadVoos();
        this.initAnimations();
        this.initFormValidation();
    }

    cacheElements() {
        // Header e navegação
        this.hamburger = document.querySelector('.hamburger');
        this.navMenu = document.querySelector('.nav-menu');
        this.navLinks = document.querySelectorAll('.nav-link');
        
        // Forms
        this.searchForm = document.getElementById('searchForm');
        this.contatoForm = document.getElementById('contatoForm');
        this.newsletterForm = document.querySelector('.newsletter-form');
        
        // Elementos dinâmicos
        this.voosLista = document.getElementById('voosLista');
        this.modal = document.getElementById('modal');
        this.modalBody = document.getElementById('modalBody');
        
        // Tabs
        this.tabBtns = document.querySelectorAll('.tab-btn');
        
        // Botões de detalhes
        this.detalhesBtns = document.querySelectorAll('.btn-detalhes');
    }

    bindEvents() {
        // Menu mobile
        this.hamburger?.addEventListener('click', () => this.toggleMenu());
        
        // Links de navegação
        this.navLinks.forEach(link => {
            link.addEventListener('click', (e) => this.handleNavClick(e));
        });
        
        // Scroll event para active link
        window.addEventListener('scroll', () => this.updateActiveLink());
        
        // Forms
        this.searchForm?.addEventListener('submit', (e) => this.handleSearch(e));
        this.contatoForm?.addEventListener('submit', (e) => this.handleContato(e));
        this.newsletterForm?.addEventListener('submit', (e) => this.handleNewsletter(e));
        
        // Tabs
        this.tabBtns.forEach(btn => {
            btn.addEventListener('click', (e) => this.handleTabClick(e));
        });
        
        // Botões de detalhes
        this.detalhesBtns.forEach(btn => {
            btn.addEventListener('click', (e) => this.handleDetalhes(e));
        });
        
        // Fechar modal
        document.querySelector('.modal-close')?.addEventListener('click', () => this.closeModal());
        window.addEventListener('click', (e) => {
            if (e.target === this.modal) this.closeModal();
        });
        
        // Login button
        document.querySelector('.btn-login')?.addEventListener('click', () => this.showLoginModal());
        
        // Signup button
        document.querySelector('.btn-signup')?.addEventListener('click', () => this.showSignupModal());
    }

    toggleMenu() {
        this.hamburger?.classList.toggle('active');
        this.navMenu?.classList.toggle('active');
    }

    handleNavClick(e) {
        e.preventDefault();
        const link = e.currentTarget;
        const targetId = link.getAttribute('href');
        
        if (targetId === '#') return;
        
        const targetSection = document.querySelector(targetId);
        if (targetSection) {
            targetSection.scrollIntoView({ behavior: 'smooth' });
            
            // Fecha menu mobile se aberto
            this.navMenu?.classList.remove('active');
            this.hamburger?.classList.remove('active');
            
            // Atualiza active link
            this.navLinks.forEach(l => l.classList.remove('active'));
            link.classList.add('active');
        }
    }

    updateActiveLink() {
        const sections = document.querySelectorAll('section');
        const scrollPosition = window.scrollY + 100;

        sections.forEach(section => {
            const sectionTop = section.offsetTop;
            const sectionBottom = sectionTop + section.offsetHeight;
            const sectionId = section.getAttribute('id');

            if (scrollPosition >= sectionTop && scrollPosition < sectionBottom) {
                this.navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${sectionId}`) {
                        link.classList.add('active');
                    }
                });
            }
        });
    }

    // Carregar voos dinamicamente
    loadVoos() {
        this.showLoader();
        
        // Simulando chamada API
        setTimeout(() => {
            const voos = [
                {
                    origem: 'GRU',
                    destino: 'GIG',
                    origemCidade: 'São Paulo',
                    destinoCidade: 'Rio de Janeiro',
                    partida: '08:00',
                    chegada: '09:00',
                    duracao: '1h',
                    preco: 299,
                    parcelas: 10
                },
                {
                    origem: 'GIG',
                    destino: 'CGH',
                    origemCidade: 'Rio de Janeiro',
                    destinoCidade: 'São Paulo',
                    partida: '10:30',
                    chegada: '11:30',
                    duracao: '1h',
                    preco: 279,
                    parcelas: 10
                },
                {
                    origem: 'GRU',
                    destino: 'BSB',
                    origemCidade: 'São Paulo',
                    destinoCidade: 'Brasília',
                    partida: '14:00',
                    chegada: '16:00',
                    duracao: '2h',
                    preco: 399,
                    parcelas: 12
                }
            ];
            
            this.renderVoos(voos);
        }, 1000);
    }

    renderVoos(voos) {
        const voosHTML = voos.map(voo => `
            <article class="voo-item">
                <div class="voo-horario">
                    <span class="hora">${voo.partida}</span>
                    <span class="cidade">${voo.origem} - ${voo.origemCidade}</span>
                </div>
                
                <div class="voo-duracao">
                    <i class="fas fa-plane"></i>
                    <span>${voo.duracao}</span>
                </div>
                
                <div class="voo-horario">
                    <span class="hora">${voo.chegada}</span>
                    <span class="cidade">${voo.destino} - ${voo.destinoCidade}</span>
                </div>
                
                <div class="voo-preco">
                    <div class="preco">R$ ${voo.preco}</div>
                    <div class="parcelamento">em até ${voo.parcelas}x</div>
                    <button class="btn-comprar" data-voo='${JSON.stringify(voo)}'>Comprar</button>
                </div>
            </article>
        `).join('');
        
        this.voosLista.innerHTML = voosHTML;
        
        // Adiciona eventos aos botões de compra
        document.querySelectorAll('.btn-comprar').forEach(btn => {
            btn.addEventListener('click', (e) => this.handleCompra(e));
        });
    }

    handleCompra(e) {
        const vooData = JSON.parse(e.currentTarget.dataset.voo);
        this.showModal('Reserva de Voo', `
            <h3>Confirmar reserva</h3>
            <p>Voo: ${vooData.origem} (${vooData.origemCidade}) → ${vooData.destino} (${vooData.destinoCidade})</p>
            <p>Horário: ${vooData.partida} - ${vooData.chegada}</p>
            <p>Preço: R$ ${vooData.preco}</p>
            <button class="btn-submit" onclick="latamSite.confirmarCompra()">Confirmar</button>
        `);
    }

    confirmarCompra() {
        this.showMessage('success', 'Reserva confirmada com sucesso!');
        setTimeout(() => this.closeModal(), 2000);
    }

    handleSearch(e) {
        e.preventDefault();
        const formData = new FormData(e.target);
        const searchData = Object.fromEntries(formData);
        
        this.showMessage('success', 'Buscando voos...');
        
        // Simula busca
        setTimeout(() => {
            this.showModal('Resultados da Busca', `
                <h3>Voos encontrados</h3>
                <p>Origem: ${searchData.from}</p>
                <p>Destino: ${searchData.to}</p>
                <p>Data: ${searchData.date}</p>
                <p>Passageiros: ${searchData.passengers}</p>
                <p>Redirecionando para resultados...</p>
            `);
        }, 1500);
    }

    handleContato(e) {
        e.preventDefault();
        const formData = new FormData(e.target);
        const contatoData = Object.fromEntries(formData);
        
        this.showMessage('success', 'Mensagem enviada com sucesso!');
        e.target.reset();
    }

    handleNewsletter(e) {
        e.preventDefault();
        const email = e.target.querySelector('input[type="email"]').value;
        
        if (this.validateEmail(email)) {
            this.showMessage('success', 'Inscrição realizada com sucesso!');
            e.target.reset();
        } else {
            this.showMessage('error', 'Por favor, insira um e-mail válido.');
        }
    }

    handleTabClick(e) {
        const tab = e.currentTarget;
        this.tabBtns.forEach(btn => btn.classList.remove('active'));
        tab.classList.add('active');
        
        // Aqui você pode carregar diferentes voos baseado na tab
        this.loadVoos();
    }

    handleDetalhes(e) {
        const card = e.currentTarget.closest('.destino-card');
        const destino = card.querySelector('h3').textContent;
        const preco = card.querySelector('.destino-preco').textContent;
        
        this.showModal(destino, `
            <img src="${card.querySelector('img').src}" alt="${destino}" style="width: 100%; border-radius: 5px; margin-bottom: 1rem;">
            <h3>${destino}</h3>
            <p>${preco}</p>
            <p>Descrição detalhada do destino, incluindo informações sobre pontos turísticos, clima, melhor época para visitar e dicas de viagem.</p>
            <button class="btn-submit" onclick="latamSite.reservarDestino('${destino}')">Reservar agora</button>
        `);
    }

    reservarDestino(destino) {
        this.showMessage('success', `Reserva para ${destino} iniciada!`);
        setTimeout(() => this.closeModal(), 1500);
    }

    showLoginModal() {
        this.showModal('Login', `
            <form id="loginForm" onsubmit="latamSite.handleLogin(event)">
                <div class="form-group">
                    <label for="loginEmail">E-mail</label>
                    <input type="email" id="loginEmail" required>
                </div>
                <div class="form-group">
                    <label for="loginPassword">Senha</label>
                    <input type="password" id="loginPassword" required>
                </div>
                <button type="submit" class="btn-submit">Entrar</button>
                <p style="text-align: center; margin-top: 1rem;">
                    <a href="#" onclick="latamSite.showSignupModal()">Não tem conta? Cadastre-se</a>
                </p>
            </form>
        `);
    }

    showSignupModal() {
        this.showModal('Cadastro', `
            <form id="signupForm" onsubmit="latamSite.handleSignup(event)">
                <div class="form-group">
                    <label for="signupNome">Nome completo</label>
                    <input type="text" id="signupNome" required>
                </div>
                <div class="form-group">
                    <label for="signupEmail">E-mail</label>
                    <input type="email" id="signupEmail" required>
                </div>
                <div class="form-group">
                    <label for="signupPassword">Senha</label>
                    <input type="password" id="signupPassword" required>
                </div>
                <div class="form-group">
                    <label for="signupConfirm">Confirmar senha</label>
                    <input type="password" id="signupConfirm" required>
                </div>
                <button type="submit" class="btn-submit">Cadastrar</button>
                <p style="text-align: center; margin-top: 1rem;">
                    <a href="#" onclick="latamSite.showLoginModal()">Já tem conta? Faça login</a>
                </p>
            </form>
        `);
    }

    handleLogin(e) {
        e.preventDefault();
        this.showMessage('success', 'Login realizado com sucesso!');
        setTimeout(() => this.closeModal(), 1500);
    }

    handleSignup(e) {
        e.preventDefault();
        const password = document.getElementById('signupPassword').value;
        const confirm = document.getElementById('signupConfirm').value;
        
        if (password !== confirm) {
            this.showMessage('error', 'As senhas não conferem.');
            return;
        }
        
        this.showMessage('success', 'Cadastro realizado com sucesso!');
        setTimeout(() => this.closeModal(), 1500);
    }

    showModal(title, content) {
        this.modalBody.innerHTML = `
            <h2>${title}</h2>
            ${content}
        `;
        this.modal.classList.add('active');
        document.body.style.overflow = 'hidden';
    }

    closeModal() {
        this.modal.classList.remove('active');
        document.body.style.overflow = '';
    }

    showMessage(type, text) {
        const messageDiv = document.createElement('div');
        messageDiv.className = `${type}-message`;
        messageDiv.textContent = text;
        
        // Remove mensagens anteriores
        const oldMessages = document.querySelectorAll('.success-message, .error-message');
        oldMessages.forEach(msg => msg.remove());
        
        // Insere nova mensagem
        const main = document.querySelector('main');
        main.insertBefore(messageDiv, main.firstChild);
        
        // Remove após 3 segundos
        setTimeout(() => {
            messageDiv.remove();
        }, 3000);
    }

    showLoader() {
        this.voosLista.innerHTML = '<div class="loader"></div>';
    }

    initAnimations() {
        // Animação de entrada para elementos quando scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, { threshold: 0.1 });

        // Observa cards e outros elementos
        document.querySelectorAll('.destino-card, .servico-card, .voo-item').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'all 0.6s ease';
            observer.observe(el);
        });
    }

    initFormValidation() {
        // Validação de e-mail
        const emailInputs = document.querySelectorAll('input[type="email"]');
        emailInputs.forEach(input => {
            input.addEventListener('blur', () => {
                if (input.value && !this.validateEmail(input.value)) {
                    this.showFieldError(input, 'E-mail inválido');
                } else {
                    this.clearFieldError(input);
                }
            });
        });

        // Validação de telefone
        const telInputs = document.querySelectorAll('input[type="tel"]');
        telInputs.forEach(input => {
            input.addEventListener('input', (e) => {
                e.target.value = this.formatPhone(e.target.value);
            });
        });
    }

    validateEmail(email) {
        const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        return re.test(email);
    }

    formatPhone(phone) {
        return phone.replace(/\D/g, '')
            .replace(/^(\d{2})(\d)/g, '($1) $2')
            .replace(/(\d)(\d{4})$/, '$1-$2');
    }

    showFieldError(input, message) {
        const formGroup = input.closest('.form-group');
        let errorDiv = formGroup.querySelector('.error-text');
        
        if (!errorDiv) {
            errorDiv = document.createElement('small');
            errorDiv.className = 'error-text';
            errorDiv.style.color = 'red';
            formGroup.appendChild(errorDiv);
        }
        
        errorDiv.textContent = message;
        input.style.borderColor = 'red';
    }

    clearFieldError(input) {
        const formGroup = input.closest('.form-group');
        const errorDiv = formGroup.querySelector('.error-text');
        
        if (errorDiv) {
            errorDiv.remove();
        }
        
        input.style.borderColor = '';
    }
}

// Inicialização
document.addEventListener('DOMContentLoaded', () => {
    window.latamSite = new LatamSite();
});

// Export para uso em outros módulos (se necessário)
if (typeof module !== 'undefined' && module.exports) {
    module.exports = LatamSite;
} 

### Readme.md
// Classe principal do site
class LatamSite {
    constructor() {
        this.init();
    }

    init() {
        this.cacheElements();
        this.bindEvents();
        this.loadVoos();
        this.initAnimations();
        this.initFormValidation();
    }

    cacheElements() {
        // Header e navegação
        this.hamburger = document.querySelector('.hamburger');
        this.navMenu = document.querySelector('.nav-menu');
        this.navLinks = document.querySelectorAll('.nav-link');
        
        // Forms
        this.searchForm = document.getElementById('searchForm');
        this.contatoForm = document.getElementById('contatoForm');
        this.newsletterForm = document.querySelector('.newsletter-form');
        
        // Elementos dinâmicos
        this.voosLista = document.getElementById('voosLista');
        this.modal = document.getElementById('modal');
        this.modalBody = document.getElementById('modalBody');
        
        // Tabs
        this.tabBtns = document.querySelectorAll('.tab-btn');
        
        // Botões de detalhes
        this.detalhesBtns = document.querySelectorAll('.btn-detalhes');
    }

    bindEvents() {
        // Menu mobile
        this.hamburger?.addEventListener('click', () => this.toggleMenu());
        
        // Links de navegação
        this.navLinks.forEach(link => {
            link.addEventListener('click', (e) => this.handleNavClick(e));
        });
        
        // Scroll event para active link
        window.addEventListener('scroll', () => this.updateActiveLink());
        
        // Forms
        this.searchForm?.addEventListener('submit', (e) => this.handleSearch(e));
        this.contatoForm?.addEventListener('submit', (e) => this.handleContato(e));
        this.newsletterForm?.addEventListener('submit', (e) => this.handleNewsletter(e));
        
        // Tabs
        this.tabBtns.forEach(btn => {
            btn.addEventListener('click', (e) => this.handleTabClick(e));
        });
        
        // Botões de detalhes
        this.detalhesBtns.forEach(btn => {
            btn.addEventListener('click', (e) => this.handleDetalhes(e));
        });
        
        // Fechar modal
        document.querySelector('.modal-close')?.addEventListener('click', () => this.closeModal());
        window.addEventListener('click', (e) => {
            if (e.target === this.modal) this.closeModal();
        });
        
        // Login button
        document.querySelector('.btn-login')?.addEventListener('click', () => this.showLoginModal());
        
        // Signup button
        document.querySelector('.btn-signup')?.addEventListener('click', () => this.showSignupModal());
    }

    toggleMenu() {
        this.hamburger?.classList.toggle('active');
        this.navMenu?.classList.toggle('active');
    }

    handleNavClick(e) {
        e.preventDefault();
        const link = e.currentTarget;
        const targetId = link.getAttribute('href');
        
        if (targetId === '#') return;
        
        const targetSection = document.querySelector(targetId);
        if (targetSection) {
            targetSection.scrollIntoView({ behavior: 'smooth' });
            
            // Fecha menu mobile se aberto
            this.navMenu?.classList.remove('active');
            this.hamburger?.classList.remove('active');
            
            // Atualiza active link
            this.navLinks.forEach(l => l.classList.remove('active'));
            link.classList.add('active');
        }
    }

    updateActiveLink() {
        const sections = document.querySelectorAll('section');
        const scrollPosition = window.scrollY + 100;

        sections.forEach(section => {
            const sectionTop = section.offsetTop;
            const sectionBottom = sectionTop + section.offsetHeight;
            const sectionId = section.getAttribute('id');

            if (scrollPosition >= sectionTop && scrollPosition < sectionBottom) {
                this.navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${sectionId}`) {
                        link.classList.add('active');
                    }
                });
            }
        });
    }

    // Carregar voos dinamicamente
    loadVoos() {
        this.showLoader();
        
        // Simulando chamada API
        setTimeout(() => {
            const voos = [
                {
                    origem: 'GRU',
                    destino: 'GIG',
                    origemCidade: 'São Paulo',
                    destinoCidade: 'Rio de Janeiro',
                    partida: '08:00',
                    chegada: '09:00',
                    duracao: '1h',
                    preco: 299,
                    parcelas: 10
                },
                {
                    origem: 'GIG',
                    destino: 'CGH',
                    origemCidade: 'Rio de Janeiro',
                    destinoCidade: 'São Paulo',
                    partida: '10:30',
                    chegada: '11:30',
                    duracao: '1h',
                    preco: 279,
                    parcelas: 10
                },
                {
                    origem: 'GRU',
                    destino: 'BSB',
                    origemCidade: 'São Paulo',
                    destinoCidade: 'Brasília',
                    partida: '14:00',
                    chegada: '16:00',
                    duracao: '2h',
                    preco: 399,
                    parcelas: 12
                }
            ];
            
            this.renderVoos(voos);
        }, 1000);
    }

    renderVoos(voos) {
        const voosHTML = voos.map(voo => `
            <article class="voo-item">
                <div class="voo-horario">
                    <span class="hora">${voo.partida}</span>
                    <span class="cidade">${voo.origem} - ${voo.origemCidade}</span>
                </div>
                
                <div class="voo-duracao">
                    <i class="fas fa-plane"></i>
                    <span>${voo.duracao}</span>
                </div>
                
                <div class="voo-horario">
                    <span class="hora">${voo.chegada}</span>
                    <span class="cidade">${voo.destino} - ${voo.destinoCidade}</span>
                </div>
                
                <div class="voo-preco">
                    <div class="preco">R$ ${voo.preco}</div>
                    <div class="parcelamento">em até ${voo.parcelas}x</div>
                    <button class="btn-comprar" data-voo='${JSON.stringify(voo)}'>Comprar</button>
                </div>
            </article>
        `).join('');
        
        this.voosLista.innerHTML = voosHTML;
        
        // Adiciona eventos aos botões de compra
        document.querySelectorAll('.btn-comprar').forEach(btn => {
            btn.addEventListener('click', (e) => this.handleCompra(e));
        });
    }

    handleCompra(e) {
        const vooData = JSON.parse(e.currentTarget.dataset.voo);
        this.showModal('Reserva de Voo', `
            <h3>Confirmar reserva</h3>
            <p>Voo: ${vooData.origem} (${vooData.origemCidade}) → ${vooData.destino} (${vooData.destinoCidade})</p>
            <p>Horário: ${vooData.partida} - ${vooData.chegada}</p>
            <p>Preço: R$ ${vooData.preco}</p>
            <button class="btn-submit" onclick="latamSite.confirmarCompra()">Confirmar</button>
        `);
    }

    confirmarCompra() {
        this.showMessage('success', 'Reserva confirmada com sucesso!');
        setTimeout(() => this.closeModal(), 2000);
    }

    handleSearch(e) {
        e.preventDefault();
        const formData = new FormData(e.target);
        const searchData = Object.fromEntries(formData);
        
        this.showMessage('success', 'Buscando voos...');
        
        // Simula busca
        setTimeout(() => {
            this.showModal('Resultados da Busca', `
                <h3>Voos encontrados</h3>
                <p>Origem: ${searchData.from}</p>
                <p>Destino: ${searchData.to}</p>
                <p>Data: ${searchData.date}</p>
                <p>Passageiros: ${searchData.passengers}</p>
                <p>Redirecionando para resultados...</p>
            `);
        }, 1500);
    }

    handleContato(e) {
        e.preventDefault();
        const formData = new FormData(e.target);
        const contatoData = Object.fromEntries(formData);
        
        this.showMessage('success', 'Mensagem enviada com sucesso!');
        e.target.reset();
    }

    handleNewsletter(e) {
        e.preventDefault();
        const email = e.target.querySelector('input[type="email"]').value;
        
        if (this.validateEmail(email)) {
            this.showMessage('success', 'Inscrição realizada com sucesso!');
            e.target.reset();
        } else {
            this.showMessage('error', 'Por favor, insira um e-mail válido.');
        }
    }

    handleTabClick(e) {
        const tab = e.currentTarget;
        this.tabBtns.forEach(btn => btn.classList.remove('active'));
        tab.classList.add('active');
        
        // Aqui você pode carregar diferentes voos baseado na tab
        this.loadVoos();
    }

    handleDetalhes(e) {
        const card = e.currentTarget.closest('.destino-card');
        const destino = card.querySelector('h3').textContent;
        const preco = card.querySelector('.destino-preco').textContent;
        
        this.showModal(destino, `
            <img src="${card.querySelector('img').src}" alt="${destino}" style="width: 100%; border-radius: 5px; margin-bottom: 1rem;">
            <h3>${destino}</h3>
            <p>${preco}</p>
            <p>Descrição detalhada do destino, incluindo informações sobre pontos turísticos, clima, melhor época para visitar e dicas de viagem.</p>
            <button class="btn-submit" onclick="latamSite.reservarDestino('${destino}')">Reservar agora</button>
        `);
    }

    reservarDestino(destino) {
        this.showMessage('success', `Reserva para ${destino} iniciada!`);
        setTimeout(() => this.closeModal(), 1500);
    }

    showLoginModal() {
        this.showModal('Login', `
            <form id="loginForm" onsubmit="latamSite.handleLogin(event)">
                <div class="form-group">
                    <label for="loginEmail">E-mail</label>
                    <input type="email" id="loginEmail" required>
                </div>
                <div class="form-group">
                    <label for="loginPassword">Senha</label>
                    <input type="password" id="loginPassword" required>
                </div>
                <button type="submit" class="btn-submit">Entrar</button>
                <p style="text-align: center; margin-top: 1rem;">
                    <a href="#" onclick="latamSite.showSignupModal()">Não tem conta? Cadastre-se</a>
                </p>
            </form>
        `);
    }

    showSignupModal() {
        this.showModal('Cadastro', `
            <form id="signupForm" onsubmit="latamSite.handleSignup(event)">
                <div class="form-group">
                    <label for="signupNome">Nome completo</label>
                    <input type="text" id="signupNome" required>
                </div>
                <div class="form-group">
                    <label for="signupEmail">E-mail</label>
                    <input type="email" id="signupEmail" required>
                </div>
                <div class="form-group">
                    <label for="signupPassword">Senha</label>
                    <input type="password" id="signupPassword" required>
                </div>
                <div class="form-group">
                    <label for="signupConfirm">Confirmar senha</label>
                    <input type="password" id="signupConfirm" required>
                </div>
                <button type="submit" class="btn-submit">Cadastrar</button>
                <p style="text-align: center; margin-top: 1rem;">
                    <a href="#" onclick="latamSite.showLoginModal()">Já tem conta? Faça login</a>
                </p>
            </form>
        `);
    }

    handleLogin(e) {
        e.preventDefault();
        this.showMessage('success', 'Login realizado com sucesso!');
        setTimeout(() => this.closeModal(), 1500);
    }

    handleSignup(e) {
        e.preventDefault();
        const password = document.getElementById('signupPassword').value;
        const confirm = document.getElementById('signupConfirm').value;
        
        if (password !== confirm) {
            this.showMessage('error', 'As senhas não conferem.');
            return;
        }
        
        this.showMessage('success', 'Cadastro realizado com sucesso!');
        setTimeout(() => this.closeModal(), 1500);
    }

    showModal(title, content) {
        this.modalBody.innerHTML = `
            <h2>${title}</h2>
            ${content}
        `;
        this.modal.classList.add('active');
        document.body.style.overflow = 'hidden';
    }

    closeModal() {
        this.modal.classList.remove('active');
        document.body.style.overflow = '';
    }

    showMessage(type, text) {
        const messageDiv = document.createElement('div');
        messageDiv.className = `${type}-message`;
        messageDiv.textContent = text;
        
        // Remove mensagens anteriores
        const oldMessages = document.querySelectorAll('.success-message, .error-message');
        oldMessages.forEach(msg => msg.remove());
        
        // Insere nova mensagem
        const main = document.querySelector('main');
        main.insertBefore(messageDiv, main.firstChild);
        
        // Remove após 3 segundos
        setTimeout(() => {
            messageDiv.remove();
        }, 3000);
    }

    showLoader() {
        this.voosLista.innerHTML = '<div class="loader"></div>';
    }

    initAnimations() {
        // Animação de entrada para elementos quando scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, { threshold: 0.1 });

        // Observa cards e outros elementos
        document.querySelectorAll('.destino-card, .servico-card, .voo-item').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'all 0.6s ease';
            observer.observe(el);
        });
    }

    initFormValidation() {
        // Validação de e-mail
        const emailInputs = document.querySelectorAll('input[type="email"]');
        emailInputs.forEach(input => {
            input.addEventListener('blur', () => {
                if (input.value && !this.validateEmail(input.value)) {
                    this.showFieldError(input, 'E-mail inválido');
                } else {
                    this.clearFieldError(input);
                }
            });
        });

        // Validação de telefone
        const telInputs = document.querySelectorAll('input[type="tel"]');
        telInputs.forEach(input => {
            input.addEventListener('input', (e) => {
                e.target.value = this.formatPhone(e.target.value);
            });
        });
    }

    validateEmail(email) {
        const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        return re.test(email);
    }

    formatPhone(phone) {
        return phone.replace(/\D/g, '')
            .replace(/^(\d{2})(\d)/g, '($1) $2')
            .replace(/(\d)(\d{4})$/, '$1-$2');
    }

    showFieldError(input, message) {
        const formGroup = input.closest('.form-group');
        let errorDiv = formGroup.querySelector('.error-text');
        
        if (!errorDiv) {
            errorDiv = document.createElement('small');
            errorDiv.className = 'error-text';
            errorDiv.style.color = 'red';
            formGroup.appendChild(errorDiv);
        }
        
        errorDiv.textContent = message;
        input.style.borderColor = 'red';
    }

    clearFieldError(input) {
        const formGroup = input.closest('.form-group');
        const errorDiv = formGroup.querySelector('.error-text');
        
        if (errorDiv) {
            errorDiv.remove();
        }
        
        input.style.borderColor = '';
    }
}

// Inicialização
document.addEventListener('DOMContentLoaded', () => {
    window.latamSite = new LatamSite();
});

// Export para uso em outros módulos (se necessário)
if (typeof module !== 'undefined' && module.exports) {
    module.exports = LatamSite;
} 
