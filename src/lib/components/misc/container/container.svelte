<script lang="ts">
	import { cn } from '$lib/utils';
	import type { HTMLAttributes } from 'svelte/elements';

	let { children, class: className, ...restProps }: HTMLAttributes<HTMLDivElement> = $props();
</script>

<div class={cn('mx-auto w-full max-w-5xl px-6', className)} {...restProps}>
	{@render children?.()}
</div>
