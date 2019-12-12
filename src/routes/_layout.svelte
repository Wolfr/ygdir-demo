<script>
    export let segment;

    import Header from '../components/Header.svelte';
    import Footer from '../components/Footer.svelte';
</script>

<style lang="scss" global>
     @import "./style/app.scss";
</style>

<Header segment={segment} />

<slot></slot>

<Footer />