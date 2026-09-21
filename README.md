# victorgabriell
```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Meu Blog</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f2f2f2;
            color: #222;
        }

        header {
            background: linear-gradient(135deg, #6a0dad, #9b30ff);
            color: white;
            text-align: center;
            padding: 50px 20px;
        }

        header h1 {
            font-size: 45px;
            margin-bottom: 10px;
        }

        header p {
            font-size: 18px;
        }

        nav {
            background: #222;
            text-align: center;
            padding: 15px;
            position: sticky;
            top: 0;
            z-index: 10;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }

        nav a:hover {
            color: #c77dff;
        }

        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 20px;
        }

        .sobre {
            background: white;
            padding: 30px;
            border-radius: 15px;
            margin-bottom: 30px;
            text-align: center;
            box-shadow: 0 5px 15px #0002;
        }

        .sobre img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 15px;
        }

        .posts {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .post {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px #0002;
            transition: 0.3s;
        }

        .post:hover {
            transform: translateY(-5px);
        }

        .post img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .conteudo {
            padding: 20px;
        }

        .conteudo h2 {
            color: #6a0dad;
            margin-bottom: 10px;
        }

        .conteudo p {
            line-height: 1.6;
            margin-bottom: 15px;
        }

        button {
            background: #6a0dad;
            color: white;
            border: none;
            padding: 10px 18px;
            border-radius: 20px;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            background: #9b30ff;
            transform: scale(1.05);
        }

        footer {
            background: #222;
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 40px;
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 32px;
            }

            nav a {
                margin: 0 5px;
                font-size: 14px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>✨ Meu Blog</h1>
        <p>Um pouco sobre mim, meus interesses e minhas histórias.</p>
    </header>

    <nav>
        <a href="#inicio">Início</a>
        <a href="#sobre">Sobre mim</a>
        <a href="#posts">Posts</a>
        <a href="#contato">Contato</a>
    </nav>

    <main id="inicio">

        <section class="sobre" id="sobre">

            <!-- Troque o link abaixo pela sua foto -->
            <img src="https://picsum.photos/300" alt="Minha foto">

            <h2>Olá, eu sou seu nome! 👋</h2>

            <p>
                Bem-vindo ao meu blog! Aqui eu compartilho um pouco
                sobre minha vida, meus interesses, projetos e coisas
                que gosto de fazer.
            </p>

        </section>

        <h2 id="posts" style="margin-bottom: 20px;">
            📝 Meus Posts
        </h2>

        <section class="posts">

            <article class="post">

                <img src="https://picsum.photos/600/400?random=1"
                    alt="Imagem do post">

                <div class="conteudo">

                    <h2>Meu primeiro post</h2>

                    <p>
                        Este é o meu primeiro post no blog.
                        Aqui posso escrever sobre mim e contar
                        um pouco da minha história.
                    </p>

                    <button onclick="curtir(this)">
                        ❤️ Curtir <span>0</span>
                    </button>

                </div>

            </article>


            <article class="post">

                <img src="https://picsum.photos/600/400?random=2"
                    alt="Imagem do post">

                <div class="conteudo">

                    <h2>Meus hobbies</h2>

                    <p>
                        Aqui posso falar sobre meus hobbies,
                        filmes, séries, jogos, músicas e outras
                        coisas que gosto.
                    </p>

                    <button onclick="curtir(this)">
                        ❤️ Curtir <span>0</span>
                    </button>

                </div>

            </article>


            <article class="post">

                <img src="https://picsum.photos/600/400?random=3"
                    alt="Imagem do post">

                <div class="conteudo">

                    <h2>Meus projetos</h2>

                    <p>
                        Neste espaço posso apresentar meus
                        projetos de programação, trabalhos
                        escolares e outras criações.
                    </p>

                    <button onclick="curtir(this)">
                        ❤️ Curtir <span>0</span>
                    </button>

                </div>

            </article>

        </section>

        <section class="sobre" id="contato" style="margin-top: 30px;">

            <h2>📱 Entre em contato</h2>

            <p style="margin: 15px 0;">
                Você pode colocar aqui suas redes sociais
                e formas de contato.
            </p>

            <button onclick="mostrarMensagem()">
                Entrar em contato
            </button>

        </section>

    </main>

    <footer>
        <p>© 2026 - Meu Blog | Feito por mim 💜</p>
    </footer>


    <script>

        function curtir(botao) {

            let numero = botao.querySelector("span");

            let curtidas = Number(numero.textContent);

            curtidas++;

            numero.textContent = curtidas;

            botao.style.transform = "scale(1.1)";

            setTimeout(() => {
                botao.style.transform = "scale(1)";
            }, 200);

        }


        function mostrarMensagem() {

            alert("Obrigado por visitar meu blog! 😊");

        }

    </script>

</body>

</html>
```
