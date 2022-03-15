<script lang="ts">
    import Header from '../components/Header.svelte';
</script>

<Header></Header>
<main>
    <div class="container">
        <h1>Sobre nós</h1>
    
        <p>
            Estamos integrados no Grupo V Private e nascemos com o intuito de complementar as necessidades dos nossos Clientes no que diz respeito à intermediação de crédito e consultadoria, tanto de particulares como de empresas.
        </p>
    
        <p>
            Somos um intermediário de crédito vinculado autorizado e supervisionado pelo Banco de Portugal:
        </p>
    
        <ul>
            <li>Registo nº XXXX;</li>
            <li>Seguro de responsabilidade civil Intermediação de Crédito (exceto Imobiliário) da Seguradora XXXX - Apólice XXXX, válida de XXX a XXX;</li>
            <li>Seguro de responsabilidade civil de crédito para imóveis de habitação da seguradora XXXX Seguradora XXXX - Apólice XXXX, válida de XXX a XXX.</li>
        </ul>
    
        <p>
            Trabalhamos com um diversificado e reconhecido conjunto de Instituições Financeiras que nos permite apresentar sempre a solução ajustada a cada Cliente e nas melhores condições.
        </p>
    
        <p>
            O nosso foco são os Clientes. Ajudamos a poupar tempo e dinheiro. Não só nos preocupamos em apresentar as melhores soluções como também no cabal esclarecimento das condições contratuais. Queremos que os nossos Clientes realizem os seus sonhos de forma responsável, obtendo a solução ajustada a cada momento.
        </p>
    
        <p>
            Contamos com profissionais experientes e preocupados em servir o Cliente de forma responsável, rigorosa, transparente e com a privacidade que cada processo de crédito assim o exige.
        </p>
    
        <p>
            Estamos presentes nas lojas V Private em Gaia, Valongo e Porto.
        </p>
    
        <p>
            Ajudamos e simplificamos!
        </p>
    </div>
</main>

<style>
    main {
        max-width: 50%;
		margin: 0 auto;
        display: flex;
        flex-direction: column;
    }

    .container {
        margin: 8rem 0 4rem 0;
    }

    li {
        margin: 0.25rem 0;
    }

    h1 {
        font-size: 2.5rem;
        font-weight: bold;
        margin: 1rem 0;
    }

    p {
        margin: 0.5rem 0;
        text-align: justify;
    }
</style>