<script>
    export let data, altTheme;
</script>

<main id="{data.id}" class="{altTheme ? 'alt-theme' : 'default-theme'}">
    <div class="container">
        <div class="service-title">
            <h1>{data.title}</h1>
        </div>

        <!-- <span class="service-subtitle">
            O que pretende?
        </span> -->

        <div class="subservice-flex">
            {#each data.features as feature}
                <div class="subservice-item">{ feature }</div>
            {/each}
        </div>

        <div class="service-grid">
            <div class="service-image">
                <img src="images/example.jpg" alt="" />
            </div>
            <!-- <div class="service-title">
                <h1>{data.title}</h1>
            </div> -->
            <div class="service-description">
                {#each data.description as line}
                    <p>{line}</p>
                {/each}
            </div>
            <button class="service-button">Vamos conversar?</button>
        </div>
    </div>
</main>

<style lang="scss">
    :root {
        --main-bg-color: rgb(250, 250, 250);
        --alt-bg-color: #003690;
    }

    main {
        min-height: 100vh;
    }

    button {
        background-color: var(--alt-bg-color);
        box-shadow: rgba(50, 50, 93, 0.25) 0px 30px 60px -12px, rgba(0, 0, 0, 0.3) 0px 18px 36px -18px;
        color: var(--main-bg-color);
        border: none;
        border-radius: 5px;
        padding: 10px;
        font-size: 1.2em;
        font-weight: bold;
        cursor: pointer;
        transition: all 0.2s ease-in-out;
    }

    button:hover {
        background-color: var(--main-bg-color);
        color: var(--alt-bg-color);
    }

    .default-theme {
        background: linear-gradient(270deg, #ffffff, #f2f2f2);
        background-size: 400% 400%;

        -webkit-animation: gradient 5s ease infinite;
        -moz-animation: gradient 5s ease infinite;
        animation: gradient 5s ease infinite;

        color: black;
    }

    .alt-theme {
        background: linear-gradient(270deg, #003690, #0047bf);
        background-size: 400% 400%;

        -webkit-animation: gradient 5s ease infinite;
        -moz-animation: gradient 5s ease infinite;
        animation: gradient 5s ease infinite;

        color: white;
    }

    @keyframes gradient {
        0% {
            background-position: 0% 50%;
        }
        50% {
            background-position: 100% 50%;
        }
        100% {
            background-position: 0% 50%;
        }
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

    h1 {
        font-size: 52px;
    }

    p {
        font-size: 20px;
    }

    p:first-child {
        margin-top: 0;
    }

    .service-title {
        align-self: center;
    }

    .service-subtitle {
        font-size: 1rem;
        margin: 2rem 0;
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
		height: 100px;
		padding: 0 1em;
		margin: 0.5em;
        box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
        border-radius: 5px;
        padding: 10px;
        font-weight: bold;
        // background-color: var(--alt-bg-color);
    }

    .service-grid {
        display: grid;
        grid-template-columns: auto;
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
        margin-left: 2rem;
        grid-column: 2;
        grid-row: 1;
    }

    .service-button {
        margin-left: 2rem;
        grid-column: 2;
        grid-row: 2;
    }
</style>