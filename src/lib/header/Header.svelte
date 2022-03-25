<script>
	import { page } from '$app/stores';
</script>

<header>
	<div class="bg-neutral-700 py-2 mt-2 mx-8">
		<ul class="flex flex-row justify-center gap-2 text-neutral-300">
			<li class:active={$page.url.pathname === '/'}>
				<a sveltekit:prefetch href="/">Home</a>
			</li>
			<li class:active={$page.url.pathname === '/about'}>
				<a sveltekit:prefetch href="/about">About</a>
			</li>
		</ul>
	</div>
</header>