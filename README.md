# Devchris
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Cards</title>
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&amp;display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<style>
    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Poppins", sans-serif;
}

body {
    background: #F6F9FF;
    height: 100vh;
    width: 100%;

    display: flex;
    justify-content: center;
    align-items: center;

    color: #434343;

    font-size: 16px;
}

main.cards {
    display: flex;
    padding: 32px;
}

main.cards section.card {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    background: white;
    padding: 1rem 1.5rem;
    border-radius: 8px;
    max-height: 468px;
    margin-left: 32px;
}

main.cards section.card:first-child {
    margin-left: 0;
}

main.cards section.card .icon {
    width: 64px;
    height: 64px;
}

main.cards section.card img {
    width: 100%;
}

main.cards section.card h3 {
    font-size: 100%;
    margin: 16px 0;
}

main.cards section.card span {
    font-weight: 300;
    max-width: 240px;
    font-size: 80%;
    margin-bottom: 16px;
}

main.cards section.card button {
    padding: 0.5rem 1rem;
    text-transform: uppercase;
    border-radius: 32px;
    border: 0;
    cursor: pointer;
    font-size: 80%;
    font-weight: 500;
    color: #fff;
    margin-bottom: 16px 0;
}

main.cards section.card.contact button {
    background: linear-gradient(to right, #9F66FF, #DFCBFF);
}
main.cards section.card.shop button {
    background: linear-gradient(to right, #3E8AFF, #BBDEFF);
}
main.cards section.card.about button {
    background: linear-gradient(to right, #FE5F8F, #FFC7D9);
}

main.cards section.card.contact {
    box-shadow: 20px 20px 50px -30px #DBC4FF;
}
main.cards section.card.shop {
    box-shadow: 20px 20px 50px -30px #AFD6FF;
}
main.cards section.card.about {
    box-shadow: 20px 20px 50px -30px #FFC1D5;
}

@media screen and (max-width: 720px) {
    main.cards {
        flex-direction: column;
    }

    main.cards section.card {
        margin-left: 0;
        margin-bottom: 32px;
    }

    main.cards section.card:last-child {
        margin-bottom: 0;
    }

    main.cards section.card button {
        font-size: 70%;
    }

}

</style>
<body>
    <main class="cards">
        <section class="card contact">
            <div class="icon">
                <img src="https://64.media.tumblr.com/9583bbab5a1aa1efad7d58fdac35d404/0dccc87e3b53b088-97/s500x750/73d24ce45280254d4348b7986b90aa70ec40f04a.png" alt="Contact us.">
            </div>
            <h3>Contato</h3>
            <span>(11)94795-**** / badetechcontato@gmail.com</span>
            <button>Saber mais</button>
        </section>
        <section class="card shop">
            <div class="icon">
                <img src="https://64.media.tumblr.com/5e5c923844b301b4d5b94c1b687cc6c9/8210175639ad6614-5f/s500x750/9f35318bce9a9ed79038acf3393a762c3a8f6b1a.png" alt="Shop here.">
            </div>
            <h3>Compre aqui.</h3>            <span>Somos a empresa BADETECH e fornecemos o melhor sistema para a sua empresa.</span>
            <button>Saber mais</button>
        </section>
        <section class="card about">
            <div class="icon">
                <img src="https://64.media.tumblr.com/5c50b07cc5aff124ea429b8668c8e029/b39f06dbbfb7c111-90/s500x750/ca9f655b3106fae848ca3fe77f2e4fe14c4963c4.png" alt="About us.">
            </div>
            <h3>Sobre nós</h3>
            <span>Somos a empresa BADETECH e fornecemos o melhor sistema para a sua empresa.</span>
            <button>Saber mais</button>
        </section>
    </main>

</body>
