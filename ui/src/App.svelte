<script>
	import Table from "./Table.svelte";
	 let firstName='test';
	 let lastName='p';
	 let person = prompt("Please enter your name", "Harry Potter");
	 $: name = person
</script>

<main>
	<h1>Hello {name}</h1>

	<Table/>
	
	
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>