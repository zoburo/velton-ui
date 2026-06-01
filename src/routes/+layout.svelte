<script lang="ts">
	import { Provider } from '$lib';
	import './layout.css';

	const { children } = $props();
</script>

<Provider>
	{@render children()}
</Provider>
