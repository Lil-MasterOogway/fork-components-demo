<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";

    let firstName = $state("Web");
    let lastName = $state("One");
    let fullName = $derived(firstName + " " + lastName)

    firstName = "Web2"
    lastName = "apple"
</script>

<p>this is the about page</p>
{#if firstName && lastName}
    <p>Hi, {fullName}</p>
{/if}
