<script>
    // @ts-nocheck

    export let char;
    export let KeyPress;
</script>

<div class="Key" on:click={()=> KeyPress(char.toUpperCase())}>
    {char.toUpperCase()}
</div>

<style>
    .Key {
        background-color: var(--bg);
        color: white;
        padding: 20px 18px;
        margin: 4px 3px;
        cursor: pointer;
        border-radius: 10px;
        transition: background-color .3s;
    }

    .Key:hover {
        background-color: rgb(7, 231, 183);
    }

    @media screen and (max-width: 600px) {
        .Key {
            padding: 15px 12px; 
            margin: 2px 1px; 
            border-radius: 8px; 
        }
    }
</style>
