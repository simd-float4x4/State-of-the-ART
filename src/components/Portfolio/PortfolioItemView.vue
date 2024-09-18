<template>
    <div class="rights_cell" @click="moveExternalURL">
        {{ title }}
        <i class="fa-solid fa-chevron-right"></i>
    </div>
</template>

<script>
    export default {
        props: {
            title: String,
            URL: String
        },
        methods: {
            moveExternalURL() {
                window.location.href = this.URL;
            }
        }
    }
</script>

<style scoped>
    .rights_cell {
        margin: var(--margin-big);
        padding: var(--margin-big);
        border-top: var(--border-thin) dashed red;
        display: flex;
        vertical-align: middle;
    }

    .rights_cell i {
        padding-left: var(--margin-big);
        padding-top: var(--margin-extra-small);
    }
</style>