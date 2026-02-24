<template>
	<section id="featured" class="mt-5 pb-4">
		<div class="container">
			<h2 class="mb-4 text-center">Featured Products</h2>

			<div
			v-for="(group, index) in chunkedProjects"
			:key="index"
			class="row"
			>
				<ProjectCard v-for="project in group"
				:key="project.id"
				:project="project"
				>
				</ProjectCard>
			</div>
		</div>
	</section>
	
</template>

<script setup>
	import {computed} from 'vue';

	import ProjectCard from './FeaturedCard.vue';
	import projects from '../data/featured.json';

	const chunkSize = 3;

	const chunkedProjects = computed(() => {
		const chunks = [];

		for (let i = 0; i < projects.length; i+=chunkSize) {
			chunks.push(projects.slice(i, i + chunkSize));
		}

		return chunks;
	})
</script>