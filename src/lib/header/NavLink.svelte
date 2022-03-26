<script>
    import { page } from "$app/stores";

    export let href;
</script>

<a sveltekit:prefetch href={href} class="nav-link" class:nav-active={$page.url.pathname === href}>
    <slot />
</a>