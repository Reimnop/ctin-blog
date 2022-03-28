<script>
	import Sidebar from '$lib/header/Sidebar.svelte';
	import '../app.css';
</script>

<Sidebar />

<main class="flex-1 p-4 md:ml-96">
	<slot />
</main>
