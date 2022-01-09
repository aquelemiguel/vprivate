<main>
    <div class="container">
        <div class="service-grid">
            <div class="service-image">
                <img src="images/example.jpg" alt="" />
            </div>
            <div class="service-title">
                <h2>Crédito Habitação</h2>
            </div>
            <div class="service-description">
                <p>Qualquer que seja a sua necessidade, estamos aqui para o ajudar a encontrar a melhor proposta de crédito.</p>
                <p>A parceria com as principais Instituições Bancárias permite-nos ter acesso às soluções mais avançadas e nas melhores condições.</p>
                <p>Disponibilize-nos os documentos e as informações necessárias e nós tratamos do processo de crédito sem qualquer custo para si.</p>
                <p>O nosso compromisso é a procura da melhor solução.</p>
            </div>
            <button class="service-button">Vamos conversar?</button>
        </div>
    </div>
</main>

<style>
    h2 {
        margin: unset;
    }

    main {
        background-color: #FFFF;
    }

    .container {
        height: 100vh;
        max-width: 70%;
        margin: 0 auto;
    }

    .service-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 10px;
        transform: translateY(50%);
    }

    .service-image {
        grid-column: 1;
        grid-row: 1/4;
    }

    .service-title {
        grid-column: 2;
        grid-row: 1;
        font-size: 32px;
    }

    .service-description {
        grid-column: 2;
        grid-row: 2;
        font-size: 20px;
    }

    .service-description p:not(:last-child) {
        padding-bottom: 0.25rem;
    }

    .service-button {
        grid-column: 2;
        grid-row: 3;
    }
</style>