<script>
    import Card from '$lib/components/Card.svelte';
    let person = {
        fullName: "Phill Connors",
        favouriteSong: "I Got You Babe", 
        petsName: "Punxsutawney Phil"
    }
</script>

<main>
<!--  -->
    {#each }
    <Card person={person}/>
    <Card />
    <Card />
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>