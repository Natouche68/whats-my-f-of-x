<script lang="ts">
	import Tries from "$lib/Tries.svelte";
	import Graph from "$lib/Graph.svelte";
</script>

<div class="w-full py-4 text-center border-b-2 border-zinc-400">
	<h1 class="text-3xl font-bold uppercase">
		What's my <span class="normal-case italic font-serif font-semibold">
			f(x)
		</span> ?
	</h1>
</div>

<div class="flex flex-row">
	<Tries />
	<Graph />
</div>
