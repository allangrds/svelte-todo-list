<script>
    import Todo from '../components/Todo.svelte'
    import List from '../components/List.svelte'
    import { tasks } from '../store'

    let tasksList

    tasks.subscribe(value => {
		tasksList = value
    })
    
    function addTask(task) {
		tasks.update(() => [...tasksList, task])
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
        list={tasksList}
    />
</main>