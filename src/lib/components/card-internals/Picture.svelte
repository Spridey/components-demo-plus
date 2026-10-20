<script>
    import billm from '$lib/assets/images/groundhog-day.webp';
    let { person ={
        fullName: "Phill Connors",
        favouriteSong: "I Got You Babe",
        petsName: "Punxsutawney Phil",
        image: "https://dummyjson.com/icon/emilys/128",
        address: {address: "123 sesame st"}
        } 
    } = $props();
</script>

<img src="{person.image}" alt="Phil">

<style>
    img {
            width: 20px;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: center;
            border-radius: 30px;
            corner-shape: squircle;
        }
</style>