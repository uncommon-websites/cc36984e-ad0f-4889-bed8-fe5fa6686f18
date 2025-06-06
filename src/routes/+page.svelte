<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  centered={true}
  title="Your company’s pulse, at a glance"
  subtitle="Stay ahead with real-time project visibility and productivity insights—no chasing updates, no unnecessary meetings. Built for executives with enterprise-grade security and zero data retention."
  customers={[
    {
      name: "Emily Chen",
      position: "CEO, NextPhase Health",
      imageSrc: "/generated/image-a-confident-female-ceo-sitting-at-her-of.webp"
    },
    {
      name: "Michael Lee",
      position: "COO, Stratus Ventures",
      imageSrc: "/generated/image-a-smiling-male-executive-in-business-cas.webp"
    },
    {
      name: "Priya Sharma",
      position: "Head of Product, Broadwave",
      imageSrc: "/generated/image-a-focused-woman-leader-with-an-open-lapt.webp"
    },
    {
      name: "Daniel Rivera",
      position: "Founder, LogicTree Labs",
      imageSrc: "/generated/image-a-male-tech-founder-wearing-a-casual-bla.webp"
    },
    {
      name: "Ava Morgan",
      position: "Business Strategist, Vertex Advisors",
      imageSrc: "/generated/image-a-female-business-strategist-with-a-glas.webp"
    }
  ]}
/>

<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/stripe.com',
		'https://logo.clearbit.com/dropbox.com',
		'https://logo.clearbit.com/zapier.com',
		'https://logo.clearbit.com/airbnb.com'
	]}
/>

<Summary
	title="AI Chief of Staff for CEOs and executives"
	text="Donna connects to your company tools and instantly delivers a real-time pulse on projects and productivity—no chasing updates or meetings required. SOC-2 compliant with zero data retention."
/>

<Testimonials
	testimonials={[
		{
			name: "Kwame Adisa",
			position: "COO",
			company: "Reformas Capital",
			quote: "Donna cut our meeting load in half. My executive team now gets instant clarity on project status, which means we can act—fast—before minor issues become risks.",
			image: "/generated/image-an-african-male-executive-standing-in-a-.webp"
		},
		{
			name: "Evelyn Foster",
			position: "CFO",
			company: "WaveNorth Logistics",
			quote: "Within 30 days, Donna uncovered two major process bottlenecks that were costing us tens of thousands every quarter. The real ROI is in the time and money we’re saving.",
			image: "/generated/image-a-caucasian-female-cfo-in-a-meeting-room.webp"
		},
		{
			name: "Daisuke Mori",
			position: "Founder & CEO",
			company: "Kairo Labs",
			quote: "My team spends less time compiling updates, and I’m never in the dark. Donna’s daily briefings help me spot blockers before they impact delivery.",
			image: "/generated/image-an-east-asian-male-founder-in-a-collabor.webp"
		}
	]}
/>

<Features
  title="Know exactly what's happening in your company"
  subtitle="Donna is your AI Chief of Staff. Get instant insight into project progress and team productivity—without the meetings and manual updates."
  features={[
    {
      title: "Real-time project tracking",
      description:
        "See the status of every initiative across your company instantly. Donna maps project owners, deadlines, blockers, and dependencies using your team's existing tools."
    },
    {
      title: "40-hour productivity analytics",
      description:
        "Understand how time is really being spent so you can spot inefficiencies, rebalance priorities, and increase output—without micromanaging."
    },
    {
      title: "Frictionless setup",
      description:
        "Securely connect Slack, Asana, Notion, Jira, Google Calendar, and more—no manual input or workflow disruption required."
    },
    {
      title: "Daily executive briefings",
      description:
        "Get a concise summary every morning of what's moving, what's stuck, and where your attention matters most—delivered straight to you."
    },
    {
      title: "Enterprise-grade security",
      description:
        "SOC-2 compliance and a zero data retention policy ensure your company data stays protected at all times."
    },
    {
      title: "Built for decision-makers",
      description:
        "Designed for CEOs and executives who need clarity and speed, Donna scales to any company size and amplifies your impact."
    }
  ]}
/>

<UseCases
  title="Use Cases"
  subtitle="Real-world applications for your business needs"
  useCases={[
    {
      title: "Spot project risks without meetings",
      description: "Get real-time visibility into project status across all teams and tools—minus the syncs and delays.",
      image: "/generated/image-a-busy-executive-in-a-modern-glass-offic.webp",
      link: {
        href: "/use-cases/spot-project-risks",
        label: "Learn more"
      }
    },
    {
      title: "See how time is spent company-wide",
      description: "Understand where your team's time goes each week so you can rebalance and focus on what matters.",
      image: "/generated/image-a-ceo-in-a-conference-room-sitting-at-a-.webp",
      link: {
        href: "/use-cases/time-analytics",
        label: "Learn more"
      }
    },
    {
      title: "Get real-time updates instead of daily standups",
      description: "Donna delivers automated status updates to Slack so your team stays aligned—no meetings required.",
      image: "/generated/image-a-leadership-team-gathered-in-a-spacious.webp",
      link: {
        href: "/use-cases/automated-updates",
        label: "Learn more"
      }
    }
  ]}
/>

<AboutTeaser />
<CallToAction
  title="Cut the noise. Take control with Donna."
  subtitle="Limited pilot for CEOs and executives"
  description="Join a select group for white-glove onboarding, fast setup, and instant visibility—no status meetings or data headaches. Reserve your spot in our exclusive pilot and see real results."
  imageSrc="/generated/image-a-confident-executive-standing-in-a-sunl.webp"
  callsToAction={[
    { href: '/get-started', label: 'Join the pilot', variant: 'primary' },
    { href: '/contact', label: 'Contact sales', variant: 'secondary' }
  ]}
/>
