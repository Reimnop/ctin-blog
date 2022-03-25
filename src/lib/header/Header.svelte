<script>
	import { page } from '$app/stores';
</script>

<header class="flex flex-col sm:flex-row items-start">
	<img src="https://upload.wikimedia.org/wikipedia/vi/c/c9/Logo_Thpt_Gia_Dinh.gif" alt="GiaDinh" width="119"/>
	<div class="bg-neutral-700 py-2 m-4 w-full">
		<ul class="flex flex-col sm:flex-row items-center gap-2 justify-evenly text-neutral-300">
			<li class:active={$page.url.pathname === '/'}>
				<a sveltekit:prefetch href="/">HOMEPAGE</a>
			</li>
			<li class:active={$page.url.pathname === '/problems'}>
				<a sveltekit:prefetch href="/problems">PROBLEMS</a>
			</li>
			<li class:active={$page.url.pathname === '/about'}>
				<a sveltekit:prefetch href="/about">GIỚI THIỆU</a>
			</li>
			<li class:active={$page.url.pathname === '/contact'}>
				<a sveltekit:prefetch href="/contact">LIÊN HỆ</a>
			</li>
		</ul>
	</div>
</header>