<script>
    export let data, altTheme;
</script>

<main class="{altTheme ? 'alt-theme' : 'default-theme'}">
    <div class="container">
        <div class="service-grid">
            <div class="service-image">
                <img src="images/example.jpg" alt="" />
            </div>
            <div class="service-title">
                <h1>{data.title}</h1>
            </div>
            <div class="service-description">
                {#each data.description as line}
                    <p>{line}</p>
                {/each}
            </div>
            <button class="service-button">Vamos conversar?</button>
        </div>

        <!-- <div class="subservices-row">
            {#each data.features as feature}
                <div class="subservice-cell">{feature}</div>
            {/each}
        </div> -->
    </div>
</main>

<style lang="scss">
    :root {
        --main-bg-color: rgb(250, 250, 250);
        --alt-bg-color: #0047bf;
    }

    main {
        height: 100vh;
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

    // invert colors on button hover 
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
        max-width: 60%;
        margin: 0 auto;
        transform: translateY(50%);
    }

    h1 {
        font-size: 52px;
    }

    p {
        font-size: 20px;
    }

    .service-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1rem;

    }

    .service-image {
        grid-column: 1;
        grid-row: 1/4;

        img {
            border-radius: 1.5em;
            box-shadow: rgba(0, 0, 0, 0.75) 0px 20px 30px -10px;
        }
    }

    .service-title {
        display: flex;
        align-items: center;
        grid-column: 2;
        grid-row: 1;
    }

    .service-description {
        grid-column: 2;
        grid-row: 2;
        text-align: justify;
    }

    .service-button {
        grid-column: 2;
        grid-row: 3;
    }
</style>