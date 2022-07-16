<script>
    export let data;
</script>

<div class="card-anchor" id="{data.id}"></div>
<div class="card-container">
    <div class="card-preview">
        <h1 class="card-header">{data.title}</h1>
        <div class="card-image" style={
            `background-image: url(../images/${data.image})`
        }></div>
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
        min-height: 50vh;
        border-radius: 10px;
        box-shadow: 0 10px 10px rgba(0, 0, 0, 0.2);
        background-color: white;
    }

    .card-anchor {
        display: block;
        position: relative;
        top: -16rem;
        visibility: hidden;
    }

    .card-preview {
        position: relative;
        color: white;
        flex: 0 0 40%;
        overflow: hidden;
    }

    .card-image {
        width: 100%;
        height: 100%;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        // background-color: #c89e28;
        // background-blend-mode: multiply;
        filter: brightness(0.9)
    }

    .card-header {
        position: absolute;
        padding: 1.5rem;
        font-size: 38px;
        text-shadow: 0 0 15px rgba(0, 0, 0, 0.8);
        z-index: 1;
    }

    .card-info {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: 5rem;
    }

    .card-description > p {
        font-size: 18px;
    }

    .card-description > p:first-of-type, .card-description > p:last-of-type {
        margin: unset;
    }

    .card-chips {
        display: flex;
        flex-wrap: wrap;
        width: 100%;
        margin-top: 1.5rem;
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