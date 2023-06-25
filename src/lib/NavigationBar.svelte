<script>
    import { page } from '$app/stores';
</script>

<nav class="flex gap-10 p-6 border-b-2">
    <a href="/sveltekit-starting-app" class:font-bold={$page.url.pathname == '/sveltekit-starting-app'}>Home</a>
    <a href="/sveltekit-starting-app/about" class:font-bold={$page.url.pathname == '/sveltekit-starting-app/about'}>About</a>
</nav>