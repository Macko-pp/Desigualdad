<script lang="ts">
	import Shrug from "./lib/shrug.svelte";
</script>

<div class="hero min-h-[40rem] rounded-t-2xl top border-b-2 border-[#FF5C5B]">
	<div class="hero-content flex-col lg:flex-row center">
		<div class="prose mx-10">
			<h1 class="text-7xl">La Desigualdad</h1>
			<p class="text-[#4A515C]">
				La desigualdad afecta a millones de personas en el mundo, incluso tú podrías estar sufriendo
				de la desigualdad. ¿Pero primero, que es la desigualdad?
			</p>
		</div>
	</div>
</div>

<div class="hero min-h-[40rem] bottom rounded-b-2xl">
	<div class="hero-content flex-col lg:flex-row">
		<div class="prose mx-10">
			<h1 class="font-bold">¿Qué Es?</h1>
			<p>
				La desigualdad es la injusticia más grande que existe entre todas las personas del planeta.
				Estas desigualdades pueden limitar los derechos humanos, por ejemplo a través de la
				discriminación, los abusos y la falta de acceso a la justicia, así como la esperanza de vida
				y el acceso a servicios esenciales como la sanidad, la educación, el agua y el saneamiento.
				Esto ocurre cuando una persona recibe un trato diferente en función de aspectos como él
				estatus social, el estatus económico, la religión, el género, la cultura o las preferencias
				sexuales.
			</p>
		</div>

		<div class="shrug ml-[-1.2rem]">
			<Shrug height="400px" />
			<p class="text-[7px] ml-44">
				Imagen por <b><u><a href="https://dribbble.com/shots/11108990-">Alberto Pozo</a></u></b> en Dribble
			</p>
		</div>
	</div>
</div>

<div class="center">
	<div class="prose">
		<h1 class="mt-20">Diferentes tipos de desigualdad</h1>
		<p>
			La desigualdad viene en muchas formas, se las voy a explicar de una manera dividida que las
			puedan entender todas mejor. La desigualdad <a href="etnica">étnica</a>, la desigualdad
			<a href="economica">económica</a>, la desigualdad de <a href="genero">género</a>, y la
			desigualdad <a href="educativa">educativa</a>. Presionen los links en la barra de navegación
			para aprender más.
		</p>

		<div class="bg-base-200 rounded-xl ml-[75px] p-[25px] max-w-[500px] center">
			<img
				class="h-[600px] rounded-xl"
				src="/poster(0).png"
				alt="El primer poster de la presentacion"
			/>
		</div>
	</div>
</div>

<style>
	h1 {
		color: var(--main);
	}

	.bottom {
		background-image: url("./lib/fall-bottom.png");
	}

	@media (prefers-color-scheme: dark) {
		.bottom {
			background-image: url("./lib/fall-bottom-dark.png");
		}
	}

	.top {
		background-image: url("./lib/blob-background.png");
	}
</style>
