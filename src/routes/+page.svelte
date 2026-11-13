<script>
	let numero = $state(0);
	
	function obtenerResultado() {
		if (numero === 0) return "neutro";
		if (numero % 2 === 0) return "par";
		return "impar";
	}
</script>

<div class="caja">
	<p>El número {numero} es {obtenerResultado()}</p>
	<input type="number" bind:value={numero}>
</div>

<style>
	.caja {
		border: 2px solid #4b0082;
		border-radius: 6px;
		padding: 20px;
		text-align: center;
		max-width: 300px;
		margin: 30px auto;
		background: white;
	}
	
	p {
		font-size: 22px;
		font-family: 'Segoe UI', sans-serif;
		color: rgb(34, 5, 112);
		margin: 0 0 15px 0;
	}
	
	input {
		font-size: 18px;
		width: 80px;
		text-align: center;
		border: 1px solid #999;
		padding: 5px;
	}
</style>
