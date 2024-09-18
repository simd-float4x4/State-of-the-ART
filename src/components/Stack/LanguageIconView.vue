<template>
    <div class="cell">
        <div class="stack_name">
            <p :style="{ 
                backgroundImage: `${color}`, 
                backgroundSize: 'cover',
                backgroundPosition: 'center',
                backgroundBlendMode: 'overlay'
            }">
                {{ stackName }}
            </p>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            stackName: String,
            color: String
        }
    }
</script>

<style scoped>
    .cell {
        position: relative;
        width: 270px;
        height: 180px;
        margin: var(--margin-default);
        flex-shrink: 0;
        box-shadow: var(--zero) var(--border-ultra-thin) var(--border-double-medium) var(--border-ultra-thin) var(--black-color);
        border-radius: var(--corner-radius-fixed);
    }

    .stack_name p {
        font-size: 36px;
        border-radius: var(--corner-radius-fixed);
        position: absolute;
        top: var(--zero);
        left: var(--zero);
        right: var(--zero);
        bottom: var(--zero);
        padding: var(--margin-default);
        font-weight: bold;
    }
</style>