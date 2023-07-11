<script>
    import { trocarEstadoDoJogo } from "./Estado.js";
</script>

<button class="menu" on:click={() => trocarEstadoDoJogo('menu')} on:keydown={() => {}}>
    Menu
</button>

<body class = "conteudo">
    <header>
       <h1>Como Jogar</h1>
    </header>
<main>
    <p>
       O Termo é um jogo de palavras divertido e desafiador que envolve adivinhar uma palavra oculta de 5 letras em 6 tentativas. <br>
	   O objetivo é descobrir a palavra correta usando dicas fornecidas pelos resultados de suas tentativas anteriores. <br> 
	</p>
	   <p>
		Descubra a palavra certa em 6 tentativas.
 Depois de cada tentativa, as peças mostram o quão perto você está da solução.
 <br> 
     <div class = "exemplo">
        <span tabindex="0" role="text" aria-label="letra T correta" class="letter right">T</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra E" class="letter">E</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra R" class="letter">R</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra M" class="letter">M</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra O" class="letter">O</span> 
    </div>

    <p tabindex="0">
        A letra <span class="exemplo">T</span>  faz parte da palavra e está na
        posição correta.
	    </p>

    <div class= "exemplo1">
        <span tabindex="0" role="text" aria-label="letra V" class="letter right">V</span>
    </div>

    <div class="exemplo2">
        <span tabindex="0" role="text" aria-label="letra I está na posição errada mais faz parte" class="letter">I</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra O" class="letter">O</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra L" class="letter">L</span>
    </div>

    <div class="exemplo1">
        <span tabindex="0" role="text" aria-label="letra A" class="letter">A</span>
    </div>

    <p tabindex="0">
     A letra <span class="exemplo2">I</span>  faz parte da palavra mas em outra posição.
    </p>
    
    </main>

    <footer class= "footer">
        <p>&copy; 2023 Jogo Termo. Todos os Direito Reservados</p>
    </footer>
</body>
<style>
 @import url('https://fonts.cdnfonts.com/css/angel-club');

body {
	margin: 0;
	padding: 0;
    background-color: #0F1A1D;
}
.conteudo {
    font-family: 'Angel Club', sans-serif;
    text-align: center;
    display: block;
    font-size: 25px;
    color: white;

}
button {
	font-family: 'Angel Club', sans-serif;
	justify-content: center;
	align-items: center;
	cursor: pointer;
	margin-top: 10px;
	margin-bottom: 10px;
	display: flex;
	font-size: 25px;
	color : #FFF6F6;
	background-color: #173B47;
	border-color: #173B47;
	border-radius: 15px;
    margin-left: 15px;
}
.menu:hover{
	background-color: #FFF6F6;
	color: #173B47;
    box-shadow : inset 0 0 0 3px #FFF6F6;
}
p{
    font-family: 'Angel Club', sans-serif;
    text-align: center;
    color: #E4FAF8;  
}
.footer {
    font-size: 15px;
    font-family: 'Angel Club', sans-serif;
    display: flex;
    flex-direction: column;
    text-align: center;
    color: white;  
    margin-top: 30px;
        
}
.exemplo {
	background-color: var(--green);
    border: none;
    align-items: center;
    border: 0.125em solid  #E4FAF8;  
    border-radius: 10%;
    box-sizing: border-box;
    color:  #E4FAF8;  
    display: inline-flex;
    font-weight: 500;
    height: 2em;
    justify-content: center;
    margin: 0 0.05em;
    width: 2em;
	}
.exemplo1 {
    border: none;
    align-items: center;
    border: 0.125em solid  #E4FAF8;  
    border-radius: 10%;
    box-sizing: border-box;
    color:  #E4FAF8;  
    display: inline-flex;
    font-weight: 500;
    height: 2em;
    justify-content: center;
    margin: 0 0.05em;
    width: 2em;
	}
.exemplo2 {
	background-color: var(--orange);
    border: none;
    align-items: center;
    border: 0.125em solid  #E4FAF8;  
    border-radius: 10%;
    box-sizing: border-box;
    color:  #E4FAF8;  
    display: inline-flex;
    font-weight: 500;
    height: 2em;
    justify-content: center;
    margin: 0 0.05em;
    width: 2em;
	}
</style>