<template>
    <h1 class="section-title">STACK</h1>
    <div class="scroll-area">
        <LanguageIcon stackName="UIKit" :color="UIKitStyle"/>
        <LanguageIcon stackName="SwiftUI" :color="SwiftUIStyle"></LanguageIcon>
        <LanguageIcon stackName="Flutter" :color="FlutterStyle"></LanguageIcon>
        <LanguageIcon stackName="Laravel" :color="LaravelStyle"></LanguageIcon>
        <LanguageIcon stackName="Ruby on Rails" :color="RubyStyle"></LanguageIcon>
        <LanguageIcon stackName="Vue.js" :color="VueJSStyle"></LanguageIcon>
        <LanguageIcon stackName="Three.js" :color="ThreeJSStyle"></LanguageIcon>
        <LanguageIcon stackName="Blender" :color="BlenderStyle"></LanguageIcon>
    </div>
</template>

<script>
import LanguageIcon from "./LanguageIconView.vue"

export default {
    components: {
        LanguageIcon
    },
    computed: {
        UIKitStyle() {
            const imageUrl = require('../../assets/images/images.001.png');
            return `linear-gradient(0deg, rgba(194, 57, 248, 1), rgba(48, 53, 97, 1)), url(${imageUrl})`;
        },
        SwiftUIStyle() {
            const imageUrl = require('../../assets/images/images.002.png');
            return `linear-gradient(90deg, rgba(65, 164, 253, 1), rgba(14, 244, 255, 1)), url(${imageUrl})`;
        },
        FlutterStyle() {
            const imageUrl = require('../../assets/images/images.006.png');
            return `linear-gradient(90deg, rgba(212, 248, 57, 1), rgba(97, 64, 48, 1)), url(${imageUrl})`;
        },
        LaravelStyle() {
            const imageUrl = require('../../assets/images/images.003.png');
            return `linear-gradient(90deg, rgba(247, 93, 139, 1), rgba(254, 220, 64, 1)), url(${imageUrl})`;
        },
        RubyStyle() {
            const imageUrl = require('../../assets/images/images.004.png');
            return `linear-gradient(120deg, rgba(255, 84, 54, 0.8), rgba(255, 255, 255, 0)), url(${imageUrl})`;
        },
        VueJSStyle() {
            const imageUrl = require('../../assets/images/images.005.png');
            return `linear-gradient(0deg, rgba(89, 248, 57, 1), rgba(97, 94, 48, 1)), url(${imageUrl})`;
        },
        ThreeJSStyle() {
            const imageUrl = require('../../assets/images/images.007.png');
            return `linear-gradient(270deg, rgba(85, 85, 85, 1), rgba(0, 0, 0, 1)), url(${imageUrl})`;
        },
        BlenderStyle() {
            const imageUrl = require('../../assets/images/images.008.png');
            return `linear-gradient(90deg, rgba(248, 134, 57, 1), rgba(97, 48, 48, 1)), url(${imageUrl})`;
        },
    }
}
</script>

<style scoped>
    .scroll-area {
        width: var(--full-width);
        display: flex;
        overflow-x: scroll;
    }
</style>