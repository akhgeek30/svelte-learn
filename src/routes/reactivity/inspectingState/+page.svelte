<script>
    let numbers = $state([1, 2, 3, 4]);
    let total = $derived(numbers.reduce((t, n) => t + n, 0));
    function addNumbers(){
        numbers.push(numbers.length + 1);
        console.log($state.snapshot(numbers)); //Make the reactive numbers as a non-reactive for inspection
    }

    $inspect(numbers).with(console.trace);
</script>

<p> {numbers.join(' + ')} = {total} </p>

<button onclick={addNumbers}>
    Add Number
</button>
