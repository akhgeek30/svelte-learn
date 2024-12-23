<script>
    let numbers = $state([1, 2, 3, 4]);
    let total = $derived(numbers.reduce((t, n) => t + n, 0));
    function addNumbers(){
        numbers.push(numbers.length + 1);
    }
</script>

<p> {numbers.join(' + ')} = {total} </p>

<button onclick={addNumbers}>
    Add Number
</button>
