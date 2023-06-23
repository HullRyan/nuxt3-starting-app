<template>
	<div className="flex flex-col items-center justify-between">
		<div
			className="flex flex-col items-center gap-4 p-6 w-96 h-48 border rounded-lg"
		>
			<div className="font-bold flex flex-col items-center justify-between p-1">
				Count: {{ count }}
			</div>
			<button @click="count++" className="rounded-lg bg-slate-200 hover:bg-slate-300 p-2">
				Click Me
			</button>
			<div
				className="flex flex-col items-center justify-between p-1"
				v-show="count % 2 == 0"
			>
				{{ description }}
			</div>
		</div>
	</div>
</template>

<script setup>
defineProps(["description"]);

const count = useState("count", () => 0);
</script>
