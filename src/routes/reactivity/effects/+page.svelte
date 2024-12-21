<script>
    let elapsed = $state(0);
    let interval = $state(1000);

    $effect(() => {
        const id = setInterval(() => {
            elapsed += 1;
        }, interval);

        return () => {
            clearInterval(id);
        }
    });
</script>
<p> elapsed : {elapsed}</p>


<button onclick={() => interval /= 2} > Speed Up </button>

<button onclick={() => interval *= 2}> Speed down </button>
