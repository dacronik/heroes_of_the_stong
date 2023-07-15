<template>
    <div>
        <div class="error">
            <h1>Error 404</h1>
            <h1>Page NotFound</h1>
            <router-link to="/"><v-btn color="blue">Regresar</v-btn></router-link>
            <router-view/>
           
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'component-name',
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
    .error{
        width: 100%;
        height: 94vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-image: url("@/assets/img/not_found.gif");
        background-position: center;
    }   
    .error h1{
        font-size: 4rem;
        font-weight: 700;
        color: blue;
    }
</style>