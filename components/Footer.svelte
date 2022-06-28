<div class="footer-container">
    <div class="footer-column footer-contacts">
        <img class="brand-logo" src="images/vprivate-transparent-white.png" alt="V Private Logo">
        <span class="contact-info">manuel.leal@vprivate.pt</span>
        <span class="contact-info">+351 938 885 971 // +351 220 044 700</span>
        <span class="contact-info">Dias úteis das 9h00 às 18h00</span>
    </div>

    <div class="footer-column footer-navigation">
        <h2>Navegação</h2>
        <div class="footer-link" on:click={() => window.location.href = '/sobre'}>Quem somos</div>
        <div class="footer-link" on:click={() => {
            window.location.href = '/';
            window.scrollTo(0);
        }}>Serviços</div>
        <div class="footer-link" on:click={() => window.location.href = '/privacidade'}>Política de Privacidade</div>
    </div>
    <div class="footer-column footer-legal">
        <h2>Informação Legal</h2>
        <div>ICV nº 6715</div>
        <div class="footer-link">RAL</div>
        <div class="footer-link">Livro de Reclamações</div>
    </div>
</div>

<style>
    .brand-logo {
        width: 200px;
        margin-bottom: 1rem;
    }

    .contact-info {
        padding-left: 0.5rem;
    }

    h2 {
        margin: unset;
    }

    .footer-container {
        display: flex;
        justify-content: center;
        bottom: 0;
        height: 40vh;
        box-shadow: rgba(0, 0, 0, 0.1) 0px -4px 12px;
        background: rgb(40, 30, 3);
        color: white;
        padding: 0 10rem;
    }

    .footer-column {
        display: flex;
        flex-direction: column;
        align-self: center;
    }

    .footer-contacts {
        flex-basis: 40%;
        border-right: 1px solid rgb(207, 157, 31);
        margin-right: 5rem;
    }

    .footer-navigation, .footer-legal {
        flex-basis: 20%;
    }
    
    .footer-column h2 {
        margin: 0 0 2rem 0;
    }

    .footer-column div {
        margin: 0.25rem 0;
    }

    .footer-link:hover {
        font-weight: bold;
        cursor: pointer;
    }
</style>