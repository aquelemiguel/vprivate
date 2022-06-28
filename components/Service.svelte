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
        <!-- <img class="card-image" src="../../images/landing2.jpg" alt="Card" /> -->
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
        margin: 2rem;
        overflow: hidden;
        width: 65%;
        border-radius: 10px;
        box-shadow: 0 10px 10px rgba(0, 0, 0, 0.2);
    }

    .card-preview {
        background-color: #c89e28;
        // background-blend-mode: multiply;
        // background-image: url(../../images/landing2.jpg);
        color: white;
        // padding: 2rem;
        flex: 0 0 40%;
        overflow: hidden;
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
</style>