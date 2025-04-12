<script lang="ts">
	const tries = $state([
		["", "", "", "", "", ""],
		["", "", "", "", "", ""],
		["", "", "", "", "", ""],
		["", "", "", "", "", ""],
		["", "", "", "", "", ""],
		["", "", "", "", "", ""],
	]) as string[][];
</script>

<div class="size-full flex flex-col gap-4 justify-center items-center">
	{#each tries as tryEntry}
		<div class="flex flex-row gap-4">
			{#each tryEntry as char}
				<div
					class="w-12 h-12 text-center content-center text-2xl font-semibold font-serif italic bg-zinc-700"
				>
					{char}
				</div>
			{/each}
		</div>
	{/each}
</div>
