    
<script lang="ts">
	const projects = [
		{
			title: 'Project One: E-Commerce Platform',
			description:
				'A full-stack e-commerce site built with SvelteKit, Stripe for payments, and Prisma for the database. Features product search, user authentication, and an admin dashboard.',
			tech: ['SvelteKit', 'TypeScript', 'Stripe', 'Prisma', 'TailwindCSS'],
			liveUrl: '#',
			sourceUrl: '#'
		},
		{
			title: 'Project Two: Real-time Chat App',
			description:
				'A WebSocket-based chat application allowing users to join rooms and communicate in real-time. Built with Node.js on the backend and Svelte on the frontend.',
			tech: ['Svelte', 'Node.js', 'WebSocket', 'Express'],
			liveUrl: '#',
			sourceUrl: '#'
		}
	];
</script>

<svelte:head>
	<title>Your Name | Software Developer</title>
	<meta name="description" content="Personal portfolio of Your Name, a passionate developer." />
</svelte:head>

<div class="max-w-3xl mx-auto px-4 py-16 sm:py-24 space-y-16">
	<!-- SECTION: Hero / Introduction -->
	<section class="text-center md:text-left md:flex md:items-center md:justify-between">
		<div>
			<h1 class="text-4xl md:text-5xl font-extrabold tracking-tight text-primary">
				Your Name
			</h1>
			<h2 class="mt-2 text-xl md:text-2xl text-muted-foreground">
				A passionate developer creating modern web experiences.
			</h2>
			<p class="mt-4 max-w-xl mx-auto md:mx-0 text-lg text-foreground/80">
				I specialize in building fast, accessible, and beautiful applications with SvelteKit,
				TypeScript, and modern web technologies.
			</p>
		</div>

		<div class="mt-8 md:mt-0 flex justify-center md:justify-start gap-2">
		</div>
	</section>

	<!-- SECTION: Projects -->
	<section class="space-y-8">
		<h2 class="text-3xl font-bold tracking-tight text-primary border-b pb-2">Featured Projects</h2>
		<div class="space-y-12">
			{#each projects as project, i}
				<div
					class="grid grid-cols-1 md:grid-cols-[1fr,2fr] gap-4 md:gap-8 items-start"
				>
					<h3 class="text-lg font-semibold text-muted-foreground md:text-right">
						{project.title}
					</h3>
					<div class="space-y-4">
						<p class="text-foreground/90">
							{project.description}
						</p>
						<div class="flex flex-wrap gap-2">
							{#each project.tech as tech}
								<span
									class="inline-flex items-center rounded-md bg-secondary px-2.5 py-0.5 text-sm font-medium text-secondary-foreground"
								>
									{tech}
								</span>
							{/each}
						</div>
						<div class="flex items-center gap-4 mt-2">
						</div>
					</div>
				</div>
			{/each}
		</div>
	</section>
</div>

  