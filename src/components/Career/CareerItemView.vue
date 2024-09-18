<template>
    <div class="career-content">
        <div class="career-title">
            <h2>{{ companyName }}</h2>
        </div>
        <div class="career-item">
            <p class="l-lg-gray">{{ history }}</p>
            <br>
            <h3>{{ projectName }}</h3>
            <h4>{{ projectConcept }}</h4>
            <p class="l-lg-gray">{{ projectStack }}</p>
            <br>
            <h3>担当業務</h3>
            <ul class="ml-16">
                <li v-for="item in whatIachieved" :key="item">
                    {{ item }}
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            companyName: String,
            history: String,
            projectName: String,
            projectStack: String,
            projectConcept: String,
            whatIachieved: Array
        }
    }
</script>

<style scoped>
    .career-title {
        display: flex;
    }

    .career-title::before {
        content: '';
        width: 36px;
        height: 36px;
        border-radius: var(--corner-radius-half);
        margin: var(--zero) var(--margin-default);
        background-color: var(--accent-color);
        border: var(--border-thin) dashed black;
        padding:  var(--margin-small);
        box-sizing: border-box;
    }

    .career-content {
        margin: var(--margin-default);
    }

    .career-item {
        margin: var(--zero) var(--margin-big);
        padding: var(--margin-default);
        border-left: var(--border-double-thin) dashed var(--accent-color);
    }
</style>