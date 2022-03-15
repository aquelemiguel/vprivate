<script lang="ts">
    import * as json from '../public/db.json';
	const data = json['default'];

	import Footer from '../components/Footer.svelte';
    
    const navigateTo = (url: string) => {
        window.location.href = url;
    }
</script>

<main>
    <div class="main-container">
		<div class="background-image"></div>

        <div class="outer-overlay">
            <div class="inner-overlay">
                <div class="title-container">
                    <h1>V PRIVATE</h1>
                    <h3>Intermediário Crédito</h3>
                </div>

                <div class="services-row">
                    {#each data as service}
						<div class="service-row-box" on:click={() => navigateTo(`/servicos#${service.id}`)}>
							<span class="service-title">{service.title}</span>
							<span class="learn-more">Saiba mais...</span>
						</div>
                    {/each}
                </div>
            </div>
        </div>
    </div>

    <div class="about-container">
        <div class="about-overlay">
            <h2>Bem-vindo</h2>
            <p>Somos uma empresa do Grupo V Private e temos como missão a definição, conjunta e totalmente gratuita para si, da melhor solução de crédito para a concretização do seu projeto.</p><br/>
            
            <p>Temos um leque variado e significativo de parceiros financeiros que nos permite ter acesso à solução adequada a cada necessidade e nas melhores condições financeiras.</p><br/>
    
            <p>Garantimos rigor, personalização e privacidade em cada processo de crédito. Somos um intermediário de crédito vinculado, autorizado pelo Banco de Portugal, com o registo nº XXXX.</p><br/>
    
            <p>Ajudamos e simplificamos!</p>
        </div>
    </div>

    <Footer />
</main>

<style>
	.main-container {
		position: relative;
		overflow: hidden;
		height: 100vh;
	}

	.background-image {
		width: 100%;
		height: 100%;
		background-image: linear-gradient(rgba(200, 157, 40, 0.6), rgba(200, 157, 40, 0.6)), url(../../images/landing2.jpg);
		background-size: cover;
		background-position: center;
	}

	.outer-overlay {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: rgba(0, 0, 0, 0.5);
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.inner-overlay {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		color: white;
	}

	.inner-overlay h1 {
		font-size: 128px;
		color: white;
		text-shadow: 0px 4px 3px rgba(0, 0, 0, 0.212),
            		 0px 8px 13px rgba(0,0,0,0.1),
             		 0px 18px 23px rgba(0,0,0,0.1);
	}

	.inner-overlay h3 {
        font-weight: 300;
        font-size: 20px;
        text-shadow: 0px 4px 3px rgba(0, 0, 0, 0.212),
            		 0px 8px 13px rgba(0,0,0,0.1),
             		 0px 18px 23px rgba(0,0,0,0.1);
        margin: unset;
	}

	.title-container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin-bottom: 4rem;
	}

	.services-row {
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.service-row-box {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		width: 240px;
		height: 150px;
		padding: 0 2rem;
		margin: 0.5em 0.5em 0 0.5em;
		border: 2px solid white;
		box-shadow: rgba(0, 0, 0, 0.56) 0px 22px 70px 4px;
	}

	.service-row-box:hover {
		background: white;
		color: black;
		transition: all 0.3s ease-in-out;
		cursor: pointer;
	}

	.service-title {
		font-size: 1.5rem;
		font-weight: 600;
		margin: auto 0;
	}

	.learn-more {
		font-size: 0.75rem;
		margin-bottom: 1rem;
	}

	.about-container {
		max-width: 60%;
		margin: 0 auto;
		display: flex;
	}

	.about-overlay {
		margin: 5rem 0rem;
	}

	.about-overlay > h2 {
		font-size: 64px;
		margin: 0 0 2rem 0;
	}

	.about-overlay > p {
		font-size: 1.2rem;
		line-height: 1.5;
		text-align: justify;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>