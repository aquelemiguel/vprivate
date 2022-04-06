<script>
    export let data;
</script>

<main id="{data.id}">
    <div class="container">
        <div class="service-title">
            <h1>{data.title}</h1>
        </div>

        <div class="subservice-flex">
            {#each data.features as feature}
                <div class="subservice-item">{ feature }</div>
            {/each}
        </div>

        <div class="service-grid">
            <div class="service-image">
                <img src="images/example.jpg" alt="" />
            </div>
            <div class="service-description">
                {#each data.description as line}
                    <p>{line}</p>
                {/each}
            </div>
            <button class="lets-talk-button" on:click={() => window.location.href = '/contactos'}>Vamos conversar?</button>
        </div>
    </div>
</main>

<style lang="scss">
    main {
        min-height: 100vh;
        padding-top: 2.5rem;
    }

    .lets-talk-button {
        font-size: 1.2em;
        font-weight: bold;
    }

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        max-width: 55%;
        margin: 0 auto;
        min-height: 100vh;
    }

    p {
        font-size: 20px;
    }

    p:first-child {
        margin-top: 0;
    }

    .service-title {
        align-self: flex-start;
        font-size: 32px;
    }

    .subservice-flex {
        display: flex;
        width: 100%;
        justify-content: space-between;
        margin: 3rem 0 2rem 0;
    }

    .subservice-item {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		width: 240px;
		height: 60px;
		padding: 0 1em;
		margin: 0.5em;
        box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
        border-radius: 5px;
        padding: 10px;
        font-weight: bold;
        background-color: #c89e28;
        color: white;
    }

    .service-grid {
        display: grid;
        grid-auto-rows: auto 5rem;
        gap: 2rem;
        margin: 2rem 0;
    }

    .service-image {
        grid-column: 1;
        grid-row: 1/3;

        img {
            max-width: 100%;
            border-radius: 1.5em;
            box-shadow: rgba(0, 0, 0, 0.75) 0px 20px 30px -10px;
        }
    }

    .service-description {
        grid-column: 2;
        grid-row: 1;
    }

    .service-button {
        margin-left: 2rem;
        grid-column: 2;
        grid-row: 2;
    }
</style>