<script>
    let counter = $state(0);

    function increment(){
        counter++;
    }
</script>


<button onclick="{increment}">
    Clicked {counter} 
    {counter === 1 ? 'time' : 'times'}
</button>