<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
</script>

<header>
	<nav>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname === '/cv' ? 'page' : undefined}>
				<a href="/cv">cv</a>
			</li>
			<li>
				<a href="https://github.com/Life-of-Felix?tab=repositories">Github</a>
			</li>
			
		</ul>
	</nav>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		background-image: url("images/background2.png");
		background-size: 10rem;
		background-position: center;
		background-blend-mode: hard-light;
		background-color: var(--felixPurple);
		height: 100%;
	}
	ul{
		list-style: none;
		padding: 0%;
	}
	nav{
		width: 100%;
	}
	ul li{
		margin: 5% 0%;
	}
	a{
		color: var(--felixWhite);
		font-size: 1.5rem;
		box-shadow: var(--felixWhite) 0rem 0rem inset;
		display: inline-block;    
		padding: 5% 0%;
		width: 100%;
		background: rgba(255, 255, 255, 0.2);  
		backdrop-filter: blur(.15rem); 
		box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
		border-top: .1rem rgba(255, 255, 255, 0.2) solid;
		text-align: center;
		text-decoration: none;
		letter-spacing: .2rem;
	}
	a:hover{
		background: rgba(0, 0, 0, 0.1);  
		transition: .2s ease-in-out;
	}
</style>
