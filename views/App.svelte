<script lang="ts">
	import Footer from '../components/Footer.svelte';
	import Services from './Services.svelte';
</script>

<main>
	<div class="main-container">
		<img src="images/landing.jpg" alt="" />

		<div class="outer-overlay">
			<div class="inner-overlay">
				<div class="title-container">
					<h1>V PRIVATE</h1>
				</div>

				<div class="services-row">
					<div class="service-row-box">Crédito Habitação</div>
					<div class="service-row-box">Crédito Pessoal & Cartões Crédito</div>
					<div class="service-row-box">Crédito Automóvel</div>
					<div class="service-row-box">Empresas</div>
				</div>
			</div>
		</div>
	</div>

	<div class="about-container">
		<div class="about-overlay">
			<h2>Sobre nós</h2>
			<p>Somos uma empresa do Grupo V Private e temos como missão a definição, conjunta e totalmente gratuita para si, da melhor solução de crédito para a concretização do seu projeto.</p><br/>
			
			<p>Temos um leque variado e significativo de parceiros financeiros que nos permite ter acesso à solução adequada a cada necessidade e nas melhores condições financeiras.</p><br/>
	
			<p>Garantimos rigor, personalização e privacidade em cada processo de crédito. Somos uma empresa autorizada e supervisionada pelo Banco de Portugal.</p><br/>
	
			<p>Ajudamos e simplificamos!</p>
		</div>
	</div>

	<!-- <Services /> -->
	<Footer />
</main>

<style>
	.main-container {
		position: relative;
		overflow: hidden;
		height: 100vh;
	}

	.main-container img {
		width: 100%;
		height: 100%;
		object-fit: cover;
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

	.inner-overlay h2 {

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
		align-items: center;
		justify-content: center;
		text-align: center;
		width: 240px;
		height: 150px;
		font-size: 24px;
		padding: 0 1em;
		margin: 0.5em;
		border: 2px solid white;
		font-weight: 600;
		box-shadow: rgba(0, 0, 0, 0.56) 0px 22px 70px 4px;
	}

	.service-row-box:hover {
		background: white;
		color: black;
		transition: all 0.3s ease-in-out;
		cursor: pointer;
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