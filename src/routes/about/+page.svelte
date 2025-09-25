<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Removed StakeholderGrid import as it's not needed
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Mission Precision",
			description: "Every system deployed must meet the exact operational requirements. No compromises on accuracy, reliability, or safety in mission-critical environments."
		},
		{
			title: "Operational Excellence",
			description: "From deployment to decommission, we optimize for seamless integration with existing defense workflows and command structures."
		},
		{
			title: "Transparent Accountability",
			description: "Full audit trails, open-source principles, and human oversight at every decision point. Your data, your rules, your control."
		},
		{
			title: "Democratic Values",
			description: "Built for liberal democracies with constitutional oversight, civil rights protection, and ethical use frameworks at our foundation."
		}
	];
</script>

<SecondaryHero
	title="Autonomy without complexity"
	subtitle="Defense made smarter, not harder"
	imageSrc="/generated/image-a-team-of-diverse-engineers-collaboratin.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Founded by defense engineers who understood the operational gaps in autonomous surveillance. Too many capable teams were limited by complex interfaces and vendor constraints.",
		"We built Ark to solve a specific problem: scaling drone operations without scaling headcount. Every feature serves operational necessity, not engineering novelty.",
		"Our approach is grounded in democratic accountability. Human oversight isn't an afterthought—it's built into the system architecture. Operators maintain full control and decision authority.",
		"Today, defense teams deploy Ark to strengthen border security, enhance situational awareness, and reduce operational burden. The technology serves the mission, not the other way around."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- CTA Section -->
<CallToAction
	title="Step into autonomous operations"
	subtitle="Ready when you are"
	description="Deploy scalable drone surveillance without expanding your team. Experience military-grade autonomy that integrates seamlessly with your existing command structure."
/>
