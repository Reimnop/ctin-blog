<script>
	import { page } from '$app/stores';
</script>

<div class="sticky w-[380px] h-[100vh] bg-slate-800 flex flex-col gap-4 shadow-colored">
	<div class="flex flex-row p-4 items-center w-full">
		<img src="https://upload.wikimedia.org/wikipedia/vi/c/c9/Logo_Thpt_Gia_Dinh.gif" alt="GiaDinh" width="110" height="110"/>
		<div class="title relative text-center text-6xl w-full">
			<b>GDI LIBRARY</b>
		</div>
	</div>
	<div class="nav-link" class:active={$page.url.pathname === '/'}>
		<a sveltekit:prefetch href="/">🏠 HOMEPAGE</a>
	</div>
	<div class="nav-link" class:active={$page.url.pathname === '/problems'}>
		<a sveltekit:prefetch href="/problems">📜 PROBLEMS</a>
	</div>
	<div class="nav-link" class:active={$page.url.pathname === '/about'}>
		<a sveltekit:prefetch href="/about">🎤 GIỚI THIỆU</a>
	</div>
	<div class="nav-link" class:active={$page.url.pathname === '/contact'}>
		<a sveltekit:prefetch href="/contact">📞 LIÊN HỆ</a>
	</div>
</div>