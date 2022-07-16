<!-- <div class="wrap">
    <ul class="clients">
      <li><a href=""></a></li>
      <li><a href=""><img src="images/partners/bpi.png" alt="Airbnb"></a></li>
      <li><a href=""><img src="images/partners/caixa-geral-de-depositos.png" alt="Apple"></a></li>
      <li><a href=""><img src="images/partners/novo-banco.png" alt="Microsoft"></a></li>
      <li><a href=""><img src="images/partners/novo-banco.png" alt="Microsoft"></a></li>
      <li><a href=""><img src="images/partners/novo-banco.png" alt="Microsoft"></a></li>

    </ul>
</div> -->

<div class="container">
    <img src="images/partners/bpi.png" alt="UAE">
    <img src="images/partners/novo-banco.png" alt="UAE">
    <img src="images/partners/caixa-geral-de-depositos.png" alt="UAE">
    <img src="images/partners/santander.png" alt="UAE">
    <img src="images/partners/cofidis.png" alt="UAE">
    <img src="images/partners/bankinter.png" alt="UAE">
</div>

<style>
    .container {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }

    img {
        align-self: center;
        width: 8rem;
        padding: 1rem 1rem;
    }
</style>

<!-- <div class="scroll-parent">
    <div class="scroll-element primary">
        <img src="images/partners/bpi.png" alt="UAE">
        <img src="images/partners/novo-banco.png" alt="UAE">
        <img src="images/partners/caixa-geral-de-depositos.png" alt="UAE">
        <img src="images/partners/santander.png" alt="UAE">
        <img src="images/partners/cofidis.png" alt="UAE">
        <img src="images/partners/bankinter.png" alt="UAE">
    </div>
    <div class="scroll-element secondary">
        <img src="images/partners/bpi.png" alt="UAE">
        <img src="images/partners/novo-banco.png" alt="UAE">
        <img src="images/partners/caixa-geral-de-depositos.png" alt="UAE">
        <img src="images/partners/santander.png" alt="UAE">
        <img src="images/partners/cofidis.png" alt="UAE">
        <img src="images/partners/bankinter.png" alt="UAE">
    </div>

</div>

<style>
    .scroll-parent {
        position: relative;
        width: 100%;
        height: 10rem;
        overflow-x: hidden;
    }

    .scroll-element {
        width: inherit;
        height: inherit;
        position: absolute;
        left: 0%;
        top: 0%;
        display: flex;
        align-items: center;
        justify-content: space-around;
        animation: primary 20s linear infinite;
    }

    img {
        width: 10rem;
        /* padding: 0 5rem; */
    }

    .primary {
        animation: primary 20s linear infinite;
    }

    .secondary {
        animation: secondary 20s linear infinite;
    }

    @keyframes primary {
        from {
            left: 0%;
        }
        to {
            left: -100%;
        }
    }

    @keyframes secondary {
        from {
            left: 100%;
        }
        to {
            left: 0%;
        }
    }
</style> -->