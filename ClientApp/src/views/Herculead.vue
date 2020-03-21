<template>
    <v-container fluid>
        <v-slide-y-transition mode="out-in">
            <v-row>
                <v-col>
                    
                    Leads
                </v-col>
                <v-col>
                    test
                </v-col
                    <v-data-table 
                        :headers="headers"
                        :items="leads">
                    </v-data-table>
                
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
export default class HerculeadView extends Vue {
    public data() {
        return {
            headers: [
                {
                    text: 'Full Name',
                    align: 'start',
                    sortable: false,
                    value: 'fullName',
                },
                { text: 'Company Name', value: 'companyName' },
                { text: 'City', value: 'city' },
                { text: 'State', value: 'state' },
                { text: 'Address', value: 'address' },
                { text: 'Business Phone', value: 'businessPhone' },
                { text: 'E-mail', value: 'email' },
                { text: 'Update Date', value: 'updateDate' }

            ],
            leads: [
                {
                    fullName: 'Bob Joe',
                    companyName: 'Ambit',
                    city: 'Fort Worth',
                    state: 'TX',
                    address: '3232 Lodosa',
                    businessPhone: '(817) 370-9068',
                    email: 'nigeriaPrince@aol.com',
                    updateDate: '03-19-2020',
                },
            ],
        };
    }
}
</script>


