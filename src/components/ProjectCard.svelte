<script>
	export let nome;
	export let tipo;
	export let immagine;
</script>

<!-- svelte-ignore a11y-mouse-events-have-key-events -->
<div
	class="max-w-xs sm:max-w-md md:max-w-xl m-14 h-auto flex flex-col  rounded-xl bg-gray-800 dark:bg-green-400 hover:shadow-lg ease-linear duration-100 sm:hover:scale-105"
	style="scroll-snap-align:center;"
>
	<div class="topPart md:flex-shrink-0">
		<img
			class=" max-w-xs sm:max-w-md md:max-w-lg rounded-xl rounded-b-none"
			src="images\projects\{immagine}.jpg"
			alt=""
		/>
	</div>
	<div class="bottomPart w-full h-full grid grid-cols-2 items-center justify-items-center">
		<div class="p-5 testi flex flex-col gap-5">
			<h2 class="text-left text-xl md:text-2xl font-semibold text-green-500 dark:text-gray-800">
				{nome}
			</h2>
			<p class="text-sm md:text-md text-white">
				Tipo: <span class="italic"> {tipo}</span>
			</p>
		</div>
		<a
			href="/progetti/{nome}"
			class="flex w-min whitespace-nowrap h-1/3 items-center bg-green-400 dark:bg-gray-800 text-gray-800 dark:text-green-400  hover:scale-105  hover:bg-white dark:hover:text-gray-800 cursor-pointer first-letter:duration-100 transition-all  ease-linear p-3  rounded-md font-semibold"
		>
			More Info
		</a>
	</div>
</div>
