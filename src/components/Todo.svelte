<script>
    import List from './List.svelte'

    let task = ''
    let tasks = []

    function addTask () {
        tasks = [
            ...tasks,
            task,
        ]
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

    <List
        list={tasks}
    />
</form>