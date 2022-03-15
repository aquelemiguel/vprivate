<script lang="ts">
</script>

<main>
    <div class="header-container">
        <img on:click={() => window.location.href = '/'} class="header-logo" src="images/vprivate-transparent.png" alt="V Private Logo">
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

    .header-logo {
        height: 70%;
        width: 100%;
        object-fit: contain;
        cursor: pointer;
    }
</style>