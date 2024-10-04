<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
<!-- The job in mind -->
<!-- https://jobs.opera.com/p/6c09a732ee97-product-designer  -->
 <div class="wrap">
	<section id="landImage">
		<img src="/src/lib/images/pH.png" alt="portret">
	</section>
	<section id="operaText">
		<h1>Hej Opera</h1>
		<p> My name is Felix Lindblom and here is my portfolio</p>
	</section>
 </div>


<style>
	img{
		width: 20rem;
	}
	.wrap{
		display: grid;
		grid-template-columns: repeat(6, 1fr);
		grid-template-rows: repeat(4, 1fr); 
		grid-template-areas: 
		"te te te  .  .  . "
		".  .  .  im im im "
		".  .  .  im im im "
		".  .  .  .  .  . "
		;
	}
	#landImage{
		grid-area: im;
	}
	#landImage img{
		
		width: 100%;
		min-height: 100%;
		overflow: hidden;
	}
	#operaText{
		grid-area: te;
		display: flex;
		flex-direction: column;
		align-items: start;
		margin: 0%;
	}
	
</style>
