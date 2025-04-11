<script lang="ts">
	import "../app.css";

	let { children } = $props();
</script>

<svelte:head>
	<title>What's my f(x) ?</title>
</svelte:head>

<div class="w-screen h-screen bg-zinc-900 text-zinc-100">
	{@render children()}
</div>
