<script>
    import { trocarEstadoDoJogo } from "./Estado.js";
</script>

<body>
    <header>
       
    </header>
<main class= "conteudo">
    <h1>Termo</h1>
        <button class="menu" on:click={() => trocarEstadoDoJogo('jogar')} on:keydown={() => {}}>
            Jogar
        </button>
        <button class="menu" on:click={() => trocarEstadoDoJogo('Comojogar')} on:keydown={() => {}}>
            Como Jogar
        </button>  
        <button class="menu" on:click={() => trocarEstadoDoJogo('sobre')} on:keydown={() => {}}>
            sobre
        </button>  
</main>
</body>

<style>
 @import url('https://fonts.cdnfonts.com/css/angel-club');
	
	body {
		margin: 0;
		padding: 0;
        background-color: #0F1A1D;
    }
    .conteudo{
		font-family: 'Angel Club', sans-serif;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 80vh;
		color : #E4FAF8;
		font-size: 50px;
	}
    button {
		font-family: 'Angel Club', sans-serif;
		justify-content: center;
		align-items: center;
		cursor: pointer;
		margin-top: 10px;
		margin-bottom: 10px;
		display: flex;
		font-size: 30px;
		color : #FFF6F6;
		background-color: #173B47;
		border-color: #173B47;
		border-radius: 15px;
	}
    .menu:hover{
		background-color: #FFF6F6;
		color: #173B47;
        box-shadow : inset 0 0 0 3px #FFF6F6;
	}
</style>