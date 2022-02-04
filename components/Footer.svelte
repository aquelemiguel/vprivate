<div class="footer-container">
    <div class="footer-column">
        <h2>Navegação</h2>
        <div on:click={() => window.location.href = '/about'}>Quem somos</div>
        <div on:click={() => window.location.href = '/services'}>Serviços</div>
        <div on:click={() => window.location.href = '/partners'}>Parceiros</div>
    </div>
    <div class="footer-column">
        <h2>Navegação</h2>
        <div>Contactos</div>
        <div>Política de Privacidade</div>
        <div>Termos & Condições</div>
    </div>
    <div class="footer-column">
        <h2>Informação Legal</h2>
        <div>ICV nº XXXXXXX</div>
        <div>RAL</div>
        <div>Livro de Reclamações</div>
    </div>
</div>

<style>
    h2 {
        margin: unset;
    }

    .footer-container {
        display: flex;
        justify-content: center;
        bottom: 0;
        width: 100%;
        background-color: #003690;
        height: 40vh;
    }

    .footer-column {
        display: flex;
        flex-basis: 20em;
        flex-direction: column;
        color: #eae6e5;
        align-self: center;
    }
    
    .footer-column h2 {
        margin: 0 0 2rem 0;
    }

    .footer-column div {
        margin: 0.25rem 0;
    }
</style>