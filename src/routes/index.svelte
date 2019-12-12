<script>
    import Hero from '../components/Hero.svelte';
    import InstallInstructions from '../components/InstallInstructions.svelte';
    import Usps from '../components/Usps.svelte';
</script>

<svelte:head>
    <title>Ygdir - Documentation</title>
</svelte:head>

<div class="c-container">

    <main>
        <Hero />
        <InstallInstructions />
    </main>

    <Usps />

</div>
