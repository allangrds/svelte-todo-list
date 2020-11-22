<script>
    export let onSave
    let task = ''

    function addTask () {
        onSave(task)
        task = ''
    }
</script>

<form>
    <input
        type="text"
        bind:value={task}
    />
    <button type="button" on:click={addTask}>
        Criar
    </button>
</form>