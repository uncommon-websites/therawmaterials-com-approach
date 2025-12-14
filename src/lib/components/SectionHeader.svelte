<script lang="ts">
	export let number: string;
	export let title: string;
	export let color: string;
	export let textColor: string = "text-white";
</script>

<div class="sticky top-0 z-10 w-full p-4 {color} {textColor} mb-8">
	<div class="text-xl font-medium mb-2">{number}</div>
	<h2 class="text-6xl font-medium tracking-tight">{title}</h2>
</div>
