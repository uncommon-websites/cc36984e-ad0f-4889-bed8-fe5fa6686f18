<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Talia Nguyen",
      position: "CEO",
      company: "Basis",
      quote:
        "Donna gives me 10 status meetings worth of clarity in a 30-second read. We save hours every week—and I always know where to focus.",
      image: "/generated/image-a-professional-headshot-of-a-vietnamese-.webp"
    },
    {
      name: "Matteo Rosser",
      position: "COO",
      company: "Answerly",
      quote:
        "The productivity insights showed us why the engineering org was slowing down—before metrics ever would. Donna paid for itself in the first month.",
      image: "/generated/image-a-professional-headshot-of-a-black-briti.webp"
    },
    {
      name: "Cheryl Lynn",
      position: "Founder",
      company: "Signal & Source",
      quote:
        "It’s like having someone quietly update me on what matters every single day, without bothering anyone on the team. Setup was instant and everyone felt the impact right away.",
      image: "/generated/image-a-professional-headshot-of-an-east-asian.webp"
    }
  ]}
/>

<CallToAction
  title="Lead without the meetings"
  subtitle="Know what matters, before anyone needs to tell you"
  description="Donna is your AI Chief of Staff—offering daily, real-time visibility into projects, blockers, and productivity, no status meetings required. See what moves, what needs attention, and where to focus next. White-glove onboarding is included. Spots are limited."
  imageSrc="/generated/image-a-happy-executive-in-a-modern-office-env.webp"
  callsToAction={[
    { href: '/contact', label: 'Request access', variant: 'primary' },
    { href: 'mailto:founders@bondapp.io', label: 'Talk to founders', variant: 'secondary' }
  ]}
/>
