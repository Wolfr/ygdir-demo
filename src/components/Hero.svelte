<script>
    import typewriter from 'svelte-typewriter/typewriter'
</script>

<style>
    p {
        font-size: 3.2rem;
        text-align: center;
        margin: 4.8rem auto;
        font-weight: 600;
        color: #000;
        max-width: 80%;
        line-height: 110%;
    }
    @media (min-width: 80rem) {
        p {
            min-height: 7rem;
        }
    }
</style>

<p use:typewriter>Ygdir is a new CSS framework that aims to make CSS less painful.</p>
