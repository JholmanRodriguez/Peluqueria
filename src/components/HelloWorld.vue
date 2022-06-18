<template>
    <v-container-fluid class="">
      <v-row>
        <v-col>
          <h1 class="mt-4 text-center title"> Sala De imagen D' mary</h1>
        </v-col>
        <v-col>
          
        </v-col>
        <v-col>
          
        </v-col>
        <v-col>
          <button>
          <img class="mt-5" src="https://cdn-icons-png.flaticon.com/512/3144/3144456.png" alt="" id="i" @mouseover="showAlert()" >
          </button>
        </v-col>
      </v-row>

    <v-row id="i2">
      <v-col>
      </v-col>
      <v-col>
        <br><br><br>
        <h1 class="white--text">peluqueria D' Mary</h1>
        <p class="white--text"> ¿Qué te quieres hacer Hoy?</p>
        <v-text-field label="¿Qué te quieres hacer Hoy?" solo dende></v-text-field>
      </v-col>
      <v-col>
      </v-col>
      <v-col>
      </v-col>
    </v-row>

    <v-row id="b">
    </v-row>

<v-row>
  <v-col>
    <template>
  <v-card
    :loading="loading" class="mx-auto my-12" max-width="374">
    <template slot="progress">
      <v-progress-linear color="deep-purple" height="10" indeterminate
      ></v-progress-linear>
    </template>
    <v-img
      height="250" src="https://www.blog.cazcarra.com/wp-content/uploads/2019/04/tecnicas-de-corte-de-cabello.jpg"
    ></v-img>

    <v-card-title>Corte de cabello</v-card-title>

    <v-card-text>
      <v-row
        align="center" class="mx-0">
        <v-rating
          :value="5.0" color="amber" dense half-increments readonly size="14">
        </v-rating>
        <div class="grey--text ms-4">
          5.0 (413)
        </div>
      </v-row>
      <div class="my-4 text-subtitle-1">
        $ • Italian, Cafe
      </div>
      <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
    </v-card-text>
    <v-divider class="mx-4"></v-divider>
    <v-card-title>Tonight's availability</v-card-title>
    <v-card-text>
    </v-card-text>

    <v-card-actions>
      <v-btn
        color="deep-purple lighten-2" text @click="reserve"
      >
        Reserve
      </v-btn>
    </v-card-actions>
  </v-card>
</template>
      </v-col>  
    </v-row>

    </v-container-fluid>
    
</template>


<script>
  export default {
    name: 'HelloWorld',
    
    data: () => ({
      loading: false,
      selection: 1,
    }),
    methods:{
      reserve () {
        this.loading = true
        setTimeout(() => (this.loading = false), 2000)
      },
      showAlert() {
      // Use sweetalert2
      this.$swal('Este es tu carrito de compras');
    },
    }
  }
  
</script>
<style>

#i{
height:40px;
}
#i2{
  height:450px;
  width: 100vw;
  background-image: url("https://i.ibb.co/W3RhxBL/Sin-t-tulo-2.png");
}
#b{
  width:100vw;
  height:100px;
  background-image :url("https://i.ibb.co/6PfLKv5/Sin-t-tulo-1.png");
}
</style>