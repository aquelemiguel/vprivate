<script lang="ts">
    export let isOpen = false;

    const closeModal = () => {
        isOpen = false;
    }

    window.onclick = function(event) {
        if (event.target.className.includes('modal-container')) {
            closeModal();
        }
    }
</script>

<div class="modal-container"
    style={`display: ${isOpen ? 'block' : 'none'}`}>
    <div class="modal-content">
        <div class="modal-relative-content">
            <h1>Vamos conversar?</h1>
    
            <p>manuel.leal@vprivate.pt</p>
            <p>+351 938 885 971 // +351 220 044 700</p>
            <p>Dias úteis das 9h00 às 18h00</p>
    
            <button
                class="modal-close-btn"
                on:click={closeModal}>
                Fechar
            </button>
        </div>
    </div>
</div>

<style>
    .modal-container {
        display: none;
        position: fixed;
        z-index: 1000;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        background-color: rgba(0, 0, 0, 0.4);
    }

    .modal-content {
        background-color: white;
        border-radius: 0.5rem;
        box-shadow: 0 10px 10px rgba(0, 0, 0, 0.2);
        margin: 15% auto;
        padding: 2rem;
        width: 40%;
        height: 25%;
        font-size: 18px;
    }

    .modal-relative-content {
        position: relative;
    }

    .modal-relative-content > h1 {
        margin-bottom: 1rem;
    }

    .modal-relative-content > p {
        margin: 0.5rem 0;
    }

    .modal-close-btn {
        position: absolute;
        top: 0;
        right: 0;
    }
</style>