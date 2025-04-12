<script lang="ts">
	import "../app.css";

	let { children } = $props();
</script>

<svelte:head>
	<title>What's my f(x) ?</title>
</svelte:head>

<div class="h-screen bg-zinc-900 text-zinc-100">
	<div
		class="w-full h-20 text-center content-center border-b-2 border-zinc-400"
	>
		<h1 class="text-3xl font-bold uppercase">
			What's my <span class="normal-case italic font-serif font-semibold">
				f(x)
			</span> ?
		</h1>
	</div>
	<div class="h-[calc(100%-5rem)]">
		{@render children()}
	</div>
</div>
