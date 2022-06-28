<script lang="ts">
    import { onMount } from "svelte";

    let url = '';
    onMount(() => url = getCurrentPage());

    const getCurrentPage = () => {
        const urlParts = window.location.href.split('/');
        return urlParts[urlParts.length - 1];
    }
</script>

<main>
    <div class="header-container">
        <div class="header-row">
            <img on:click={() => window.location.href = '/'} class="header-logo" src="images/vprivate-transparent.png" alt="V Private Logo">
            <span class="navbar-option navbar-link" on:click={() => window.location.href = '/'}>Início</span>
            <span class="navbar-option navbar-link {url.includes('sobre') ? 'selected' : ''}" on:click={() => window.location.href = '/sobre'}>Quem somos</span>
            <span class="navbar-option navbar-link {url.includes('servicos') ? 'selected' : ''}" on:click={() => window.location.href = '/servicos'}>Serviços</span>
            <button class="navbar-option lets-talk-button">Vamos conversar?</button>
        </div>
    </div>
</main>

<style>
    main {
        height: 6rem;
        width: 100%;
        background: white;
        box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
        position: fixed;
        top: 0;
    }

    .header-container {
        max-width: 50%;
        margin: 0 auto;
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .header-row {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
    }

    .header-logo {
        height: 70%;
        object-fit: contain;
        cursor: pointer;
    }

    .navbar-option {
        cursor: pointer;
        text-transform: uppercase;
        transition: all 0.2s ease-in-out;
    }

    .navbar-option:hover, .navbar-option.selected {
        color: #c89e28;
        font-weight: bold;
    }

    .navbar-link {
        flex: 1 1 0px;
        text-align: center;
    }

    .lets-talk-button {
        margin-left: 1rem;
        margin-bottom: unset;
    }
</style>