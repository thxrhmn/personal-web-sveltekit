<script>
	import dataStatic from '../routes/dataStatic';
</script>

<ol class="relative border-l border-gray-200 dark:border-gray-700">
	{#each dataStatic.projects as item}
		<li class="mb-10 ml-4">
			<div
				class="absolute w-3 h-3 bg-gray-200 rounded-full mt-1.5 -left-1.5 border border-white dark:border-black dark:bg-black"
			/>
			<time class="mb-1 text-sm font-normal leading-none italic">
				{item.process}
			</time>
			<h3 class="project-name font-semibold">{item.name}</h3>
			<p class="mb-4 text-base font-normal">{item.desc}</p>
			<div class="flex">
				<h5 class="text-sm mr-3">stacks:</h5>
				<ul class="flex text-sm project-stacks gap-3">
					{#each item.stacks as itm}
						<li class="underline">
							{itm.name}
						</li>
					{/each}
				</ul>
			</div>
			<div class="flex">
				<!-- <Link href={item.linkGH}>
            <Image
              class="rounded-full project-stacks-link"
              src="/github.svg"
              alt="Github Logo"
              width={15}
              height={15}
            />
          </Link>
          <Link href={item.linkProd}>
            <Image
              class="rounded-full project-stacks-link"
              src="/network.svg"
              alt="Network Logo"
              width={15}
              height={15}
            />
          </Link> -->
			</div>
		</li>
	{/each}
</ol>
