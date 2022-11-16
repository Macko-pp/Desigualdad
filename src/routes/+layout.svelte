<script lang="ts">
	import "../app.postcss";
	import NotEquals from "./lib/not-equals.svelte"

	let audio: any;

	function playAudio() {
		setTimeout(() => {
			audio.play()
		},0)	
	}
</script>

<div class="navbar bg-slate-100 dark:bg-slate-800">
	<div class="flex-none">
		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<a href="/" on:click={playAudio}>
			<btn class="btn btn-square btn-ghost hover:bg-transparent spin">
				<NotEquals />
			</btn>
			<audio src="src/routes/lib/GreenGiant.mp3" bind:this={audio}></audio>
		</a>
	</div>
	<div class="flex-1">
		<a class="btn btn-ghost normal-case text-xl font-extrabold pl-3" href="./">Desigualdad</a>
	</div>
	<div class="flex-none">
		<ul class="menu menu-horizontal p-0">
			<li><a class="btn btn-ghost normal-case" href="etnica">Desigualdad Étnica</a></li>
			<li><a class="btn btn-ghost normal-case" href="economica">Desigualdad Economica</a></li>
			<li><a class="btn btn-ghost normal-case" href="genero">Desigualdad de Genero</a></li>
			<li><a class="btn btn-ghost normal-case" href="educacion">Desigualdad Educativa</a></li>
		</ul>
	</div>
</div>

<div class="padded">
	<slot />
</div>

<style>
	@keyframes spin {
		0% {
			transform: rotate(0);
		}

		100% {
			transform: rotate(360deg);
		}
	}

	.spin {
		animation: spin 1s ease 0s 1 normal forwards;
	}

	.padded {
		padding: 50px;
	}
</style>
