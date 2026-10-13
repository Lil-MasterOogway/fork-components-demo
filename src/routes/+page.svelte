<script>
    import Card from '$lib/components/Card.svelte';
    let people = [
        {
        fullName: "Phill Connors",
        favouriteSong: "I Got You Babe",
        petsName: "Punxsutawney Phil"
    },
        {
        fullName: "Peter Venkman",
        favouriteSong: "In The Name Of Love",
        petsName: "Jason"
    },
        {
        fullName: "Mr Boss",
        favouriteSong: "Doo Doo",
        petsName: "Steve Minecraft"
    },
    ];
</script>

<main>
<!-- TODO make this a loop -->
 {#each people as person}
    <Card person={person} />
 {/each}
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
    }
</style>