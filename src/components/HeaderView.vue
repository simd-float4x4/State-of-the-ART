<template>
    <header class="header">
        <div class="container">
            <div class="inner">
                STATE OF THE ART
            </div>
        </div>
    </header>
</template>

<style scoped>
    .header {
        background-color: var(--black-color);
        width: var(--full-width);
        height: var(--header-height);
        z-index: 99999;
        position: fixed;
    }

    .container, .inner {
        width: var(--full-width);
        height: var(--header-height);
        border-bottom: var(--border-double-thin) solid var(--accent-color);
        display: flex;
        align-items: center;
        justify-content: center;
        margin: auto;
        max-width: var(--full-width);
        box-shadow: var(--zero) var(--border-ultra-thin) var(--border-double-medium) var(--border-ultra-thin) var(--black-color);
    }
</style>