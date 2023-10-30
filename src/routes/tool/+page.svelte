<script>
	import Nav from '../../components/Nav.svelte';
    import dataStatic from '../../data/dataStatic';
</script>

<div class="font-jetbrains-mono flex justify-center mx-[5%]">
	<div class="w-[500px] mt-10 flex flex-col gap-8">
		<Nav />
        <h1 class="text-lg font-semibold text-center">Tools</h1>
        <div class="flex flex-col gap-x-5 gap-y-2 justify-center">
            {#each dataStatic.tools as tool, idx}
                <h1 class="">{idx+1}. {tool.name}</h1>
            {/each}
        </div>
	</div>
</div>
