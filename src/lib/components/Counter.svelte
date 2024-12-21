<script lang="ts">
    import { counter } from '$lib/components/shared.svelte';
</script>
<button onclick="{() => counter.count += 1}">clicks: {counter.count}</button>