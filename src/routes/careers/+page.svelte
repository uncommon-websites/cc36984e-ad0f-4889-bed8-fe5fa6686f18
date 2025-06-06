<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Flexible Work",
			description: "Remote-first with flexible hours that respect work-life balance.",
			icon: IconBriefcase
		},
		{
			title: "Growth Opportunities",
			description: "Continuous learning with mentorship and education stipends.",
			icon: IconUsers
		},
		{
			title: "Comprehensive Benefits",
			description: "Health coverage, retirement plans, and generous paid time off.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
	{
		name: "Alex Chen",
		position: "Engineering Manager",
		company: "Engineering Team",
		quote:
			"Mentorship and growth are part of every day here. I have the freedom to tackle ambitious projects, but there’s always someone willing to lend a hand or share advice. The learning never stops—and neither does the support.",
		image:
			"/generated/image-an-asian-male-engineering-manager-in-a-m.webp"
	},
	{
		name: "Danielle Brooks",
		position: "Product Designer",
		company: "Design Team",
		quote:
			"From day one, people made me feel like my ideas matter. The culture is inclusive, kind, and honestly—fun. I know my voice is heard, and that inspires me to do my best work.",
		image:
			"/generated/image-a-young-black-woman-product-designer-in-.webp"
	},
	{
		name: "Carlos Ramirez",
		position: "Operations Specialist",
		company: "Operations",
		quote:
			"Donna has become like a second family. Leadership is approachable and genuinely cares about balance, not just results. I can focus on my work knowing I’m trusted and valued.",
		image:
			"/generated/image-a-latino-male-operations-specialist-in-a.webp"
	}
];

	const processSteps = [
	{
		step: 1,
		title: "Apply",
		description: "Send your resume or LinkedIn and a brief note on why you're interested—no cover letter required."
	},
	{
		step: 2,
		title: "Intro call",
		description: "A quick conversation with one of our founders to align on goals and answer your questions."
	},
	{
		step: 3,
		title: "Practical challenge",
		description: "A realistic async or live task (1–2 hours max) so your skills and thinking can shine."
	},
	{
		step: 4,
		title: "Final interview",
		description: "Meet with founders and team, discuss approach and values, and get a sense of day-to-day collaboration."
	}
];

	const values = [
		{
			icon: IconHeart,
			title: "Passion",
			description: "We're driven by a shared passion for innovation and excellence."
		},
		{
			icon: IconUsers,
			title: "Collaboration",
			description: "We believe in teamwork and collaboration to achieve great things."
		},
		{
			icon: IconGlobe,
			title: "Global Impact",
			description: "We're committed to making a positive impact on the world."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Build with purpose, lead with trust"
	subtitle="Make real impact alongside a brilliant, supportive team."
	imageSrc="/generated/image-a-modern-office-setting-featuring-a-dive.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Work with impact, growth, and trust" />

	<div class="prose max-w-screen-lg mx-auto text-lg mb-12">
		<ul>
			<li><strong>Build the future of executive work:</strong> Help reshape how leadership teams operate using cutting-edge AI.</li>
			<li><strong>Zero bureaucracy, high ownership:</strong> Move fast, make decisions, and see your work ship to top-tier executives weekly.</li>
			<li><strong>Direct impact, real companies:</strong> Work directly with CEOs and operators, and see your work used by real decision makers from day one.</li>
			<li><strong>Be part of something early:</strong> We’re growing fast—joining now will shape the product and the culture from the ground up.</li>
		</ul>
	</div>

	<div class="mt-10 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Our culture" subtitle="How we work and what we value" />
	<div class="prose max-w-screen-lg mx-auto text-lg mb-10">
		<ul>
			<li><strong>High standards, low ego:</strong> We work hard, obsess over quality, and respect each other equally.</li>
			<li><strong>Action wins:</strong> We prioritize speed and iteration over overthinking and presentations.</li>
			<li><strong>Build what matters:</strong> We care about solving real customer problems, not just shipping cool tech.</li>
			<li><strong>Default to trust:</strong> Everyone has freedom to explore and ownership to build—with accountability to deliver.</li>
			<li><strong>Clear, direct communication:</strong> Everyone is close to the founders and empowered to challenge ideas. No politics, just teamwork.</li>
			<li><strong>Diversity & balance:</strong> We’re committed to a supportive, inclusive team, and protecting work/life balance at every level.</li>
			<li><strong>Data privacy is our DNA:</strong> Everything we do puts privacy first—inside our product and inside our company.</li>
		</ul>
	</div>
</section>

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
