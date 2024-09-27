<script>
	import Header from './Header.svelte';
	import '../app.css';
</script>

<div class="app">
	<header>
		<Header />
	</header>
	

	<main>
		<slot />
	</main>

	<footer>
		<p>Work in pogress</p>
	</footer>
</div>

<style>
	.app {
		
		display: grid;
		grid-template-columns: 1fr 6fr;
		grid-template-areas: 
		"na ma"
		"na fo"
		;
		min-height: 100vh;
	}
	header{
		grid-area: na;
	}
	main {
		grid-area: ma;
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		grid-area: fo;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
		background-color: blueviolet;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
