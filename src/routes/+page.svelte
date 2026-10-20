<script>
    import Card from '$lib/components/Card.svelte';

    let { data } = $props();
    let userList = data.users.users;

    let people = [{
        fullName: "Phill Connors",
        favouriteSong: "I Got You Babe", 
        petsName: "Punxsutawney Phil"
    },
    {
        fullName: "Phill Swift",
        favouriteSong: "the phil swift song", 
        petsName: "phil dog"
    },
    {
        fullName: "jeff the killer",
        favouriteSong: "whels on the bus", 
        petsName: "jeff the killer's cat"
    }
];
</script>

<main>
<!--  -->
    {#each people as person}
        <Card person={person}/>
    {/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>