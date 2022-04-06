<div class="wrap">
    <ul class="clients">
      <li><a href=""><img src="images/partners/santander.png" alt="UAE"></a></li>
      <li><a href=""><img src="images/partners/bpi.png" alt="Airbnb"></a></li>
      <li><a href=""><img src="images/partners/caixa-geral-de-depositos.png" alt="Apple"></a></li>
      <li><a href=""><img src="images/partners/novo-banco.png" alt="Microsoft"></a></li>
    </ul>
</div>

<style>
    .wrap {
    padding: 0 4.8rem;
    position: relative;
    width: 90%;
    }

    .clients {
        align-items: center;
        -webkit-box-align: center;
        display: grid;
        gap: 4.8rem 4.8rem;
        grid-template-columns: auto auto;
        justify-items: center;
        margin: 4.8rem auto;
        max-width: 1024px; }

    .clients li {
    list-style: none;
    margin: 0;
    -webkit-transition: all .3s ease-in-out;
    transition: all .3s ease-in-out;
    }
    .clients img {
    height: 3.2rem;

    }
    .clients:hover li {
    filter: blur(0px);
    -webkit-filter: blur(0px);
    }
    .clients:hover li:not(:hover)  {
    filter: blur(2px);
    -webkit-filter: blur(2px);
    }
    .clients li:hover {
    -webkit-transform: translateY(-0.3rem);
    transform: translateY(-0.3rem); 
    }

    @media (min-width: 1024px) {
    .clients {
        grid-template-columns: auto auto auto auto; }
        
    .clients img {
    height: 4rem; }}

    /* --- Images (gray logo) --- */
    .clients img {
        filter: grayscale(100%)
    }

    .clients img:hover {
    background: none;
    -webkit-filter: grayscale(0%);
            filter: grayscale(0%);
    -webkit-transition: all .3s ease-in-out;
    transition: all .3s ease-in-out; }
</style>