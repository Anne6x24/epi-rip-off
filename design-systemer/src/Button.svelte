<script>
    export let type;
    export let mode;
</script>

<button class:inversed={mode==="inversed"} class={type}><slot/></button>

<style>

    button {
        color:var(--primary-font-color);
        border-radius: 10px 10px 10px 10px;
        border: none;
        background: grey;
        padding: 0.8rem;
        font-family: "futura";
        margin-block: 1rem;
    }

    button:hover{
        background: hsl(0, 0%, 80%);
        color:black;
    }

    .primary {
        background: var(--primary-color);
    }

   
    .secondary {
        background: var(--secondary-color);
    }

    .accent {
        background: var(--accent-color);
    }

    .ghost {
        color:var(--ghost-font-color);
        background: none;
    }

    .link{
        background: none;
    }

    .link:hover {
        text-decoration: underline;
        color: var(--primary-color);
    }


  


</style>