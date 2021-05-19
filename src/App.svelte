<script>
	export let name;
	export let headText = 'This is a div';
	let age = 40;
	function incrementAge() {
		age += 1;
	}
</script>

<main>
    <div class="test">{headText}</div>
	<h1>Hello {name}!, my age is {age}</h1>
	<button on:click="{incrementAge}">Click Me!</button>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
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

	.test {
	    width: 500px;
	    height: 500px;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

</style>
