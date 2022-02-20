<script>
</script>

<main>
    <div class="main-page-wrapper">
        <div class="main-page">
            <div class="overlay-container">
                <h2 class="overlay-title">
                    Os nossos Clientes sempre em primeiro lugar.
                </h2>
                <span class="overlay-content">
                    A pensar nos nossos Clientes temos vindo a alargar os nossos serviços.
                    Ajudamos e facilitamos as tarefas dos nossos Clientes.
                </span>
                <div class="button-row">
                    <button>Seguros</button>
                    <button>Créditos</button>
                </div>
            </div>
        </div>
    </div>

    <div class="subpage-wrapper">
        <h2 class="subpage-title">
            Somos um grupo experiente na:
        </h2>

        <div class="subpage-card-row">
            <div class="subpage-card">
                <img class="subpage-card-logo" src="img/icons/icon-1.png" alt="" />
                <h3 class="subpage-card-title">Consultoria e gestão de seguros</h3>
                <span class="subpage-card-content">
                    Com uma equipa de profissionais com mais de 25 anos de experiência, atuando no
                    mercado nacional e internacional e com parceiros sólidos e de grande confiança;
                </span>
            </div>

            <div class="subpage-card">
                <img class="subpage-card-logo" src="img/icons/icon-1.png" alt="" />
                <h3 class="subpage-card-title">Intermediação de crédito</h3>
                <span class="subpage-card-content">
                    Uma via simples e gratuita para obter os financiamentos para a realização dos
                    seus projetos;
                </span>
            </div>
        
            <div class="subpage-card">
                <img class="subpage-card-logo" src="img/icons/icon-1.png" alt="" />
                <h3 class="subpage-card-title">Consultoria financeira e gestão de património</h3>
            </div>
        </div>

        <h3 class="subpage-subtitle">
            A nossa missão é servir os nossos Clientes com rigor, responsabilidade, ética e
            confidencialidade, valores que os nossos profissionais sempre implementaram.
        </h3>

        <div class="subpage-card-row">
            <div class="subpage-big-card">
                <h3 class="subpage-big-card-title">Seguros</h3>
            </div>
            <div class="subpage-big-card">
                <h3 class="subpage-big-card-title">Créditos</h3>
            </div>
        </div>
    </div>

    <div class="footer-container">
        <div class="footer-row">
            <div class="footer-column">
                <h4 class="footer-title">Contacte-nos</h4>
                <div class="footer-map">Map goes here</div>
                <div class="footer-address">
                    <h4>Vila Nova de Gaia</h4>
                    <span>
                        Rua Raimundo de Carvalho, 354<br>
                        4430-185, Mafamude, Vila Nova de Gaia
                    </span>
                </div>
            </div>

            <div class="footer-column">
                <div class="footer-phone">
                    <img src="" alt="" class="footer-phone-logo" />
                    <span class="footer-phone-info">
                        <span><strong>Telefone:</strong>+351 220 044 700</span><br>
                        <span><strong>Fax:</strong>(+351) 220 044 709</span>
                    </span>
                </div>
                <div class="footer-map">Map goes here</div>
                <div class="footer-address">
                    <h4>Porto</h4>
                    <span>
                        Rua Manuel Pinto de Azevedo, 323<br>
                        4100-321 Porto
                    </span>
                </div>
            </div>

            <div class="footer-column">
                <div class="footer-email">
                    <img src="" alt="" class="footer-email-logo" />
                    <span class="footer-email-info">
                        <span><strong>Geral:</strong>geral@vprivate.pt</span><br>
                        <span><strong>Sinistros:</strong>sinistros@vprivate.pt</span><br>
                        <span><strong>Cobranças:</strong>cobrancas@vprivate.pt</span>
                    </span>
                </div>
                <div class="footer-map">Map goes here</div>
                <div class="footer-address">
                    <h4>Valongo</h4>
                    <span>
                        Rua da Passagem, 432 loja 34<br>
                        4440-565 Valongo
                    </span>
                </div>
            </div>
        </div>
    </div>
</main>

<style>
    .main-page-wrapper {
        background-color: #fbf8e9;
    }

    .main-page, .subpage-wrapper, .footer-row {
        max-width: 73%;
        margin: 0 auto;
    }

    .main-page {
        height: 94vh;
        position: relative;
    }

    .overlay-container {
        position: absolute;
        top: 19vh;
        background-color: #cfb136;
        width: 60vh;
        padding: 4rem;
        height: 48vh;
    }

    .overlay-title {
        font-size: 2.75rem;
    }

    .overlay-content {
        font-size: 1.1rem;
        margin-top: 1rem;
    }

    .button-row {
        margin-top: 2rem;
    }

    button {
        border: none;
        width: 12.5rem;
        height: 3.5rem;
    }

    .subpage-wrapper {
        margin-bottom: 5rem;
    }

    .subpage-title {
        font-size: 2.5rem;
        margin-top: 4rem;
        text-align: center;
    }

    .subpage-card-row {
        display: flex;
    }

    .subpage-card {
        /* background-color: #fbf8e9; */
        background-color: #cfb136;
        display: flex;
        flex-direction: column;
        height: 30vh;
        align-items: center;
        flex: 1 1 0px;
        padding: 3rem;
        text-align: center;
    }

    .subpage-card:not(:last-of-type) {
        margin-right: 2rem;
    }

    .subpage-card-logo {
        width: 5rem;
        height: 5rem;
    }

    .subpage-card-title {
        margin-top: 3rem;
    }

    .subpage-subtitle {
        text-align: center;
        max-width: 50%;
        width: 100%;
        margin: 5rem auto;
    }

    .subpage-big-card {
        background-color: #cfb136;
        height: 25vh;
        display: flex;
        flex-grow: 1;
        padding: 3rem;
        text-align: center;
        font-size: 2rem;
    }

    .subpage-big-card:not(:last-of-type) {
        margin-right: 2rem;
    }

    .subpage-big-card-title {
        margin: auto;
    }

    .footer-container {
        background-color: #cfb136;
        height: 75vh;
        width: 100%;
    }

    .footer-title {
        font-size: 2rem;
        margin: unset;
    }

    .footer-row {
        display: flex;
    }

    .footer-column {
        display: flex;
        flex-direction: column;
        flex: 1;
        height: 60vh;
    }

    .footer-column:not(:last-of-type) {
        margin-right: 2rem;
    }

    .footer-title, .footer-phone, .footer-email {
        flex-grow: 1;
    }

    .footer-title, .footer-phone, .footer-email {
        display: flex;
        align-items: center;
        line-height: 1.5rem;
    }

    .footer-phone-logo, .footer-email-logo {
        width: 5rem;
        height: 5rem;
        margin-right: 1rem;
    }

    .footer-map {
        background-color: white;
        height: 25vh;
    }
</style>