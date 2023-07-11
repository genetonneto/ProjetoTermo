<script>
    import { trocarEstadoDoJogo } from "./Estado.js";
    import { board } from "./Estado.js"
    import Cell from './Cell.svelte';

</script>
<button class="menu" on:click={() => trocarEstadoDoJogo('menu')} on:keydown={() => {}}>
    Menu
</button>
<style>
     @import url('https://fonts.cdnfonts.com/css/angel-club');
.game-board {
margin: 50px auto;
width: fit-content;
font-family: 'Angel Club', sans-serif;
}

.row {
display: flex;
}

* {
	margin: 0;
	padding: 0;
    font-family: 'Angel Club', sans-serif;
}


body {
	font-family: 'Angel Club', sans-serif;
	background-color: #0F1A1D;

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
.menu:hover {
		background-color: #FFF6F6;
		color: #173B47;
        box-shadow : inset 0 0 0 3px #FFF6F6;
}

</style>
<body>
    


<div class="game-board">
    {#each $board as column, y}
         <div class="row" >
            {#each column as row, x}
                 <Cell {y} {x} />
            {/each}

         </div>
    {/each}

</div>

</body>
