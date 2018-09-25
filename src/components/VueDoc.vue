<template>
    <div id="vuedoc">
        <navigation :docsource="docsource"></navigation>
        <documentation :docsource="docsource"></documentation>
    </div>
</template>

<script>
import Navigation from './Navigation.vue';
import Documentation from './Documentation.vue';

import docsource from '../../documentation_src/cobalt-specification.json';

export default {
    name: 'vuedoc',
    components: {Navigation, Documentation},
    data() {
        return({
            docsource: docsource
        });
    }
}
</script>

<style>
body {
    margin: 0px;
    padding: 0px;
}
#vuedoc {
    margin-left: 200px;
    width: auto;
    overflow: auto;
}
</style>
