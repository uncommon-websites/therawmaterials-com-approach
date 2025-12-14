<script lang="ts">
	import "../app.css";
	import Sidebar from "$lib/components/Sidebar.svelte";
</script>

<div class="flex min-h-screen bg-rm-bg">
	<div class="hidden md:block w-24 shrink-0">
		<Sidebar />
	</div>
	<div class="flex-1">
		<header class="fixed top-0 left-0 md:left-24 right-0 z-50 flex justify-between items-start p-6 mix-blend-difference text-white pointer-events-none">
			<div class="flex flex-col">
				<span class="text-sm font-medium">Raw</span>
				<span class="text-sm font-medium">Materials</span>
			</div>
			
			<div class="text-right">
				<span class="text-sm font-medium block">An Unusual</span>
				<span class="text-sm font-medium block">Design Company</span>
			</div>
		</header>
		
		<div class="fixed top-6 left-1/2 -translate-x-1/2 z-50 mix-blend-difference text-white pointer-events-none">
			<svg width="120" height="80" viewBox="0 0 120 80" fill="currentColor">
				<path d="M0 0h15v80H0V0zm25 0h45c15 0 25 10 25 25s-10 25-25 25h-30v30H25V0zm15 15v20h30c7 0 10-3 10-10s-3-10-10-10H40zm60 0h15l15 80h-15l-12-65-12 65H76l15-80z" />
			</svg>
		</div>

		<slot />
	</div>
</div>
