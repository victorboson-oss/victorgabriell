# victorgabriell
```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Blog Projeto - Victor Gabriell</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0f0f0f;
            color: white;
        }

        /* CABEÇALHO */
        header {
            min-height: 400px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;

            background:
                linear-gradient(#0009, #0009),
                url("https://images.unsplash.com/photo-1518770660439-4636190af475")
                center/cover;
        }

        header h1 {
            font-size: 55px;
            color: #00ff88;
            margin-bottom: 15px;
        }

        header p {
            font-size: 20px;
        }

        /* MENU */
        nav {
            background: #111;
            padding: 18px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 2px solid #00ff88;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00ff88;
        }

        /* CONTEÚDO */
        main {
            max-width: 1100px;
            margin: auto;
            padding: 40px 20px;
        }

        section {
            margin-bottom: 60px;
        }

        .titulo {
            color: #00ff88;
            text-align: center;
            font-size: 35px;
            margin-bottom: 30px;
        }

        /* SOBRE */
        .sobre {
            text-align: center;
            background: #181818;
            padding: 35px;
            border-radius: 20px;
            box-shadow: 0 0 20px #00ff8830;
        }

        .sobre h2 {
            color: #00ff88;
            margin-bottom: 15px;
        }

        .sobre p {
            max-width: 750px;
            margin: auto;
            line-height: 1.8;
            font-size: 18px;
        }

        /* CARDS */
        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 25px;
        }

        .card {
            background: #181818;
            padding: 25px;
            border-radius: 18px;
            text-align: center;
            transition: 0.3s;
            border: 1px solid #333;
        }

        .card:hover {
            transform: translateY(-8px);
            border-color: #00ff88;
            box-shadow: 0 0 20px #00ff8830;
        }

        .card h3 {
            color: #00ff88;
            margin-bottom: 12px;
        }

        .card p {
            line-height: 1.6;
        }

        .emoji {
            font-size: 45px;
            margin-bottom: 15px;
        }

        /* INTERESSES */
        .interesses {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }

        .tag {
            background: #00ff88;
            color: #000;
            padding: 12px 20px;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .tag:hover {
            transform: scale(1.1);
            background: white;
        }

        /* BOTÃO */
        button {
            margin-top: 20px;
            padding: 13px 25px;
            border: none;
            border-radius: 30px;
            background: #00ff88;
            color: #000;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            transform: scale(1.08);
            background: white;
        }

        /* RODAPÉ */
        footer {
            background: #050505;
            text-align: center;
            padding: 30px;
            border-top: 2px solid #00ff88;
        }

        footer p {
            color: #aaa;
        }

        /* CELULAR */
        @media (max-width: 600px) {

            header h1 {
                font-size: 38px;
            }

            nav a {
                display: inline-block;
                margin: 6px;
            }

            .titulo {
                font-size: 28px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>💻 Blog Projeto</h1>
        <p>Bem-vindo ao meu mundo!</p>
    </header>

    <nav>
        <a href="#sobre">Sobre mim</a>
        <a href="#hobbies">Hobbies</a>
        <a href="#gostos">Meus gostos</a>
        <a href="#objetivo">Meu objetivo</a>
    </nav>

    <main>

        <!-- SOBRE MIM -->
        <section id="sobre">

            <h2 class="titulo">👨‍💻 Sobre Mim</h2>

            <div class="sobre">

                <h2>Victor Gabriell Boson da Silva</h2>

                <p>
                    Olá! Meu nome é Victor Gabriell, tenho 16 anos
                    e moro em Guaribas. Atualmente estudo programação
                    e estou aprendendo cada vez mais sobre tecnologia
                    e desenvolvimento de sistemas.
                </p>

                <p style="margin-top: 15px;">
                    Criei este blog para apresentar um pouco sobre mim,
                    meus interesses, meus hobbies e meus objetivos.
                </p>

            </div>

        </section>


        <!-- HOBBIES -->
        <section id="hobbies">

            <h2 class="titulo">🎨 Meus Hobbies</h2>

            <div class="cards">

                <div class="card">
                    <div class="emoji">🎨</div>
                    <h3>Desenhar</h3>
                    <p>
                        Gosto de desenhar e criar diferentes tipos
                        de desenhos.
                    </p>
                </div>

                <div class="card">
                    <div class="emoji">🎤</div>
                    <h3>Cantar</h3>
                    <p>
                        Uma das coisas que gosto de fazer é cantar
                        e me divertir com a música.
                    </p>
                </div>

                <div class="card">
                    <div class="emoji">🎸</div>
                    <h3>Tocar música</h3>
                    <p>
                        Também gosto de tocar instrumentos e
                        explorar o mundo da música.
                    </p>
                </div>

                <div class="card">
                    <div class="emoji">💻</div>
                    <h3>Programação</h3>
                    <p>
                        Estou estudando programação e quero evoluir
                        cada vez mais nessa área.
                    </p>
                </div>

            </div>

        </section>


        <!-- MEUS GOSTOS -->
        <section id="gostos">

            <h2 class="titulo">⭐ Meus Gostos</h2>

            <div class="interesses">

                <div class="tag">🎬 A Barraca do Beijo</div>

                <div class="tag">👻 Supernatural</div>

                <div class="tag">🎮 Minecraft</div>

                <div class="tag">🎤 Michael Jackson</div>

                <div class="tag">🎵 Música</div>

                <div class="tag">🎨 Desenhos</div>

                <div class="tag">💻 Programação</div>

            </div>

        </section>


        <!-- OBJETIVO -->
        <section id="objetivo">

            <h2 class="titulo">🚀 Meu Objetivo</h2>

            <div class="sobre">

                <h2>Meu futuro</h2>

                <p>
                    Meu objetivo é crescer profissionalmente,
                    aprender bastante sobre programação e construir
                    uma carreira de sucesso na área de tecnologia.
                </p>

                <p style="margin-top: 15px;">
                    Quero conquistar minha independência financeira
                    e alcançar meus objetivos através do meu trabalho
                    e conhecimento.
                </p>

                <button onclick="mostrarMensagem()">
                    ✨ Conheça meu projeto
                </button>

            </div>

        </section>

    </main>


    <footer>
        <p>
            © 2026 Blog Projeto — Victor Gabriell
        </p>

        <p style="margin-top: 8px;">
            Feito com HTML, CSS e JavaScript 💻
        </p>
    </footer>


    <script>

        function mostrarMensagem() {

            alert(
                "🚀 Este é o meu projeto! " +
                "Estou estudando programação e quero continuar evoluindo."
            );

        }

    </script>

</body>

</html>
```
