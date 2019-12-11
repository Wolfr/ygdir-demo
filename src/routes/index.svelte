<script>
    import Hero from '../components/Hero.svelte';
    import InstallInstructions from '../components/InstallInstructions.svelte';
</script>

<svelte:head>
    <title>Ygdir - Documentation</title>
</svelte:head>

<div class="c-container">

    <main class="c-content">

        <Hero />

        <InstallInstructions />

    </main>

    <article>

        <h3>Based on proven CSS methodologies</h3>

        <p>Through a combination of BEM and ITCSS, with clear rules regarding namespacing, we provide a scalable base to build from.</p>

        <h3>Start from scratch (or don’t)</h3>

        <p>Base Ygdir is just a reset and a series of conventions. You can choose to plug in pre-built components, but unlike other frameworks, we don’t ship 300kb worth of default CSS. If your project only has a form and a few buttons, only include the needed components.</p>

        <h3>Javascript framework independent</h3>

        <p>Use whichever Javascript framework you want. Ygdir is independent from Javascript frameworks. The reality of web development is that different things are written with different frameworks. Why would you tie your CSS to a single framework?</p>

        <h3>Convention-first</h3>

        <p>In Ygdir, components follow a strict convention. This leads to predictable code that can be maintained over time. For example, it is easy to tell whether a component is dead code.</p>

        <h3>Not utility-first</h3>

        <p>Utility-first CSS leads to horrible many-to-many problems. It looks like a good idea at first, until you have to maintain it. Utility-first frameworks promote messy code.</p>
        <p>We don’t have a problem with prototyping and quickly trying things, but using too many utilities leads to maintenance problems.</p>

    </article>

</div>
