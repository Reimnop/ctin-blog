<script context="module">
	import Card from "./Card.svelte"

	export const prerender = true;
</script>

<svelte:head>
	<title>Homepage</title>
	<link rel="icon" type="image/png" href="logo_gd.png" />
</svelte:head>

<div class="flex flex-row flex-wrap gap-4">
	{#each Array(20) as _}
		<div class="w-96">
			<Card>
				<b slot="header">Hello world!</b>
				<span slot="body">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer ac nisl ut quam tincidunt lobortis a sit amet lectus. Nunc vel libero pretium erat auctor condimentum quis pellentesque lectus. Vestibulum sem nisl, tempor non sapien sit amet, ultricies maximus quam. Maecenas mollis auctor libero a dictum. Morbi tempor velit quis leo consectetur, et mollis purus fringilla. Pellentesque rhoncus odio a dui ultricies laoreet. Nam convallis porta consectetur. Nulla at risus viverra ligula bibendum dapibus. Nam finibus a nisl quis feugiat. Praesent eleifend quam eu congue dignissim. Etiam consequat quis magna sit amet dignissim. Nam non rutrum est. Sed tempus erat commodo diam porta, ut eleifend urna mollis. Quisque elit eros, tincidunt id tellus vitae, ultrices fermentum tellus. Sed porta consectetur turpis, vel efficitur augue semper non. Aliquam elit est, porttitor sed velit sit amet, tempus rutrum leo.</span>
			</Card>
		</div>
	{/each}
</div>