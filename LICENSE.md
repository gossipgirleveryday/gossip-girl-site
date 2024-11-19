<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gossip Girl - Plotki z Upper East Side</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Yeseva+One&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="header">
        <div class="logo">
            <h1>Gossip Girl</h1>
            <p>Plotki z Upper East Side</p>
        </div>
        <nav class="navigation">
            <ul>
                <li><a href="#latest">Najświeższe Plotki</a></li>
                <li><a href="#about">O Gossip Girl</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="latest" class="latest-posts">
            <h2>Najświeższe Plotki</h2>
            <div class="post">
                <h3>Wielki powrót Sereny van der Woodsen!</h3>
                <p>Serena wraca do Nowego Jorku po latach nieobecności. Co ją skłoniło do powrotu? Plotki mówią o romansie z jednym z przystojnych przestępców...</p>
            </div>
            <div class="post">
                <h3>Blair Waldorf na randce z tajemniczym milionerem</h3>
                <p>Blair uchwycona na kolacji z przystojnym, nieznanym mężczyzną. Czyżby była to jej nowa miłość? Więcej wkrótce...</p>
            </div>
        </section>

        <section id="about" class="about">
            <h2>O Gossip Girl</h2>
            <p>Gossip Girl to tajemnicza postać, która śledzi życie młodych, bogatych i pięknych mieszkańców Upper East Side. Jej blog stał się źródłem plotek, skandali i sensacji. Nikt nie wie, kim jest – ale jedno jest pewne: wiesz o wszystkim, zanim zdążysz o tym pomyśleć...</p>
        </section>

        <section id="contact" class="contact">
            <h2>Kontakt z Gossip Girl</h2>
            <p>Masz coś, o czym Gossip Girl powinna wiedzieć? Wyślij swoją wiadomość anonimowo. Plotka, która zostanie opublikowana, może zmienić życie!</p>
            <form action="#">
                <textarea placeholder="Twoja plotka..." rows="4"></textarea>
                <button type="submit">Wyślij</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Gossip Girl. Wszystkie prawa zastrzeżone.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

/* styles.css */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto', sans-serif;
}

body {
    background-color: #2c2c2c;
    color: #fff;
    line-height: 1.6;
}

header {
    background-color: #111;
    padding: 20px;
    text-align: center;
}

header .logo h1 {
    font-family: 'Yeseva One', cursive;
    font-size: 3rem;
    color: #ffb3b3;
    margin-bottom: 0;
}

header .logo p {
    font-size: 1.2rem;
    color: #ddd;
}

nav ul {
    list-style: none;
    margin-top: 20px;
}

nav ul li {
    display: inline;
    margin: 0 20px;
}

nav ul li a {
    text-decoration: none;
    color: #ffb3b3;
    font-size: 1.2rem;
}

nav ul li a:hover {
    text-decoration: underline;
}

main {
    padding: 40px 20px;
}

.latest-posts .post {
    background-color: #444;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 8px;
}

.latest-posts .post h3 {
    font-size: 1.8rem;
    color: #ffb3b3;
}

.latest-posts .post p {
    font-size: 1rem;
    color: #ccc;
}

.about, .contact {
    margin-top: 40px;
}

.about h2, .contact h2 {
    font-size: 2rem;
    color: #ffb3b3;
}

.contact form textarea {
    width: 100%;
    padding: 10px;
    border: 2px solid #ffb3b3;
    border-radius: 5px;
    margin-top: 10px;
    background-color: #333;
    color: #fff;
    font-size: 1rem;
}

.contact form button {
    background-color: #ffb3b3;
    color: #333;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    margin-top: 10px;
    font-size: 1rem;
    cursor: pointer;
}

.contact form button:hover {
    background-color: #ff6666;
}

footer {
    text-align: center;
    margin-top: 40px;
    background-color: #111;
    padding: 20px;
    font-size: 0.8rem;
    color: #bbb;
}
// script.js
document.querySelector('form').addEventListener('submit', function(e) {
    e.preventDefault();
    alert("Twoja plotka została wysłana! Gossip Girl już wie...");
});
