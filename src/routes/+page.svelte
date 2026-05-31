<script lang="ts">
	import { Button, Container } from '$lib';
</script>

<svelte:head>
	<title>Velton UI - Modern component library for Svelte</title>
</svelte:head>

<Container class="max-w-3xl py-24 text-center">
	<h1 class="text-4xl leading-snug font-semibold">Modern component library for Svelte</h1>
	<p class="mx-auto mt-2 w-5/6 text-lg leading-relaxed text-muted-foreground">
		Now you can focus on building great things and turning ideas into reality without ever worrying
		about the UI again.
	</p>
	<div class="mt-7 flex justify-center gap-2.5">
		<Button href="/getting-started/" size="lg">Get started</Button>
		<Button size="lg" variant="outline">Browse components</Button>
	</div>
</Container>
