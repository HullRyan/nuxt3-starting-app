<script setup>
defineProps(["title", "body"]);
</script>

<template>
	<div>
		<div class="flex flex-col items-center justify-between p-12">
			{{ title }}
		</div>
		<div class="flex flex-col items-center justify-between p-16">
			{{ body }}
		</div>
	</div>
</template>
