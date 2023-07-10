<script>
    import { trocarEstadoDoJogo } from "./Estado.js";
</script>

    <button class="menu" on:click={() => trocarEstadoDoJogo('menu')} on:keydown={() => {}}>
    Menu
    </button>

    <body class = "conteudo">
 <header>
    <h1>Sobre</h1>
 </header>
<main>
    <p>
      Esse projeto foi desenvolvido pelo os alunos do 1º Período do Curso de TSI <br>
	Na disciplina de Programação Imperativa do Professor Allan Diego Silva Lima, onde desenvolvemos o Jogo Termo<br> 
	</p>
	    <h2>Alunos</h2>

    <ul>
        <li><p>Jadson andrewns</p><a href="https://github.com/jadsonfe" target="_blank">Github</a></li>
        <li><p>Paulo Cabral</p><a href="https://github.com/pauloJ-r" target="_blank">Github</a></li>
        <li><p>Matheus de Oliveira</p><a href="https://github.com" target="_blank">Github</a></li>
        <li><p>Matheus Wenceslau</p><a href="https://github.com/WENCESLAUN" target="_blank">Github</a></li>
        <li></li>
    </ul>

    <h2>Monitores</h2>

    <li><p>Geneteton Neto</p><a href="https://github.com/genetonneto" target="_blank">Github</a></li>
    <li><p>Luiz</p><a href="https://github.com" target="_blank">Github</a></li>

</main>
    </body>

<footer>
    <p>&copy; 2023 Jogo Termo. Todos os Direito Reservados</p>
</footer>
<style>
     @import url('https://fonts.cdnfonts.com/css/angel-club');
	
body {
	margin: 0;
	padding: 0;
    background-color: #0F1A1D;
}

.conteudo {
	font-family: 'Angel Club', sans-serif;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
    text-align: center;
	height: 80vh;
	color : #E4FAF8;
	font-size: 25px;
}
    

a {
    font-family: 'Angel Club', sans-serif;
	justify-content: center ;
	align-items: center;
    font-size: 25px;
    cursor: pointer;
	background-color: #173B47;
	border-color: #173B47;
	border-radius: 15px;
    margin-left: 15px;
    text-decoration: none;
    color: white; 
}


.menu {
	font-family: 'Angel Club', sans-serif;
	justify-content: center;
	align-items: center;
	cursor: pointer;
	margin-top: 10px;
	margin-bottom: 10px;
	display: flex;
	font-size: 25px;
	color : #ffffff;
	background-color: #173B47;
	border-color: #173B47;
    margin-left: 15px;
	border-radius: 15px;
}
 
.menu:hover {
    color: #173B47;
    background-color: #FFF6F6;
    box-shadow : inset 0 0 0 3px #FFF6F6;
}

a:hover{
    background-color: #FFF6F6;
    color: #173B47;
}

footer {
    font-family: 'Angel Club', sans-serif;
    text-align: center;
    color: white;  
        
}

li {
    list-style-type: none;
    display: inline-block;
    margin-right: 10px;
}

li a {
    text-decoration: none;
    color: #E4FAF8;
    padding: 5px;
    

}
</style>