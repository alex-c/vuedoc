<template>
    <div id="vd-navigation">
        <div class="vd-nav-chapter" v-for="chapter in docsource.chapters">{{chapter.title}}</div>
    </div>
</template>

<script>
export default {
    name: 'vd-navigation',
    props: ['docsource'],
    data() {
        return({});
    }
}
</script>

<style lang="scss">
#vd-navigation {
    position: fixed;
    top: 0px;
    left: 0px;
    bottom: 0px;
    width: 200px;
    background-color: red;
}
</style>
