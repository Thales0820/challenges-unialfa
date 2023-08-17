### html

~~~html

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>One Piece</title>
    <link rel="shortcut icon" href="Imagens/Icon.png">
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css">
</head>
<body>
    <header>
        <a class="logo" href="index.html">
            <img src="Imagens/logo.png" alt="One Piece">
        </a>
        <nav>
            <ul>
                <li>
                    <a href="https://mangalivre.net/manga/one-piece/13" title="Mangá">
                        <i class="bi bi-journal-bookmark-fill"></i>
                        Ler o Mangá 
                    </a>
                </li>
                <li>
                    <a href="https://www.crunchyroll.com/pt-br/series/GRMG8ZQZR/one-piece" title="Anime">
                        <i class="bi bi-play-circle-fill"></i>
                        Assistir o Anime
                    </a>
                </li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="texto">
            <h1>Uma Simples Sinopse de One Piece:</h1>

            <p><strong>A série foca em Monkey D. Luffy, um jovem feito de borracha, que, inspirado em seu ídolo de infância, o poderoso pirata Shanks, o Ruivo, parte em uma jornada do mar do East Blue para encontrar o tesouro mítico, o One Piece, e proclamar-se o Rei dos Piratas.</strong></p>
        </section>
        <section>
            <h3 class="texto">Principais Protagonistas</h3>

            <div  class="grid">
                <div class="coluna">
                    <img src="Imagens/Luffy.jpg" alt="Luffy">
                    <p><strong>Monkey D. Luffy</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Monkey_D._Luffy">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Zoro.jpg" alt="Zoro">
                    <p><strong>Roronoa Zoro</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Roronoa_Zoro">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Nami.jpg" alt="Nami">
                    <p><strong>Nami</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Nami">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Ussopp.jpg" alt="Ussopp">
                    <p><strong>Ussopp</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Usopp">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Sanji.jpg" alt="Sanji">
                    <p><strong>Vismoke Sanji</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Sanji">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Chopper.jpg" alt="Chopper">
                    <p><strong>Tony Tony Chopper</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Tony_Tony_Chopper">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Nico Robin.jpg" alt="Robin">
                    <p><strong>Nico Robin</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Nico_Robin">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Franky.jpg" alt="Franky">
                    <p><strong>Franky</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Franky">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Brook.jpg" alt="Brook">
                    <p><strong>Brook</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Brook">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
                <div class="coluna">
                    <img src="Imagens/Jinbei.jpg" alt="Jinbei">
                    <p><strong>Jinbei</strong></p>
                    <a href="https://onepiece.fandom.com/pt/wiki/Jinbe">
                        <i class="bi bi-plus-circle"></i>
                        Mais detalhes
                    </a>
                </div>
            </div>
        </section>
    </main>
</body>
</html>

~~~~

###css

~~~html

<style>

* {
    margin: 0;
    padding: 0;
    font-family: 16px Raleway, Arial, Verdana;
}

header {
    width: 100%;
    background-color: rgb(24, 141, 250);
    padding: 10px;
    display: inline-block;
    top: 0;
    position: fixed;
    height: 80px;
}

.logo img{
    width: 250px;
    height: 85px;
}

nav {
    float: right;
}

nav ul {
    list-style: none;
}

nav ul li {
    display: inline-block;
    margin: 30px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: 700;
}

nav ul li a:hover {
    color: red;
}

.texto {
    margin-top: 100px;
    text-align: center;
}

.texto h1, h3 {
    margin-bottom: 15px;
}

.grid {
    display: grid;
    grid-template-columns: 33% 33% 33%;
}

.coluna {
    text-align: center;
    border: 1px solid #ccc;
    margin: 10px;
    border-radius: 10px;
    box-shadow: 0 0 20px #ccc;
}    

.coluna img {
    width: 100%;
    border-radius: 10px 10px 0 0;
    height: 500px;
}

.coluna p {
    font-size: 18px;
    height: 40px;
    margin: 10px;
}

.coluna a {
    background-color: rgb(24, 141, 250);
    color: white;
    margin: 20px;
    padding: 5px 30px;
    border-radius: 100px;
    display: inline-block;
    text-decoration: none;
}

.coluna a:hover {
    color: red;
}

</style>

~~~