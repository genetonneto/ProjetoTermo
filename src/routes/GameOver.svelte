
<script>
    
import {GAME_WORD, board, colors, creatGrid, gameInfo, gameOver, guess} from "./Estado"
  
    const playAgain = () => {

            const wordsList = ['PRAIA','AMIGO','FALAR','CANTO',
            'MUITO','FELIZ','CHUVA','BANDA','ROSTO','COISA','OLHAR','PULAR',
        'AFETO']

        const word = wordsList[Math.floor(Math.random() * wordsList.length)];
        GAME_WORD.set(word);

        gameInfo.set({
            attempt: 0, char: 0
        });
        guess.set("");
        colors.set(creatGrid());
        board.set(creatGrid());
        gameOver.set(false)
    }
</script>

 

<div class="center">
    <h3>A Palavra Correta era: <strong>{$GAME_WORD}</strong></h3>
    <h3>Você Disse: <strong>{$guess}</strong></h3>
</div>

<div class="center">
    <button on:click={playAgain}>Jogar novamente</button>
</div>

<style>
strong {
    font-weight: 900;
    color:white;
}
h3 {
    font-size: 2em;
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
		background-color: var(--orange);
		border-radius: 10px;
}

.center {
    margin: 20px auto;
    width: fit-content;
    text-align: center;
}
</style>