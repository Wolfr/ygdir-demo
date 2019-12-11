<style>
    article {
        columns: 40rem;
        column-gap: 4rem;
        margin-top: 4rem;
        padding-top: 4rem;
        margin-bottom: 8rem;
        border-top: 1px solid #CCC;
    }
    article section {
        -webkit-column-break-inside: avoid;
        -moz-column-break-inside: avoid;
        column-break-inside: avoid;
    }
    article section h3 {
        margin-top: 0;
    }
</style>

<article>
    <section>
        <h3>Based on proven CSS methodologies</h3>
        <p>Through a combination of BEM and ITCSS, with clear rules regarding namespacing, we provide a scalable base to build from.</p>
    </section>
    <section>
        <h3>Start from scratch (or don’t)</h3>
        <p>Base Ygdir is just a reset and a series of conventions. You can choose to plug in pre-built components, but unlike other frameworks, we don’t ship 300kb worth of default CSS. If your project only has a form and a few buttons, only include the needed components.</p>
    </section>
    <section>
        <h3>Javascript framework independent</h3>
        <p>Use whichever Javascript framework you want. Ygdir is independent from Javascript frameworks. The reality of web development is that different things are written with different frameworks. Why would you tie your CSS to a single framework?</p>
    </section>
    <section>
        <h3>Convention-first</h3>
        <p>In Ygdir, components follow a strict convention. This leads to predictable code that can be maintained over time. For example, it is easy to tell whether a component is dead code.</p>
    </section>
    <section>
        <h3>Not utility-first</h3>
        <p>Utility-first CSS leads to horrible many-to-many problems. It looks like a good idea at first, until you have to maintain it. Utility-first frameworks promote messy code.</p>
        <p>We don’t have a problem with prototyping and quickly trying things, but using too many utilities leads to maintenance problems.</p>
    </section>
</article>
