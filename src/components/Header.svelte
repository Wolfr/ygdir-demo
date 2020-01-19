<script>
    export let segment;
</script>
<style>

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        border-bottom: 1px solid #DDD;
        padding: 2.4rem;
    }

    h1 a {
        display: block;
        color: #000;
        text-decoration: none;
    }

    nav a {
        margin: 0 0.4rem 0 0;
        color: #000;
        text-decoration: none;
        display: inline-block;
        padding: 0.8rem 1.2rem;
        border-radius: 0.3rem;
    }

    nav a:hover,
    nav a:focus {
        background: #EEE;
    }

    nav a.selected {
        background: #DDD;
    }

    nav img {
        position: relative;
        top: 0.6rem;
    }

</style>

<header>
    <h1>
        <a href="/">Jungle</a>
    </h1>
    <nav>
        <a href="/" class:selected={!segment}>Home</a>
        <a href="/components" class:selected={segment === "components"}>Components</a>
        <a href="https://github.com/mono-company/ygdir">
            <img src="/github-black.svg" alt="">
            Github
        </a>
    </nav>
</header>
