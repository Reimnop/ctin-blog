<script>
	import { page } from '$app/stores';
</script>

<header>
	<div class="flex flex-row m-4 items-center">
		<img src="https://upload.wikimedia.org/wikipedia/vi/c/c9/Logo_Thpt_Gia_Dinh.gif" alt="GiaDinh" width="110" height="110"/>
		<div class="title relative text-center text-6xl w-full">
			<b>GDI LIBRARY</b>
		</div>
	</div>
	<div class="bg-neutral-700 py-2 w-full sm:h-16 shadow flex flex-col sm:flex-row justify-evenly items-center gap-4">
		<div class:active={$page.url.pathname === '/'}>
			<a sveltekit:prefetch href="/">HOMEPAGE</a>
		</div>
		<div class:active={$page.url.pathname === '/problems'}>
			<a sveltekit:prefetch href="/problems">PROBLEMS</a>
		</div>
		<div class:active={$page.url.pathname === '/about'}>
			<a sveltekit:prefetch href="/about">GIỚI THIỆU</a>
		</div>
		<div class:active={$page.url.pathname === '/contact'}>
			<a sveltekit:prefetch href="/contact">LIÊN HỆ</a>
		</div>
	</div>
</header>