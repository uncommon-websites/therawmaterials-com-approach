<script lang="ts">
	import SectionHeader from "$lib/components/SectionHeader.svelte";
</script>

<div class="bg-white min-h-screen">
	<!-- Hero Section -->
	<section class="min-h-[60vh] flex flex-col justify-between p-6 pt-24 pb-12 relative">
		<div class="w-full flex justify-center mb-12">
			<svg viewBox="0 0 200 100" class="w-full max-w-3xl h-auto" fill="black">
				<!-- R -->
				<path d="M0 0 H80 C120 0 120 60 80 60 H40 V100 H0 V0 M40 30 H80 C90 30 90 40 80 40 H40 V30" />
				<!-- M -->
				<path d="M110 0 H140 L160 60 L180 0 H210 V100 H180 V40 L160 100 L140 40 V100 H110 V0" />
			</svg>
		</div>
		
		<div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-end">
			<div class="text-xs font-mono uppercase tracking-wide">
				The fastest way to launch<br>
				unusually creative digital<br>
				products that change industry<br>
				fortunes.
			</div>
		</div>
	</section>

	<!-- 01 Hello -->
	<section id="hello" class="relative">
		<SectionHeader number="01" title="Hello" color="bg-rm-red" />
		<div class="px-4 pb-20">
			<h1 class="text-[12vw] leading-[0.85] font-medium tracking-tight mb-12">
				We Are<br>
				<span class="text-rm-red">Raw</span><br>
				Materials
			</h1>

			<div class="grid grid-cols-1 md:grid-cols-12 gap-8 mb-24">
				<div class="md:col-span-4">
					<p class="text-xs font-mono mb-4">(Mission)</p>
				</div>
				<div class="md:col-span-8">
					<p class="text-4xl md:text-5xl font-medium leading-tight mb-12">
						Product design needs to be a creative endeavor.
					</p>
					<p class="text-4xl md:text-5xl font-medium leading-tight mb-12 text-gray-400">
						Optimization and incremental thinking are leading to the death of innovation and a lack of originality.
					</p>
					<p class="text-4xl md:text-5xl font-medium leading-tight text-rm-red">
						When everything is the same, being different is the greatest opportunity.
					</p>
				</div>
			</div>

			<div class="bg-gray-100 p-8 md:p-16 rounded-3xl mb-8">
				<div class="grid grid-cols-1 md:grid-cols-12 gap-8">
					<div class="md:col-span-4">
						<span class="text-xs font-mono">(Our Motion)</span>
					</div>
					<div class="md:col-span-8">
						<h3 class="text-4xl font-medium mb-12">We are building Raw Materials to:</h3>
						
						<div class="flex gap-4 mb-8">
							<span class="text-xs font-mono mt-2">(Challenge)</span>
							<p class="text-3xl font-medium">Help ambitious leaders escape the <span class="text-rm-red border-b border-rm-red">culture of conformity</span>.</p>
						</div>

						<div class="flex gap-4">
							<span class="text-xs font-mono mt-2">(Goal)</span>
							<p class="text-3xl font-medium">Design a better <span class="text-rm-red border-b border-rm-red">way forward</span>.</p>
						</div>
					</div>
				</div>
			</div>

			<!-- Unusual Wins Card -->
			<div class="bg-gradient-to-br from-orange-500 to-rm-red p-8 md:p-24 rounded-3xl text-white mb-8 text-center">
				<h2 class="text-6xl md:text-8xl font-medium tracking-tight">
					Unusual<br>Wins
				</h2>
			</div>

			<!-- Team Grid -->
			<div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-8">
				{#each [1, 2, 3] as i}
					<div class="bg-gray-100 aspect-[3/4] rounded-xl relative overflow-hidden group">
						<div class="absolute inset-0 bg-gray-200 flex items-center justify-center text-gray-400">
							Person {i}
						</div>
						<div class="absolute bottom-4 left-4">
							<p class="text-sm font-bold text-rm-red">Name Here</p>
							<p class="text-xs text-gray-500">Title Here</p>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- 02 Approach -->
	<section id="approach" class="relative">
		<SectionHeader number="02" title="Approach" color="bg-rm-purple" />
		<div class="px-4 pb-20">
			<div class="bg-rm-purple text-white p-8 md:p-16 rounded-3xl mb-8 overflow-hidden">
				<h2 class="text-[10vw] leading-none font-bold tracking-tighter text-center mix-blend-overlay opacity-50">
					Better is<br>different
				</h2>
			</div>

			<div class="bg-gray-100 p-8 md:p-16 rounded-3xl mb-8">
				<div class="grid grid-cols-1 md:grid-cols-12 gap-8">
					<div class="md:col-span-4">
						<span class="text-xs font-mono text-rm-purple">(Challenge)</span>
					</div>
					<div class="md:col-span-8">
						<p class="text-4xl md:text-5xl font-medium leading-tight mb-12 text-rm-purple">
							Rigor & Romance.<br>
							Method and imagination in equal measure.
						</p>
						<p class="text-3xl md:text-4xl font-medium leading-tight text-gray-500">
							Finding the best <span class="text-rm-purple">talent</span> in the world and helping them make the best work of their lives.
						</p>
					</div>
				</div>
			</div>

			<div class="bg-rm-purple text-white p-4 text-center rounded-xl mb-4">
				<h3 class="text-2xl font-medium">Independent in Ownership & Spirit</h3>
			</div>
		</div>
	</section>

	<!-- 03 Work -->
	<section id="work" class="relative">
		<SectionHeader number="03" title="Work" color="bg-rm-black" />
		<div class="px-4 pb-20 bg-rm-black min-h-screen pt-8">
			<div class="space-y-1">
				{#each ['7-Eleven Mobile', 'YOTI Charging', 'BMW Ai', 'BBI HOW-TO-QUIT', 'Jift Design', 'NBC Universal', 'Unity', 'Grammarly'] as client}
					<div class="border-t border-gray-800 py-6 flex justify-between items-center text-white hover:bg-gray-900 px-4 transition-colors cursor-pointer group">
						<span class="text-xl font-medium">{client}</span>
						<span class="text-xs text-gray-500 group-hover:text-white">View Case Study -></span>
					</div>
				{/each}
				<div class="border-t border-gray-800"></div>
			</div>
		</div>
	</section>

	<!-- 04 Talent -->
	<section id="talent" class="relative">
		<SectionHeader number="04" title="Talent" color="bg-rm-blue" />
		<div class="px-4 pb-20">
			<div class="bg-rm-blue text-white p-8 md:p-24 rounded-3xl mb-8 text-center overflow-hidden relative">
				<div class="text-[15vw] font-bold leading-none opacity-20 absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-full">
					RTN
				</div>
				<h2 class="text-4xl md:text-6xl font-medium relative z-10">
					The <span class="text-rm-red">(R)</span>aw<br>
					<span class="bg-white text-rm-blue px-2 rounded-full inline-block w-12 h-12 leading-[3rem] text-center text-3xl mx-1">T</span>alent<br>
					<span class="text-black italic">(N)</span>etwork
				</h2>
			</div>

			<div class="bg-rm-blue p-8 md:p-16 rounded-3xl text-white text-center">
				<p class="text-3xl md:text-5xl font-medium leading-tight">
					Finding the best talent in the world and helping them make the best work of their lives.
				</p>
			</div>
		</div>
	</section>

	<!-- 05 Careers -->
	<section id="careers" class="relative">
		<SectionHeader number="05" title="Careers" color="bg-rm-pink" />
		<div class="px-4 pb-20">
			<div class="bg-gray-100 p-8 md:p-16 rounded-3xl mb-8">
				<h2 class="text-5xl md:text-7xl font-medium leading-tight mb-12">
					We <span class="inline-block border border-gray-300 rounded-full px-6 py-2 text-2xl align-middle">Are</span> Looking <span class="inline-block border border-gray-300 rounded-full px-6 py-2 text-2xl align-middle">For</span> The <span class="bg-rm-pink text-white px-4 rounded-lg">Unusually</span> <span class="bg-black text-white px-4 rounded-lg">Talented</span>
				</h2>

				<div class="space-y-4">
					{#each ['Creative Product Design', 'Creative Motion Design', 'For the Top Unusual'] as job}
						<div class="bg-white p-4 rounded-xl flex justify-between items-center hover:shadow-lg transition-shadow cursor-pointer">
							<span class="font-medium">{job}</span>
							<span class="text-xs bg-rm-pink text-white px-2 py-1 rounded">Apply</span>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</section>

	<!-- 06 Contact -->
	<section id="contact" class="relative">
		<SectionHeader number="06" title="Contact" color="bg-rm-yellow" textColor="text-black" />
		<div class="px-4 pb-20">
			<h2 class="text-[10vw] leading-none font-medium tracking-tight mb-12 text-center">
				Let's<br>Talk<br>Creativity
			</h2>

			<div class="grid grid-cols-1 md:grid-cols-3 gap-4">
				{#each ['New Business', 'News & Press', 'Join The Team'] as item}
					<div class="bg-rm-yellow aspect-square rounded-xl flex flex-col items-center justify-end p-4 relative overflow-hidden group">
						<div class="absolute inset-0 flex items-center justify-center">
							<!-- Placeholder for person image -->
							<div class="w-32 h-48 bg-black/10 rounded-full"></div>
						</div>
						<span class="relative z-10 font-medium">{item}</span>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- 07 Unusual Index -->
	<section id="index" class="relative">
		<SectionHeader number="07" title="Unusual Index" color="bg-rm-green" textColor="text-black" />
		<div class="px-4 pb-20 bg-rm-green min-h-screen relative overflow-hidden">
			<!-- Grid Pattern -->
			<div class="absolute inset-0 opacity-20 pointer-events-none" 
				style="background-image: linear-gradient(#000 1px, transparent 1px), linear-gradient(90deg, #000 1px, transparent 1px); background-size: 40px 40px;">
			</div>

			<div class="bg-white/50 p-8 rounded-3xl mb-8 backdrop-blur-sm relative z-10">
				<h2 class="text-[15vw] leading-none font-medium tracking-tight text-center opacity-20 mix-blend-overlay">
					Index
				</h2>
			</div>
			
			<div class="p-8 md:p-16 relative z-10">
				<p class="text-3xl md:text-5xl font-medium leading-tight">
					The (Unusual) Index is our compendium of unusually great products, people, and ideas that inspire us to think differently.
				</p>
				
				<div class="mt-12">
					<button class="bg-black text-white px-8 py-4 rounded-full text-lg font-medium hover:bg-gray-800 transition-colors">
						View the Index
					</button>
				</div>
			</div>
		</div>
	</section>

	<footer class="bg-gray-100 p-8 text-center text-xs text-gray-500">
		&copy; 2024 Raw Materials. All rights reserved.
	</footer>
</div>

