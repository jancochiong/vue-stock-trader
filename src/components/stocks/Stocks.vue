<template>
    <div>
        <app-stock v-for="stock in stocks" :key="stock.id">{stock}</app-stock>
    </div>
</template>

<script>
    import Stock from './Stock.vue'

    export default {
        data(){
            return{
                stocks: [
                    {id: 1, name: 'BMW', price: 110},
                    {id: 2, name: 'FIRE', price: 11.12},
                    {id: 3, name: 'APHRIA', price: 8},
                    {id: 4, name: 'Canopy', price: 33}
                ]
            }
        },
        components:{
            appStock: Stock
        }
    }
</script>