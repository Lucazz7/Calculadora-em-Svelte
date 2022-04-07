<script lang="ts">
    export let valor: string;
    
    $: tamanhoFonte = valor.length > 20 ? 'pequena' : `s-${valor.length}`;
</script>

<div class={`tela ${tamanhoFonte}`}>
    <span>{valor}</span>
</div>

<style>
    .tela {
        display: flex;
        height: 20%;
        /* flex: 1px; */
        justify-content: flex-end;
        background-color: aliceblue;
        align-items: center;
        padding: 0px 5px;
        overflow: hidden;
        font-size: 1.7rem;
        margin: 2px 1px;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
    }

    .s-12 { font-size: 1.7rem; }
    .s-13 { font-size: 1.6em;}
    .s-14 { font-size: 1.5rem;}
    .s-15 { font-size: 1.4rem;}
    .s-16 { font-size: 1.3rem;}
    .s-17 { font-size: 1.2rem;}
    .s-18 { font-size: 1.1rem;}
    .s-19 { font-size: 1rem;}
    .s-20 { font-size: 0.9rem;}
        
    .pequena{
        font-size: 0.6rem;
    }
</style>