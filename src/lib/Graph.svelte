<script lang="ts">
	let canvas: HTMLCanvasElement;

	$effect(() => {
		const ctx = canvas.getContext("2d");
		if (ctx) {
			draw(ctx);
		}
	});

	function draw(ctx: CanvasRenderingContext2D) {
		ctx.fillStyle = "#27272a";
		ctx.fillRect(0, 0, 1000, 1000);

		ctx.strokeStyle = "#d4d4d8";
		ctx.lineWidth = 4;

		ctx.beginPath();
		ctx.moveTo(500, 0);
		ctx.lineTo(500, 1000);
		ctx.stroke();

		ctx.beginPath();
		ctx.moveTo(0, 500);
		ctx.lineTo(1000, 500);
		ctx.stroke();

		for (let i = 0; i <= 40; i++) {
			ctx.beginPath();
			ctx.moveTo(i * 25, 490);
			ctx.lineTo(i * 25, 510);
			ctx.stroke();
		}
		for (let i = 0; i <= 40; i++) {
			ctx.beginPath();
			ctx.moveTo(490, i * 25);
			ctx.lineTo(510, i * 25);
			ctx.stroke();
		}
	}
</script>

<div class="aspect-square border-l-2 border-zinc-400">
	<canvas bind:this={canvas} width="1000" height="1000" class="size-full">
		Please update your browser
	</canvas>
</div>
