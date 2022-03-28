<script>
	import NavLink from "./NavLink.svelte";

	$: outerWidth = 0
	$: innerWidth = 0
	$: outerHeight = 0
	$: innerHeight = 0

	let open = false;
</script>

<svelte:window bind:innerWidth bind:outerWidth bind:innerHeight bind:outerHeight />

<div class="sticky w-full md:w-96 md:h-[100vh] bg-slate-800 flex flex-col gap-4 shadow-colored">
	<div class="flex flex-row p-4 items-center w-full duration-200 hover:scale-105">
		<img src="logo_gd.png" alt="GiaDinh" width="110" height="110"/>
		<div class="title relative text-center text-6xl w-full">
			<b>GDI WIKI</b>
		</div>
	</div>
	<div class="flex items-center justify-center self-end bg-slate-300 text-slate-700 w-8 h-8 rounded m-2 duration-200 hover:scale-105 md:hidden" class:button-rotated={!open}>
		<button class="text-2xl rounded duration-200" on:click={() => open = !open}>
			˅
		</button>
	</div>
	{#if open || innerWidth > 768} <!-- md = 768px -->
		<div class="flex flex-col gap-4">
			<NavLink href="/">🏠 HOMEPAGE</NavLink>
			<NavLink href="/problems">📜 PROBLEMS</NavLink>
			<NavLink href="/about">🎤 GIỚI THIỆU</NavLink>
			<NavLink href="/contact">📞 LIÊN HỆ</NavLink>
		</div>
	{/if}
</div>