<script>
    import PackageInfo from "$lib/components/PackageInfo.svelte";
    const pkg = {
        name: 'svelte',
        version: '5',
        description: 'blazing fast',
        website: 'https://svelte.dev'
    }
</script>

<PackageInfo {...pkg} />