<script lang="ts">
	export let activeSection = "hello";

	const sections = [
		{ id: "hello", number: "01", label: "Hello", color: "bg-rm-red", text: "text-white" },
		{ id: "approach", number: "02", label: "Approach", color: "bg-rm-purple", text: "text-white" },
		{ id: "work", number: "03", label: "Work", color: "bg-rm-black", text: "text-white" },
		{ id: "talent", number: "04", label: "Talent", color: "bg-rm-blue", text: "text-white" },
		{ id: "careers", number: "05", label: "Careers", color: "bg-rm-pink", text: "text-white" },
		{ id: "contact", number: "06", label: "Contact", color: "bg-rm-yellow", text: "text-black" },
		{ id: "index", number: "07", label: "Unusual Index", color: "bg-rm-green", text: "text-black" }
	];
</script>

<aside class="sticky top-0 h-screen w-24 flex flex-col gap-2 p-2 pt-20 overflow-y-auto no-scrollbar">
	{#each sections as section}
		<a
			href="#{section.id}"
			class="flex flex-col items-start justify-between p-2 rounded-lg transition-all duration-300 h-24 w-full {section.color} {section.text} hover:opacity-90"
		>
			<span class="text-xs font-bold">{section.number}</span>
			<span class="text-[10px] font-medium leading-tight break-words w-full">{section.label}</span>
		</a>
	{/each}
</aside>
