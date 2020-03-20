<template>
    <v-container fluid>
        <v-slide-y-transition mode="out-in">
            <v-row>
                <v-col>
                    <h1>Counter</h1>
                    <p>This is a simple example of a Vue.js component integrated with Vuex</p>
                    <Counter />
                </v-col>
            </v-row>
        </v-slide-y-transition>
    </v-container>
</template>


<script lang="ts">
    import { Component, Vue } from 'vue-property-decorator';
    import Herculead from '@/components/Herculead.vue';

    @Component({
        components: { Herculead },
    })
    export default class HerculeadView extends Vue { }
</script>


