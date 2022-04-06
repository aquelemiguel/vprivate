<script lang="ts">
    import Header from '../components/Header.svelte';
    import Footer from '../components/Footer.svelte';
</script>

<Header></Header>
<div class="container">
    <div class="banner">
        <h1>Parceiros</h1>
    </div>

    <div class="partner-row">
        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>

        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>

        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>
    </div>

    <div class="partner-row">
        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>

        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>

        <div class="partner-container">
            <img class="partner-logo" src="images/partners/logo.png" alt="">
            <span class="partner-name">Santander</span>
        </div>
    </div>
</div>
<Footer></Footer>

<style>
    h1 {
        font-size: 3.5rem;
    }

    .container {
        min-height: 100vh;
        max-width: 50%;
		margin: 0 auto;
        display: flex;
        justify-content: center;
        flex-direction: column;
    }

    .banner {
        width: 100%;
        min-height: 8rem;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .partner-row {
        display: flex;
        justify-content: space-around;
        margin: 1rem 0;
    }

    .partner-container {
        display: flex;
		flex-direction: column;
		align-items: center;
        border-radius: 0.5rem;
        box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px, rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
        padding: 2rem 4rem 0 4rem;
        background-color: white;
    }

    .partner-logo {
        width: 10rem;
    }

    .partner-name {
        font-weight: bold;
        padding: 1.5rem 0;
    }

</style>