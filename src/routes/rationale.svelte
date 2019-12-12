<svelte:head>
    <title>Ygdir - Rationale</title>
</svelte:head>

<style>

    header {
        margin: 4.8rem 0;
    }

    header p {
        color: #999;
    }

</style>

<div class="c-container c-container--small">

    <article>

        <header>
            <h2>Rationale: A baked in CSS strategy</h2>
            <p>Written by Johan Ronsse</p>
        </header>

        <div class="c-content">
            <p>We state that Ygdir is <strong>convention first</strong>. But what does this mean?</p>

            <p>CSS frameworks are a weird one. You typically want to have the least amount of CSS possible. At the same time, if there are no rules, codebases can get super wieldy and unmaintainable.</p>

            <p>Various attempts have been made to “fix” the problems with CSS, most recently by putting CSS in JS (ugh). The problem here is that re-implementations of CSS do away with what makes CSS powerful, which is the cascade.</p>

            <p>The most interesting method of dealing with CSS is to compile CSS at the component level (like in Svelte). While interesting this ties the code to a specific framework, which is usually not what you want in a complex application using various technologies</p>

            <p>My personal conclusion from lots of projects is that there is still room for a good framework that is independent from the Javascript framework.</p>

            <p>At the same time, many projects do not need a heavy-handed framework. I have to sigh deeply when I see 300kb of code loaded for a tiny website. So I wouldn't want to ship a 300kb framework and put it out there without giving some guidance on how to use it.</p>

            <p>The way to fix CSS is to write proper CSS. But proper CSS, what does that even mean? It means writing CSS with conventions that are rigid enough to support working together.</p>

            <p>This is why Ygdir is both a framework and a proposal for a working methodology.</p>

            <p>The conventions in Ygdir won't be a new story to seasoned CSS'ers:</p>

            <ul>
                <li>Use whichever spaces/tabs convention is defined in <code>.editorconfig</code></li>
                <li>BEM namespacing
                    <ul>
                        <li>BEM as defined by Yandex and further specified by Harry Roberts</li>
                        <li>Important
                        <ul>
                            <li>do not make double underscores for grandchildren</li>
                            <li>do not attempt to recreate HTML structures in CSS; the HTML structure can be nested whereas the CSS structure will be flat</li>
                            <li>If necessary to document the component, do it in a design system (like Storybook), don't document in the file</li></ul>
                        </li>
                    </ul>
                </li>
                <li>ITCSS for the order of CSS
                    <ul>
                        <li>Reset at the top (as minimal as possible)</li>
                        <li>Global variables</li>
                        <li><code>_e-base.scss</code> file that styles <code>html</code>, <code>body</code></li>
                        <li><code>c-</code> namespace for components</li>
                        <li><code>u-</code>namespace for utilities</li>
                        <li>Avoid semantic discussions
                        <ul>
                            <li>You can have your own semantic discussions within your own team, but Ygdir specifically avoids the following discussions
                            <ul>
                                <li>What is the difference between a component and an object?
                                <ul>
                                    <li>In Ygdir there is difference between objects and components</li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                </ul>
            </li>
            </ul>
                <li>Avoid any CSS in the main SCSS file. Use <code>_trash.scss</code> for whatever you are ashamed of</li>
                <li>Avoid mixins and SCSS language features that make SCSS behave like a programming language (like maps, loops and if/else statements). These language features have their uses in complex CSS demos but in general the usage of these language features leads to convoluted code.</li>
                <li>Avoid nested code, almost everything should have a CSS specificity of 10 (class selector)</li>
                <li>Make sure selectors are searchable by their full string (e.g. .c-component__child should return all the CSS lines where that component is used)</li>
                <li>Set variables on the component level</li>
                <li>Override with global variables, but make sure the component's SCSS compiles without the global variables active</li>
            </ul>
        </div>
    </article>

</div>
