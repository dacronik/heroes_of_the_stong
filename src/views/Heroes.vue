<template>
    <div class="heroes">
        <v-container>
            <div>
                <h1>Héroes</h1>
                <div class="icons py-10">
                    <v-icon class="icon">mdi-sword</v-icon>
                    <v-icon class="icon">mdi-shield</v-icon>
                    <v-icon class="icon">mdi-crosshairs</v-icon>
                    <v-icon class="icon">mdi-heart-plus</v-icon>
                    <v-icon class="icon">mdi-dna</v-icon>
                </div>
            </div>
            <v-row>
                <v-col cols="12" md="10">
                    <v-table theme="dark" class="table">
                        <template v-slot:default>
                            <thead>
                                <tr>
                                    <th class="text-left">
                                    Héroe
                                    </th>
                                    <th class="text-left">
                                    Nombre
                                    </th>
                                    <th class="text-left">
                                    Función
                                    </th>
                                    <th class="text-left">
                                    Titulo
                                    </th>
                                    <th class="text-left">
                                    Ataque
                                    </th>
                                </tr>
                            </thead>
                            <tbody>
                            <tr
                                    v-for="(heroe,index) in heroes"
                                    :key="index">
                                    <td><img :src="heroe.imagen" width="200" height="200" alt="" srcset=""></td>
                                    <td>{{ heroe.nombre }}</td>
                                    <td>{{ heroe.funcion }}</td>
                                    <td>{{ heroe.titulo }}</td>
                                    <td>{{ heroe.ataque }}</td>
                                </tr>
                            </tbody>
                        </template>
                    </v-table>
                </v-col>
            </v-row>

        </v-container>

    </div>
</template>

<script>
import { mapState } from 'vuex';
export default {
    name: 'heroes-view',
    // props: {},
    data: function(){
        return {}
    },
    computed: {
        ...mapState(['heroes'])
    },

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
    .heroes{
        background: url('../assets/img/fondo3.jpg');
        height: 100%;
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        color: aliceblue;
    }
    .table{
        max-height: 70vh;
        overflow: auto;
    }
    .icons{
        padding: 0 10px;
        font-size: 25px;
        color: aliceblue;
    }
</style>