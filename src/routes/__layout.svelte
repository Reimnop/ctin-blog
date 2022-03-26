<script>
	import Sidebar from '$lib/header/Sidebar.svelte';
	import '../app.css';
</script>

<div class="flex flex-col md:flex-row">
	<Sidebar />

	<main class="flex-1 p-4">
		<slot />
	</main>
</div>
