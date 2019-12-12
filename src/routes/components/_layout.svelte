<svelte:head>
    <title>Ygdir - Components</title>
</svelte:head>

<script>
    export let segment;
</script>

<style>
    @media (min-width: 800px) {
        .c-layout-components {
            display: flex;
            width: 100%;
        }

        .c-layout-components__sidebar {
            padding: 3.2rem;
            border-right: 1px solid #DDD;
            min-width: 22rem;
        }
    }

    .c-layout-components__content {
        padding: 3.2rem;
        flex: 1 0 auto;
    }

</style>

<div class="c-layout-components">
    <div class="c-layout-components__sidebar">
        <ul class="c-nav-list">
            <li><a href="/components/buttons" class:selected={segment === "buttons"}>Buttons</a></li>
            <li><a href="/components/block-list" class:selected={segment === "block-list"}>Block list</a></li>
            <li><a href="/components/container" class:selected={segment === "container"}>Container</a></li>
            <li><a href="/components/nav-list" class:selected={segment === "nav-list"}>Nav list</a></li>
            <li><a href="/components/modal" class:selected={segment === "modal"}>Modal</a></li>
            <li><a href="/components/toolbar" class:selected={segment === "toolbar"}>Toolbar</a></li>
            <li><a href="/components/tooltip" class:selected={segment === "tooltip"}>Tooltip</a></li>
        </ul>
    </div>
    <div class="c-layout-components__content">
        <div class="c-container c-container--small">

            <slot></slot>

        </div>
    </div>
</div>
