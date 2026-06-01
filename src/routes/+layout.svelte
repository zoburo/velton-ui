<script lang="ts">
	import { Provider } from '$lib';
	import '$lib/styles.css';

	const { children } = $props();
</script>

<Provider>
	{@render children()}
</Provider>
