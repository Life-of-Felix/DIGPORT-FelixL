<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Felix Lindblom webpage" />
</svelte:head>
<!-- The job in mind -->
<!-- https://jobs.opera.com/p/6c09a732ee97-product-designer  -->
 <div class="wrap">
	<section id="landImage">
		<img src="images/placeholderFelix.png" alt="portrait">	
	</section>
	<h1 id="hej">Hej Experis</h1>
	<section id="shortDec">
		<p>I'm a front end devloper and educated myself at Jönköping Univirsty and FHNW in Swisserland. Technical, creactive and team motivted. I'm looking for your postion of Ux designer</p>
	</section>
 </div>


<style>
	img{
		width: 20rem;
		transition: transform 0.1s ease-out;
	}
	.wrap{
		display: grid; 
		grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr; 
		grid-template-rows: 1fr 1fr 1fr 1fr 1fr; 
		gap: 1rem 1rem; 
	}
	#landImage{
		grid-area: 2 / 2 / 5 / 6; 
		overflow: hidden;
	}
	#landImage img{
		height: 100%;
		min-width: 100%;
		object-fit: cover;
	}
	#hej{
		grid-area: 2 / 1 / 3 / 4;
		background: rgba(255, 255, 255, 0.2);  
		backdrop-filter: blur(.15rem); 
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		border-top: .1rem rgba(255, 255, 255, 0.2) solid;
		text-align: left;
		padding: 0% 5%;
		text-decoration: none;
		letter-spacing: .5rem;
		width: fit-content;
	}
	#shortDec{
		grid-area: 4 / 3 / 6 / 7; 
		z-index: 2;
		display: flex;
		flex-direction: column;
		align-items: start;
		margin: 0%;
		background: rgba(255, 255, 255, 0.2);  
		backdrop-filter: blur(.15rem); 
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		border-top: .1rem rgba(255, 255, 255, 0.2) solid;
		text-align: left;
		padding: 0% 5%;
		text-decoration: none;
		letter-spacing: .1rem;
		width: fit-content;
		height: fit-content;
	}
	
</style>
