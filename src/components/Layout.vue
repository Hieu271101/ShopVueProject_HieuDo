<template>
    <div>
          <MainNav></MainNav>
            <slot></slot>
        <VueprojectFooter></VueprojectFooter>
    </div>
</template>

<script>

import MainNav from './MainNav.vue'
import VueprojectFooter from './Footer.vue'

export default {
    name: 'LayoutVue',
    components:{
            MainNav,
            VueprojectFooter
    },
    data() {
        return {
            
        };
    },

   

    methods: {
        
    },
};
</script>

<style  scoped>

</style>