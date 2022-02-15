<script>
    let services = [
        { id: 1, text: 'Crédito Habitação' },
        { id: 2, text: 'Crédito Pessoal & Cartão Crédito' },
        { id: 3, text: 'Crédito Automóvel' },
        { id: 4, text: 'Empresas' }
    ];

    let form = {
        name: '',
        email: '',
        phone: '',
        service: '',
        message: ''
    };

    let submitted = false;

    function onSend() {
        submitted = true;
        console.log(form);
    };
</script>

<div class="outer-container">
    <div class="inner-container">
        <!-- <div class="banner">
            <h1>Contactos</h1>
        </div> -->

        <div class="form-container">
            <div class="form-left-side">
                <form class:submitted>
                    <div class="form-group">
                        <input bind:value={form.name} placeholder="Nome*" required />
                    </div>
    
                    <div class="form-group">
                        <input bind:value={form.email} placeholder="Email*" required />
                    </div>
    
                    <div class="form-group">
                        <input bind:value={form.phone} placeholder="Telefone" />
                    </div>
    
                    <div class="form-group">
                        <select bind:value={form.service} required>
                            <option hidden selected value>Serviço*</option>
                            {#each services as service}
                                <option value={service.text}>{service.text}</option>
                            {/each}
                        </select>
                    </div>
    
                    <div class="form-group">
                        <textarea bind:value={form.message} placeholder="Mensagem*" required></textarea>
                    </div>
    
                    <button disabled={false} on:click={onSend}>Enviar</button>
                </form>
            </div>

            <div class="form-right-side">
                <div class="form-image">
                    <img src="images/example.jpg" />
                </div>
    
                <div class="company-info">
                    <h3>Email</h3>
                    <p>vprivate@email.com</p>
    
                    <h3>Contacto telefónico</h3>
                    <p>+351 912 345 678</p>
                    <p>+351 912 345 678</p>
                </div>
            </div>
    
        </div>

    </div>
</div>

<style>
    .outer-container {
        background-color: #F7F7F7;
    }

    h1 {
        font-size: 3.5rem;
    }

    .inner-container {
        min-height: 100vh;
        max-width: 75%;
		margin: 0 auto;
        display: flex;
        justify-content: center;
        flex-direction: column;
    }

    .banner {
        width: 100%;
        min-height: 8rem;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    input, select {
        height: 4rem;
    }

    textarea {
        height: 15rem;
    }

    form {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .form-group {
        width: 100%;
        margin: 0.5rem 0;
    }

    .form-group > * {
        width: 100%;
        border: 0;
        border-bottom: 2px solid white;
        padding: 1rem;
        background-color: #001f53;
        color: white;
    }

    .form-group *::placeholder {
        color: white;
    }

    .submitted input:invalid {
        border-bottom: 2px solid red;
    }

    .submitted textarea:invalid {
        border-bottom: 2px solid red;
    }

    .submitted select:invalid {
        border-bottom: 2px solid red;
    }

    select:invalid option {
        color: white;
    }

    button {
        background-color: #001f53;
        color: var(--main-bg-color);
        border: none;
        min-width: 30%;
        font-size: 1.2em;
        font-weight: bold;
        cursor: pointer;
        transition: all 0.2s ease-in-out;
        margin: 1rem 0;
        height: 4rem;
    }

    button:hover {
        background-color: var(--main-bg-color);
        color: var(--alt-bg-color);
    }

    .form-container {
        display: flex;
    }

    .form-left-side {
        width: 50%;
        background-color: #003690;
        padding: 3rem 3rem 1rem 3rem;
        box-shadow: rgba(0, 0, 0, 0.6) 0px 40px 40px -15px;
        border-radius: 0.25rem;
    }

    .form-right-side {
        display: flex;
        margin-left: 1rem;
        flex-direction: column;
        justify-content: center;
        box-shadow: rgba(0, 0, 0, 0.6) 0px 40px 40px -15px;
        border-radius: 0.25rem;
        overflow: hidden;
    }

    .form-image {
        object-fit: cover;
    }

    .form-image > img {
        width: 100%;
        height: 100%;
    }

    .company-info {
        flex-grow: 1;
        background-color: #003690;
        padding: 2rem 3rem;
        color: white;
    }

    .company-info > h3 {
        font-size: 1.4rem;
        margin: 0.5rem 0;
    }

    .company-info > p {
        margin: 0.5rem 0;
    }

    .company-info > h3:last-of-type {
        margin-top: 2rem;
    }
</style>