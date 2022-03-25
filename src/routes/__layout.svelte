<script>
	import Sidebar from '$lib/header/Sidebar.svelte';
	import '../app.css';
</script>

<div class="flex flex-col md:flex-row">
	<Sidebar />

	<main class="m-4 flex-1">
		<slot />
	</main>
</div>
