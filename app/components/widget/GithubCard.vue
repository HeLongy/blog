<script setup lang="ts">
const repo = {
	name: 'HeLongy/blog',
	description: '本站主题 Github 仓库',
	url: 'https://github.com/HeLongy/blog',
}
</script>

<template>
<ZWidget title="GitHub 仓库">
	<ZRawLink v-if="repo" class="github-Widget" :to="repo.url">
		<div class="de">
			<div class="name">
				{{ repo.name }}
			</div>
			<div class="desc">
				{{ repo.description }}
			</div>
		</div>
		<div class="img">
			<iconify-icon icon="skill-icons:github-dark" width="26" height="26" />
		</div>
	</ZRawLink>
</ZWidget>
</template>