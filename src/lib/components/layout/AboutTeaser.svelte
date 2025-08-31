<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Serafim",
		role: "Founder & Creator",
		image: "https://www.unc.mn/image-placeholder.svg"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"After watching brilliant developers at three different startups spend weeks recreating the same button components, I knew something was broken. We had incredible design talent in our Discord communities, but their best work stayed buried in conversations. 21st began as my rebellion against generic toolkits – it's become the curated library I wished existed when I was shipping my first React interfaces."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8">
				<div class="flex items-center justify-center gap-4 rounded-lg border border-border bg-card p-6 transition-colors hover:bg-muted/50">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-14 rounded-full object-cover ring-2 ring-border"
					/>
					<div class="flex-1">
						<div class="text-callout font-medium">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
					</div>
					<Button href="/about" variant="secondary" size="sm" class="shrink-0">Read the story</Button>
				</div>
			</div>
		</div>
	</div>
</section>
