<script>
	import Nav from '../../components/Nav.svelte';
    import dataStatic from '../dataStatic';
</script>

<div class="font-jetbrains-mono flex justify-center mx-[20%]">
	<div class="w-[500px] mt-10 flex flex-col gap-8">
		<Nav />
        <h1 class="text-lg font-semibold text-center">Skill</h1>
        <div class="flex flex-wrap gap-x-5 gap-y-2 justify-center">
            {#each dataStatic.programmingStack as stack}
                <h1 class="">{stack} ★</h1>
            {/each}
        </div>
	</div>
</div>
