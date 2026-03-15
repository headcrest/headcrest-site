<script>
	import '../app.css';
</script>

<div class="site-wrapper">
	<nav class="nav">
		<a href="/" class="logo">
			<span class="logo-icon">🏔️</span>
			<span class="logo-text">Headcrest</span>
		</a>
		<div class="nav-links">
			<a href="/about">About</a>
			<a href="https://github.com/headcrest" target="_blank" rel="noopener">GitHub</a>
		</div>
	</nav>
	
	<main>
		<slot />
	</main>
	
	<footer class="footer">
		<p>Built with ❤️ by Headcrest • Powered by SvelteKit</p>
	</footer>
</div>

<style>
	.site-wrapper {
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}
	
	.nav {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1.5rem 2rem;
		max-width: 1200px;
		margin: 0 auto;
		width: 100%;
		box-sizing: border-box;
	}
	
	.logo {
		display: flex;
		align-items: center;
		gap: 0.5rem;
		text-decoration: none;
		color: var(--text);
		font-weight: 600;
		font-size: 1.25rem;
	}
	
	.logo-icon {
		font-size: 1.5rem;
	}
	
	.nav-links {
		display: flex;
		gap: 2rem;
	}
	
	.nav-links a {
		color: var(--text-muted);
		text-decoration: none;
		font-weight: 500;
		transition: color 0.2s;
	}
	
	.nav-links a:hover {
		color: var(--primary);
	}
	
	main {
		flex: 1;
	}
	
	.footer {
		text-align: center;
		padding: 2rem;
		color: var(--text-muted);
		font-size: 0.875rem;
	}
</style>
