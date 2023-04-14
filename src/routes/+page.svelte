<script lang="ts">
    import Todo from "../lib/todo-item.svelte"
let newTodo : string = ""
const title : string = "todo"
</script>
<svelte:head>
    <title>{title}</title>
</svelte:head>
<h1>{title}</h1>
<form action="" method="">
    <input  type="text" name="todo" aria-label="Add a todo" placeholder="+ tap to add a todo">
</form>
<Todo />
