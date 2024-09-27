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
		background-color: blue;
		height: 100%;
	}
</style>
