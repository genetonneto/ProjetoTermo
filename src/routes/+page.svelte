<script>
    import Menu from './Menu.svelte'
    import Sobre from './Sobre.svelte'
    import Jogar from './Jogar.svelte'
    import Comojogar from './Comojogar.svelte'
    import { estado } from './Estado.js'
     

    import { gameOver } from './Estado.js'
    import Keyboard from './Keyboard.svelte';
    import GameOver from './GameOver.svelte';

</script>
    {#if $estado === 'menu'}
    <Menu/>
    {:else if $estado === 'jogar'}
    <Jogar/>
    <Keyboard/>
    {#if $gameOver}
    <GameOver />
    {/if}
    {:else if $estado === 'Comojogar'}
    <Comojogar/>
    {:else if $estado === 'sobre'}
    <Sobre/>

{/if}




    

  