<script>
    import Card from '$lib/components/Card.svelte';

    let { data } = $props();
    let userList = data.users.users;


</script>

<main>
<!--  -->
    {#each userList as person}
        <Card person={person}/>
    {/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>