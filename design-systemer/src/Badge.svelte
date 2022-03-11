<script>
    export let type;
</script>


<button class={type}><slot/></button>



<style>
    button {
        color: white;
        background: grey;
        border-radius: 25px 25px 25px 25px;
        border: none;
        font-family: "futura";
        font-weight: 400;
        padding: 0.1rem;
        margin-block: 1rem ;
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
        color: var(--ghost-font-color);
        background: none;
    }

    .ghost_border {
        border: black solid 1px;
        color: var(--ghost-font-color);
        background: none;
    }

</style>