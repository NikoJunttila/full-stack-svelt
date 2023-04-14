<style>
    div{
        display: grid;
        grid-template-columns:  2rem 1fr 2rem;
        grid-gap: 0.5rem;
        align-items: center;
        margin-left: 0.5rem;
        margin-right: 0.1rem;
        padding: 0.5rem;
        background-color: antiquewhite;
        border-radius: 10px;
        filter:drop-shadow(2px 4px 6px rgba(0,0,0,0.2));
        transition: filter 0.2s;
    }
    button{
        width: 2em;
        height: 2em;
        border: none;
        background-color: transparent;
        background-position: 50% 50%;
        background-repeat: no-repeat;
        cursor: pointer;
    
    }
    input{
        border-radius: 10px;
        flex: 1;
    }
    .toggle{
        border: 1px solid rgba(0,0,0,0.2);
        border-radius: 50%;
        box-sizing: border-box;
        background-size: 1em auto;
        content: "";
    }
    .save{
        opacity: 0;
        color: green;
    }
    input:focus + .save, .save:focus {
        transition: opacity 0.3s;
        opacity: 1
    }
    .delete:hover,.delete:focus{
        opacity: 0.5;
    }
   
    
</style>

<div>
	<form action="" method="">
		<input type="hidden" name="done" value="" />
		<button class="toggle" aria-label="mark done/not"></button>
	</form>

	<form action="" method="">
		<input type="text" name="text" value="" />
		<button class="save" aria-label="text">save</button>
	</form>

	<form action="" method="">
		<button class="delete" aria-label="delete">delete</button>
	</form>
</div>
