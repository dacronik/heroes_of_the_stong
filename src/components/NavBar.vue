<template>
    <v-app-bar :elevation="2" color="blue-darken-3">
        <v-row justify="center">
            <v-btn 
            color="light" 
            variant="tonal"
            dark
            to="/"
            prepend-icon="mdi-home" 
            type="button">
            Home
            </v-btn>
        </v-row>
    </v-app-bar>
</template>

<script>
export default {
    name: 'nav-bar-comp',
    // props: {},
    data: function(){
        return {}
    },
    // computed: {},
    //methods: {}
    // watch: {},
    // components: {},
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
}
</script>

<style scoped>
    
</style>