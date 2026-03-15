<script>
	import '../app.css';
	
	let { children } = $props();
</script>

<div class="min-h-screen flex flex-col">
	<nav class="flex justify-between items-center px-8 py-6 max-w-6xl mx-auto w-full">
		<a href="/" class="flex items-center gap-2 no-underline text-text font-semibold text-xl">
			<span class="text-2xl">🏔️</span>
			<span>Headcrest</span>
		</a>
		<div class="flex gap-8">
			<a href="/about" class="text-text-muted no-underline font-medium transition-colors hover:text-primary">About</a>
			<a href="https://github.com/headcrest" target="_blank" rel="noopener" class="text-text-muted no-underline font-medium transition-colors hover:text-primary">GitHub</a>
		</div>
	</nav>
	
	<main class="flex-1">
		{@render children()}
	</main>
	
	<footer class="text-center py-8 text-text-muted text-sm">
		<p>Built with ❤️ by Headcrest • Powered by SvelteKit</p>
	</footer>
</div>
