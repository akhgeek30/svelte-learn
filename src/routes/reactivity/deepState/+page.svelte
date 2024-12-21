<script>
    let numbers = $state([1, 2, 3, 4]);

    function addNumbers(){
        numbers.push(numbers.length + 1);
        console.log(numbers);
    }
</script>

<p> {numbers.join(' + ')} = ...</p>
<button onclick={addNumbers}>
    Add Number
</button>
