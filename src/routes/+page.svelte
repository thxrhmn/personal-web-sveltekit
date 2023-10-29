<script>
	import '../app.css';
	import Nav from '../components/Nav.svelte';
	import Project from '../components/Project.svelte';

	import dataStatic from './dataStatic';
</script>

<div class="font-jetbrains-mono flex justify-center mx-[20%]">
	<div class="w-[500px] mt-10 flex flex-col gap-8">
		<div class="flex justify-center">
			<img class="w-[100px] rounded-full" src="/img.jpg" alt="avatarku" />
		</div>
		<div>
			<h1 class="text-center">{dataStatic.about.header.text}</h1>
			<h1 class="text-center">{dataStatic.about.header.text2}</h1>
		</div>

		<Nav />
		<div class="flex flex-col gap-5">
			<h3 class="first-letter:text-4xl first-letter:pr-1">{dataStatic.about.bio.text1}</h3>
			<h3>{dataStatic.about.bio.text2}</h3>
		</div>

		<div class="flex flex-col gap-5">
			<h1 class="font-bold text-center">Projects</h1>
			<Project />
		</div>
	</div>
</div>
