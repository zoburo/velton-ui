<script lang="ts">
	let { children } = $props();
</script>

<svelte:head>
	<script>
		if (
			localStorage.theme === 'dark' ||
			(!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)
		) {
			document.documentElement.classList.add('data-theme', 'dark');
			// @ts-ignore
			window.theme = 'dark';
		} else {
			document.documentElement.classList.add('data-theme', 'light');
			// @ts-ignore
			window.theme = 'light';
		}
	</script>
</svelte:head>

{@render children()}
