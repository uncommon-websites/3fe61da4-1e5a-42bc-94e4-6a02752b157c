<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconHeart from "~icons/lucide/heart";
	import IconZap from "~icons/lucide/zap";
	import IconStar from "~icons/lucide/star";
	import IconRocket from "~icons/lucide/rocket";
	import IconUsers from "~icons/lucide/users";
	import IconSparkles from "~icons/lucide/sparkles";
</script>

<Hero
	title="Professional React components that ship faster"
	subtitle="Skip the generic AI outputs. Get taste-driven components curated by real product teams."
	centered={false}
	callsToAction={[
		{
			href: "/components",
			label: "Browse components"
		},
		{
			href: "/docs",
			label: "Get started"
		}
	]}
/>
<LogoScroller 
	label="Trusted by engineering teams at"
	logoUrls={[
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/figma.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/linear.app/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we deliver"
	text="21st provides curated React components built by real product teams, not generic AI outputs. Frontend developers at venture-backed startups choose our library to ship polished interfaces faster while maintaining the design quality that sets their products apart from the competition."
/>

<Testimonials
	testimonials={[
		{
			name: "Marcus Chen",
			position: "Senior Frontend Engineer",
			company: "Velocity Labs",
			quote:
				"21st saved us 3 weeks on our landing page rebuild. Instead of building components from scratch, we shipped professional-quality UI in days. The taste-driven designs meant zero back-and-forth with our design team.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Elena Rodriguez",
			position: "Tech Lead",
			company: "Startup Forge",
			quote:
				"Before 21st, I spent 40% of my time recreating basic components. Now I focus on product features while shipping interfaces that look like they came from a top-tier design team. ROI was immediate.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "David Okafor",
			position: "Engineering Manager",
			company: "Growth Stack",
			quote:
				"21st eliminated the component lottery for our team. No more inconsistent UI or hours debating button styles. Our developers ship faster and our product feels cohesive across every screen.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Why developers choose 21st"
	subtitle="Professional components that ship faster without compromising on design quality"
	features={[
		{
			title: "Human-curated components",
			description: "Skip generic AI outputs and get taste-driven components validated by real product teams at successful startups.",
			icon: IconHeart
		},
		{
			title: "Ship in minutes, not hours",
			description: "Stop rebuilding basic UI elements from scratch and focus on features that matter to your users.",
			icon: IconZap
		},
		{
			title: "Impress stakeholders",
			description: "Professional polish that makes your demos shine and builds confidence with investors and team leads.",
			icon: IconStar
		},
		{
			title: "Built for startups",
			description: "Components designed for fast-moving teams who need to iterate quickly without sacrificing quality.",
			icon: IconRocket
		},
		{
			title: "Community-driven quality",
			description: "Battle-tested components from Discord communities and GitHub discussions, not isolated development.",
			icon: IconUsers
		},
		{
			title: "Beyond cookie-cutter design",
			description: "Distinctive components that help your product stand out in a sea of identical interfaces.",
			icon: IconSparkles
		}
	]}
/>
<AboutTeaser />
<CallToAction generating />
