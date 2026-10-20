<script>

    let { person ={
        fullName: "Phill Connors",
        favouriteSong: "I Got You Babe",
        petsName: "Punxsutawney Phil",
        image: "https://dummyjson.com/icon/emilys/128",
        address: {address: "123 sesame st"}
        } 
    } = $props();


</script>
<section>
    <h2>{person.fullName}</h2>
    <dl>
        <dt>Address:</dt>
        <dd>{person.address.address}</dd>
        <dt>Address:</dt>
        <dd>{person.address.address}</dd>
    </dl>
</section>

<style>
    dl {
        display: grid;
        grid-template-columns: max-content 1fr;
        gap: 0.5rem 1rem;
    }

    dt {
        font-weight: bold;
    }

    dd {
        margin: 0;
    }
</style>