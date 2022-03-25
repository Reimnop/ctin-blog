<script>
	import { page } from '$app/stores';
</script>

<header>
	<div class="bg-neutral-700 py-2 m-4">
		<ul class="flex flex-col sm:flex-row items-center gap-2 justify-evenly text-neutral-300">
			<li class:active={$page.url.pathname === '/'}>
				<a sveltekit:prefetch href="/">TRANG CHỦ</a>
			</li>
			<li class:active={$page.url.pathname === '/classwork'}>
				<a sveltekit:prefetch href="/classwork">BÀI TẬP</a>
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