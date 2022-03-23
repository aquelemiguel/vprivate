<div class="footer-container">
    <div class="footer-column">
        <h2>Navegação</h2>
        <div on:click={() => window.location.href = '/sobre'}>Quem somos</div>
        <div on:click={() => {
            window.location.href = '/';
            window.scrollTo(0);
        }}>Serviços</div>
        <div on:click={() => window.location.href = '/parceiros'}>Parceiros</div>
    </div>
    <div class="footer-column">
        <h2>Navegação</h2>
        <div on:click={() => window.location.href = '/contactos'}>Contactos</div>
        <div on:click={() => window.location.href = '/privacidade'}>Política de Privacidade</div>
        <div>Termos & Condições</div>
    </div>
    <div class="footer-column">
        <h2>Informação Legal</h2>
        <div>Intermediário de Crédito Vinculado nº 6 715</div>
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
        height: 40vh;
        box-shadow: rgba(0, 0, 0, 0.1) 0px -4px 12px;
        background: #c89e28;
        color: white;
    }

    .footer-column {
        display: flex;
        flex-basis: 20em;
        flex-direction: column;
        align-self: center;
    }
    
    .footer-column h2 {
        margin: 0 0 2rem 0;
    }

    .footer-column div {
        margin: 0.25rem 0;
    }
</style>