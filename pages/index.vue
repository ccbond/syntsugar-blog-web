<script>
import Vue from 'vue'
import { BIcon } from 'bootstrap-vue'
import HeaderCommon from '../components/layout/headerCommon.vue'


Vue.component('b-icon', BIcon)

export default {
    data() {
        return {
            count: 0
        };
    },
    components: { HeaderCommon }
}
</script>

<template>
<div>
<HeaderCommon />

</div>

<!-- <HeaderCommon /> -->
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>