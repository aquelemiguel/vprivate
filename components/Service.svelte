<script>
    export let data;
</script>

<!-- <main id="{data.id}">
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
</main> -->

<div class="card-container" id="{data.id}">
    <div class="card-preview">
        <h1 class="card-header">{data.title}</h1>
        <div class="card-image"></div>
    </div>

    <div class="card-info">
        <div class="card-description">
            {#each data.description as line}
                <p>{line}</p>
            {/each}
        </div>

        <div class="card-chips">
            {#each data.features as feature}
                <div class="card-chip">{ feature }</div>
            {/each}
        </div>
    </div>
</div>

<style lang="scss">
    .card-container {
        display: flex;
        max-width: 100%;
        overflow: hidden;
        width: 100%;
        border-radius: 10px;
        box-shadow: 0 10px 10px rgba(0, 0, 0, 0.2);
    }

    .card-preview {
        color: white;
        flex: 0 0 40%;
    }

    .card-image {
        width: 100%;
        height: 100%;
        background-image: url(../../images/landing2.jpg);
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        background-color: #c89e28;
        background-blend-mode: multiply;
    }

    .card-header {
        position: absolute;
        width: 20rem;
        padding: 1.5rem;
        font-size: 38px;
        text-shadow: 0 5px 5px rgba(0, 0, 0, 0.3);
    }

    .card-button {
        position: relative;
        bottom: 0px;
    }

    .card-info {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 2rem;
    }

    .card-description > p {
        font-size: 18px;
    }

    .card-chips {
        display: flex;
        flex-wrap: wrap;
        width: 100%;
        margin-top: 0.5rem;
        justify-content: flex-start;
    }

    .card-chip {
        border: 1px solid #c89e28;
        border-radius: 1rem;
        margin: 0.25rem 0;
        padding: 0.5rem;
        font-size: 12px;
        background: #c89e28;
        color: white;
        cursor: pointer;
        font-weight: bold;
    }

    .card-chip:not(:last-of-type) {
        margin-right: 0.5rem;
    }

    // main {
    //     min-height: 100vh;
    //     padding-top: 2.5rem;
    // }

    // .lets-talk-button {
    //     font-size: 1.2em;
    //     font-weight: bold;
    // }

    // .container {
    //     display: flex;
    //     flex-direction: column;
    //     align-items: center;
    //     justify-content: center;
    //     max-width: 55%;
    //     margin: 0 auto;
    //     min-height: 100vh;
    // }

    // p {
    //     font-size: 20px;
    // }

    // p:first-child {
    //     margin-top: 0;
    // }

    // .service-title {
    //     align-self: flex-start;
    //     font-size: 32px;
    // }

    // .subservice-flex {
    //     display: flex;
    //     width: 100%;
    //     justify-content: space-between;
    //     margin: 3rem 0 2rem 0;
    // }

    // .subservice-item {
	// 	display: flex;
	// 	flex-direction: column;
	// 	align-items: center;
	// 	justify-content: center;
	// 	text-align: center;
	// 	width: 240px;
	// 	height: 60px;
	// 	padding: 0 1em;
	// 	margin: 0.5em;
    //     box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    //     border-radius: 5px;
    //     padding: 10px;
    //     font-weight: bold;
    //     background-color: #c89e28;
    //     color: white;
    // }

    // .service-grid {
    //     display: grid;
    //     grid-auto-rows: auto 5rem;
    //     gap: 2rem;
    //     margin: 2rem 0;
    // }

    // .service-image {
    //     grid-column: 1;
    //     grid-row: 1/3;

    //     img {
    //         max-width: 100%;
    //         border-radius: 1.5em;
    //         box-shadow: rgba(0, 0, 0, 0.75) 0px 20px 30px -10px;
    //     }
    // }

    // .service-description {
    //     grid-column: 2;
    //     grid-row: 1;
    // }

    // .service-button {
    //     margin-left: 2rem;
    //     grid-column: 2;
    //     grid-row: 2;
    // }
</style>