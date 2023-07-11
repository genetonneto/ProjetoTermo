<script>
    import { trocarEstadoDoJogo } from "./Estado.js";
</script>

<body class = "conteudo">
    <button class="menu" on:click={() => trocarEstadoDoJogo('menu')} on:keydown={() => {}}>
        Menu
    </button>
<header>
    <div class="div-header">
        <h1>Sobre</h1>
        
    </div>
</header>

<main>
    <p>
        Esse projeto foi desenvolvido pelo os alunos do 1º Período do Curso de TSI - IFPE Campus Igarassu<br>
	    Na disciplina de Programação Imperativa do Professor Allan Diego Silva Lima, onde desenvolvemos o Jogo Termo<br> 
	</p>
	
    <h2>Alunos</h2>

    <ul>
        <li><p>Jadson Andreys</p><a href="https://github.com/jadsonfe" target="_blank">Github</a></li>  <!-- Editar sobrenome de Jadson -->
        <li><p>Paulo Cabral</p><a href="https://github.com/pauloJ-r" target="_blank">Github</a></li>
        <li><p>Matheus de Oliveira</p><a href="https://github.com" target="_blank">Github</a></li>
        <li><p>Matheus Wenceslau</p><a href="https://github.com/WENCESLAUN" target="_blank">Github</a></li>
    </ul>

    <h2>Monitores</h2>
        <li><p>Geneteton Neto</p><a href="https://github.com/genetonneto" target="_blank">Github</a></li>
        <li><p>Luiz Carlos</p><a href="https://github.com/Luizcsrj" target="_blank">Github</a></li>
</main>
</body>

<footer class="footer">
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
    text-align: center;
    display: block;
    font-size: 25px;
    color: white;
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

.footer {
    font-size: 15px;
    font-family: 'Angel Club', sans-serif;
    display: flex;
    flex-direction: column;
    text-align: center;
    color: white;  
    margin-top: 30px;
        
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