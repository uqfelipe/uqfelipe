
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Felipe (@felipebytes) - Desenvolvedor Full-Stack</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
        }

        header {
            text-align: center;
            margin-bottom: 50px;
        }

        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #fff, #4A86FF);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .subtitle {
            font-size: 1.5em;
            color: #4A86FF;
            margin-bottom: 20px;
        }

        .typing-animation {
            font-size: 1.2em;
            color: #fff;
            margin: 20px 0;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin: 20px 0;
        }

        .badge {
            padding: 8px 16px;
            background: rgba(74, 134, 255, 0.3);
            border-radius: 5px;
            font-weight: bold;
            border: 2px solid #4A86FF;
        }

        section {
            margin: 50px 0;
            padding: 30px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        h2 {
            font-size: 2.5em;
            margin-bottom: 30px;
            text-align: center;
            color: #4A86FF;
        }

        .about-code {
            background: #1e1e1e;
            padding: 25px;
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            overflow-x: auto;
            color: #d4d4d4;
            line-height: 1.8;
        }

        .code-line {
            margin: 5px 0;
        }

        .key {
            color: #9cdcfe;
        }

        .string {
            color: #ce9178;
        }

        .bracket {
            color: #ffd700;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin: 30px 0;
        }

        .tech-category {
            background: rgba(255, 255, 255, 0.08);
            padding: 25px;
            border-radius: 12px;
            border: 2px solid rgba(74, 134, 255, 0.3);
            transition: transform 0.3s ease;
        }

        .tech-category:hover {
            transform: translateY(-5px);
            border-color: #4A86FF;
        }

        .tech-category h3 {
            color: #4A86FF;
            margin-bottom: 15px;
            font-size: 1.5em;
        }

        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .tech-badge {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: bold;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s ease;
        }

        .tech-badge:hover {
            transform: scale(1.05);
        }

        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.08);
            padding: 20px;
            border-radius: 12px;
            text-align: center;
            border: 2px solid rgba(74, 134, 255, 0.3);
        }

        .stat-card img {
            max-width: 100%;
            border-radius: 8px;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 30px 0;
        }

        .project-card {
            background: rgba(255, 255, 255, 0.08);
            padding: 30px;
            border-radius: 15px;
            border: 2px solid rgba(74, 134, 255, 0.3);
            transition: transform 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            border-color: #4A86FF;
            box-shadow: 0 10px 30px rgba(74, 134, 255, 0.3);
        }

        .project-card h3 {
            color: #4A86FF;
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        .project-card p {
            font-size: 1.1em;
            line-height: 1.6;
        }

        .experience-table {
            width: 100%;
            border-collapse: collapse;
            margin: 30px 0;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            overflow: hidden;
        }

        .experience-table th,
        .experience-table td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .experience-table th {
            background: rgba(74, 134, 255, 0.3);
            font-weight: bold;
            font-size: 1.1em;
        }

        .experience-table tr:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .contact-section {
            text-align: center;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .contact-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 25px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }

        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(74, 134, 255, 0.4);
        }

        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, #4A86FF, transparent);
            margin: 50px 0;
        }

        footer {
            text-align: center;
            margin-top: 50px;
            padding: 30px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 15px;
        }

        footer p {
            font-size: 1.2em;
            margin: 10px 0;
        }

        .emoji {
            font-size: 1.5em;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2em;
            }

            h2 {
                font-size: 1.8em;
            }

            .container {
                padding: 20px;
            }

            .tech-grid,
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Animações */
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        section {
            animation: fadeIn 0.6s ease-out;
        }

        .pulse {
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% {
                opacity: 1;
            }
            50% {
                opacity: 0.7;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header>
            <h1><span class="emoji">👋</span> Olá! Eu sou o Felipe</h1>
            <div class="subtitle">@felipebytes</div>
            <div class="typing-animation pulse">
                Desenvolvedor Full-Stack | Especialista em Mobile | Apaixonado por Tecnologia
            </div>
            <div class="badges">
                <span class="badge">Developer Full-Stack</span>
                <span class="badge">Mobile iOS | Android</span>
                <span class="badge">DevOps Cloud Ready</span>
            </div>
        </header>

        <div class="divider"></div>

        <!-- Sobre Mim -->
        <section id="about">
            <h2><span class="emoji">🚀</span> Sobre Mim</h2>
            <div class="about-code">
<span class="code-line"><span class="key">const</span> felipe = <span class="bracket">{</span></span>
<span class="code-line">    <span class="key">localização:</span> <span class="string">"Vargem Alegre, MG 🇧🇷"</span>,</span>
<span class="code-line">    <span class="key">especialidades:</span> [<span class="string">"Full-Stack"</span>, <span class="string">"Mobile"</span>, <span class="string">"DevOps"</span>],</span>
<span class="code-line">    <span class="key">tecnologias:</span> <span class="bracket">{</span></span>
<span class="code-line">        <span class="key">frontend:</span> <span class="bracket">{</span></span>
<span class="code-line">            <span class="key">web:</span> [<span class="string">"JavaScript"</span>, <span class="string">"TypeScript"</span>],</span>
<span class="code-line">            <span class="key">mobile:</span> [<span class="string">"Swift"</span>, <span class="string">"Kotlin"</span>, <span class="string">"React Native"</span>, <span class="string">"Flutter"</span>]</span>
<span class="code-line">        <span class="bracket">}</span>,</span>
<span class="code-line">        <span class="key">backend:</span> [<span class="string">"Python"</span>, <span class="string">"Node.js"</span>, <span class="string">"Go"</span>, <span class="string">"Java"</span>],</span>
<span class="code-line">        <span class="key">database:</span> [<span class="string">"PostgreSQL"</span>, <span class="string">"SQL"</span>, <span class="string">"MongoDB"</span>],</span>
<span class="code-line">        <span class="key">devops:</span> [<span class="string">"Docker"</span>, <span class="string">"Terraform"</span>, <span class="string">"CI/CD"</span>, <span class="string">"Bash"</span>]</span>
<span class="code-line">    <span class="bracket">}</span>,</span>
<span class="code-line">    <span class="key">foco:</span> <span class="string">"Criar aplicações escaláveis do front ao deploy"</span>,</span>
<span class="code-line">    <span class="key">paixão:</span> <span class="string">"Aprender novas tecnologias todos os dias"</span>,</span>
<span class="code-line">    <span class="key">atualmente:</span> <span class="string">"Desenvolvendo projetos próprios e contribuindo em open-source"</span></span>
<span class="code-line"><span class="bracket">}</span>;</span>
            </div>
        </section>

        <div class="divider"></div>

        <!-- Stack Tecnológico -->
        <section id="tech-stack">
            <h2><span class="emoji">🛠️</span> Stack Tecnológico</h2>
            <div class="tech-grid">
                <div class="tech-category">
                    <h3><span class="emoji">🎨</span> Frontend Web</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">JavaScript</span>
                        <span class="tech-badge">TypeScript</span>
                        <span class="tech-badge">React</span>
                        <span class="tech-badge">HTML5</span>
                        <span class="tech-badge">CSS3</span>
                    </div>
                </div>

                <div class="tech-category">
                    <h3><span class="emoji">📱</span> Mobile</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">Swift</span>
                        <span class="tech-badge">Kotlin</span>
                        <span class="tech-badge">React Native</span>
                        <span class="tech-badge">Flutter</span>
                        <span class="tech-badge">Dart</span>
                    </div>
                </div>

                <div class="tech-category">
                    <h3><span class="emoji">⚙️</span> Backend</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">Python</span>
                        <span class="tech-badge">Node.js</span>
                        <span class="tech-badge">Go</span>
                        <span class="tech-badge">Java</span>
                        <span class="tech-badge">Ruby</span>
                    </div>
                </div>

                <div class="tech-category">
                    <h3><span class="emoji">💾</span> Banco de Dados</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">PostgreSQL</span>
                        <span class="tech-badge">MongoDB</span>
                        <span class="tech-badge">SQL</span>
                        <span class="tech-badge">PL/pgSQL</span>
                    </div>
                </div>

                <div class="tech-category">
                    <h3><span class="emoji">🔧</span> DevOps</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">Docker</span>
                        <span class="tech-badge">Terraform</span>
                        <span class="tech-badge">Bash</span>
                        <span class="tech-badge">CI/CD</span>
                        <span class="tech-badge">YAML</span>
                    </div>
                </div>

                <div class="tech-category">
                    <h3><span class="emoji">🧰</span> Ferramentas</h3>
                    <div class="tech-badges">
                        <span class="tech-badge">Git</span>
                        <span class="tech-badge">VSCode</span>
                        <span class="tech-badge">Xcode</span>
                        <span class="tech-badge">Android Studio</span>
                    </div>
                </div>
            </div>
        </section>

        <div class="divider"></div>

        <!-- Estatísticas GitHub -->
        <section id="stats">
            <h2><span class="emoji">📊</span> Estatísticas GitHub</h2>
            <div class="stats-container">
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api?username=felipebytes&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true" alt="GitHub Stats">
                </div>
                <div class="stat-card">
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=felipebytes&layout=compact&langs_count=8&theme=tokyonight" alt="Top Languages">
                </div>
            </div>
            <div class="stat-card" style="margin-top: 20px;">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=felipebytes&theme=tokyonight" alt="GitHub Streak">
            </div>
        </section>

        <div class="divider"></div>

        <!-- Projetos em Destaque -->
        <section id="projects">
            <h2><span class="emoji">🌟</span> Projetos em Destaque</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3><span class="emoji">🛒</span> E-Commerce Full-Stack</h3>
                    <p>Plataforma completa com web (React + TypeScript) e mobile (React Native), back-end em Python/Node.js, PostgreSQL e deploy automatizado com Docker.</p>
                </div>

                <div class="project-card">
                    <h3><span class="emoji">📱</span> App Mobile Nativo</h3>
                    <p>Desenvolvimento nativo com Swift (iOS) e Kotlin (Android), incluindo arquitetura MVVM, integração com APIs REST e CI/CD automatizado.</p>
                </div>

                <div class="project-card">
                    <h3><span class="emoji">🌐</span> Website de Portfólio</h3>
                    <p>Site elegante e responsivo construído com TypeScript, hospedado em infraestrutura como código (Terraform) com pipeline CI/CD.</p>
                </div>

                <div class="project-card">
                    <h3><span class="emoji">🚀</span> Microserviços com Go</h3>
                    <p>API de alta performance em Go, PostgreSQL, containerizada com Docker e orquestrada com GitHub Actions para deploy automático.</p>
                </div>
            </div>
        </section>

        <div class="divider"></div>

        <!-- Experiência em Desenvolvimento -->
        <section id="experience">
            <h2><span class="emoji">📈</span> Experiência em Desenvolvimento</h2>
            <table class="experience-table">
                <thead>
                    <tr>
                        <th>Área</th>
                        <th>Tecnologias Principais</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Web Frontend</strong></td>
                        <td>TypeScript, JavaScript, React</td>
                    </tr>
                    <tr>
                        <td><strong>Mobile Native</strong></td>
                        <td>Swift (iOS), Kotlin (Android)</td>
                    </tr>
                    <tr>
                        <td><strong>Mobile Cross</strong></td>
                        <td>React Native, Flutter (Dart)</td>
                    </tr>
                    <tr>
                        <td><strong>Backend</strong></td>
                        <td>Python, Node.js, Go, Java</td>
                    </tr>
                    <tr>
                        <td><strong>Databases</strong></td>
                        <td>PostgreSQL, SQL, MongoDB</td>
                    </tr>
                    <tr>
                        <td><strong>DevOps/Infra</strong></td>
                        <td>Docker, Terraform, Bash, CI/CD</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <div class="divider"></div>

        <!-- Entre em Contato -->
        <section id="contact" class="contact-section">
            <h2><span class="emoji">📫</span> Entre em Contato</h2>
            <div class="contact-links">
                <a href="https://instagram.com/felipebytes" target="_blank" class="contact-btn">
                    <span class="emoji">📷</span> Instagram
                </a>
                <a href="https://twitter.com/felipebytes" target="_blank" class="contact-btn">
                    <span class="emoji">🐦</span> Twitter
                </a>
                <a href="https://wa.me/5533998352941" target="_blank" class="contact-btn">
                    <span class="emoji">💬</span> WhatsApp
                </a>
                <a href="https://t.me/ufelipe" target="_blank" class="contact-btn">
                    <span class="emoji">✈️</span> Telegram
                </a>
                <a href="mailto:ufelipe@icloud.com" class="contact-btn">
                    <span class="emoji">✉️</span> Email
                </a>
                <a href="https://www.youtube.com/felipebytes" target="_blank" class="contact-btn">
                    <span class="emoji">🎥</span> YouTube
                </a>
            </div>
        </section>

        <!-- Footer -->
        <footer>
            <p><span class="emoji">✨</span> <strong>Do front-end ao deploy: criando soluções completas!</strong> <span class="emoji">✨</span></p>
            <p style="margin-top: 20px; font-size: 0.9em; opacity: 0.8;">
                Desenvolvido com <span class="emoji">❤️</span> por Felipe (@felipebytes)
            </p>
        </footer>
    </div>

