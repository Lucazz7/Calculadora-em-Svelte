<script lang="ts">
import Calculadora from "./components/Calculadora.svelte";


</script>

<div class="container">
	<h1>Svelte Calculado Teste Zeus</h1>
</div>


<main>

	<Calculadora />

</main>

<style>
	:global(body)
		 {
		background-color: rgb(183, 120, 3);
	}
	
	.container{
		display: flex;
        flex: 1px;
        justify-content: center;
        background-color: black;
		color: rgb(148, 98, 5); 
        align-items: center;
        padding: 0px 5px;
        overflow: hidden;
        font-size: 1.7rem;
        margin: 2px 1px;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
	}
	
	:root {
		--cor-fundo: #555;
	}

	main {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 100vh;
	}

</style>