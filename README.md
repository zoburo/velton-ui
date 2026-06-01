# Velton UI

Modern component library for Svelte.

## Getting started

This library requires an existing [SvelteKit](https://svelte.dev/docs/kit/introduction) project with [Tailwind CSS](https://tailwindcss.com/) configured.
If you haven't set these up yet, follow their official documentation first.

To install the library, run:

```bash
pnpm add -D velton-ui
```

Update `src/routes/layout.css` file:

```css
@import 'tailwindcss';
@import 'velton-ui/styles.css';
```

Update `src/routes/+layout.svelte` file:

```svelte
<script lang="ts">
	import { Provider } from 'velton-ui';
	import './layout.css';

	const { children } = $props();
</script>

<Provider>
	{@render children()}
</Provider>
```

That's it! You're now ready to build with Velton UI.
