<script lang="ts">
	import { Container } from '$lib';

	let { children } = $props();
</script>

<Container
	class="prose max-w-3xl py-11 prose-zinc dark:prose-invert prose-headings:font-semibold prose-h1:text-3xl"
>
	{@render children()}
</Container>
