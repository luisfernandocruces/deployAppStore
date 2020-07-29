<template>
  <div class="home">
    <v-row>
      <h1>Categorias</h1>
    </v-row>
    <v-row>
      <v-col v-for="(item,index) in categorias" :key="index">

        <v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      :src= "item.urlImage"
    >
    </v-img>
    <v-card-title> {{item.nombre}}</v-card-title>

    <v-card-text class="text--primary">
      <div>{{item.descripcion}}</div>
    </v-card-text>

    <v-card-actions>
      <v-btn
        color="orange"
        text
        to='/products'
      >
        Ver productos
      </v-btn>

    </v-card-actions>
  </v-card>


      </v-col>
    </v-row>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data(){
    return{
      categorias:[]
    }
  },
  created(){
    this.getCategorias();
  },
  methods:{
    getCategorias(){
      this.axios.get('http://localhost:1337/categorias').then((response) => {
        console.log(response.data);
        this.categorias = response.data;
      })
    }
  }
}
</script>
