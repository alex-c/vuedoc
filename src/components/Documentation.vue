<template>
    <div id="vd-container">
        <div class="vd-nav-chapter" v-for="chapter in docsource.chapters">
            <h3>{{chapter.title}}</h3>
            <div v-for="section in chapter.sections">{{section.value}}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'vd-documentation',
    props: ['docsource'],
    data() {
        return({});
    }
}
</script>

<style lang="scss">
#vd-container {
    background-color: blue;
    width: 100%;
    position: relative;
    margin: 0px;
    padding: 0px;
}
</style>
