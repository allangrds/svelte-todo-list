<script>
    import Todo from '../components/Todo.svelte'
    import List from '../components/List.svelte'

    let tasks = []

    function addTask (task) {
        tasks = [
            ...tasks,
            task,
        ]
        console.log(`tasks -`, tasks)
    }
</script>

<style>
    .container {
        width: 380px;
        margin: 0 auto;
    }
</style>

<main class="container">
    <Todo
        onSave={addTask}
    />
    <List
        list={tasks}
    />
</main>