<script lang="ts">
	import Todo from '../lib/todo-item.svelte';
	let newTodo: string = '';
	const title: string = 'todo';
</script>
<style>
h1{
    font-size: 2rem;
    text-align: center;
    padding: 1rem 0;
}
section{
    max-width: 40rem;
    border: 2px solid black;
    display: flex;
    flex-direction: column;
    align-items: center;  
    padding-bottom: 10px; 
}
section :global(input){
border: 1px solid transparent;
background-color: transparent;
color: white;
border-radius: 20px;
}
section :global(input:focus-visible){
box-shadow: inset 1px 1px 6px black;
border: 1px solid red !important;
outline: none; 
}
input{
    text-align: center;
    height: 2rem;
    margin-bottom: 0.5rem;
}

</style>

<svelte:head>
	<title>{title}</title>
</svelte:head>
<section>
<h1>{title}</h1>
<form action="" method="">
	<input type="text" name="todo" aria-label="Add a todo" placeholder="+ tap to add a todo" />
</form>
<Todo />
</section>
