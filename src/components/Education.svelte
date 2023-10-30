<script>
	import dataStatic from '../data/dataStatic';
	import Nav from './Nav.svelte';
</script>

<div class="font-jetbrains-mono flex justify-center mx-[20%]">
	<div class="w-[500px] mt-10 flex flex-col gap-8">
        <Nav />
		<div class="flex flex-col gap-5">
			<h1 class="font-bold text-center">Educations</h1>
			<ol class="relative border-l border-black dark:border-gray-700">
				{#each dataStatic.about.educations as item}
					<li class="mb-5 last:mb-0 ml-4">
						<div
							class="absolute w-3 h-3 bg-black rounded-full mt-1.5 -left-1.5 border border-white dark:border-black dark:bg-black"
						/>
						<time class="mb-1 text-sm font-normal leading-none italic">
							{item.graduation}
						</time>
						<h3 class="text-md">{item.name}</h3>
						<p class="text-base font-normal">{item.major}</p>
					</li>
				{/each}
			</ol>
		</div>
	</div>
</div>
