<script>
	import { page } from "$app/stores";
	$: path = $page.url.pathname;
	$: basePath = path.includes("/sveltekit-starting-app")
		? "/sveltekit-starting-app/"
		: "/";
</script>

<nav class="flex gap-10 p-6 border-b-2">
	<a href={basePath} class:font-bold={$page.url.pathname == basePath}>Home</a>
	<a
		href={basePath + "about"}
		class:font-bold={$page.url.pathname == basePath + "/about"}>About</a
	>
</nav>
