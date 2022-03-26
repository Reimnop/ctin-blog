<script>
    import { page } from "$app/stores";

    export let href;
    export let content;
</script>

<a sveltekit:prefetch href={href} class="nav-link" class:nav-active={$page.url.pathname === href}>{content}</a>