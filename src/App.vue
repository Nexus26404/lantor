<template>
    <tabbar :title="msg"></tabbar>
</template>

<script>
    import Tabbar from './components/Tabbar.vue'

    export default {
        name:'',
        components: {
            Tabbar
        },
        data(){
            return {
                msg: 'Hao a you'
            }
        }
    }
</script>

<style scoped>
</style>