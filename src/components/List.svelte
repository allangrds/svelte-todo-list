<script>
    export let list
</script>

<ul>
    {#each list as item}
        <li>{ item }</li>
    {/each}
</ul>