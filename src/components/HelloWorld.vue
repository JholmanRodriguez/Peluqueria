<template>
  <v-container-fluid>
    <v-row>
      <v-col cols="3">
        <h1 class="mt-4 text-center ">Sala De imagen D' mary</h1>
      </v-col>
      <v-col cols="3">

      </v-col>
      <v-col cols="3" class="mt-6" style="height: 10px;" >
        <v-text-field label="¿Qué te quieres hacer Hoy?" solo dende></v-text-field>

      </v-col>
      <v-col cols="3">
        <button v-if="agregarr === 0">
          <img class="mt-5" src="https://cdn-icons-png.flaticon.com/512/3144/3144456.png" alt="" id="i"
            @click="cambiar()" />
        </button>
      </v-col>
    </v-row>

    <div v-if="agregarr === 0">

      <v-row id="b">

        <v-col>5</v-col>
        <v-col>6</v-col>
        <v-col class="mt-4">
          <button>
            <img height="43px"
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/2048px-Instagram_icon.png"
              alt="">
          </button>
        </v-col>
        <v-col class="white--text mt-4">Mary Rodriguez</v-col>
        <v-col>7</v-col>
        <v-col>8</v-col>
        <v-col class="mt-4">
          <button>
            <img height="43px" src="http://assets.stickpng.com/images/580b57fcd9996e24bc43c53e.png" alt="">
          </button>
        </v-col>
        <v-col class="white--text mt-4">Mary Rodriguez</v-col>
        <v-col>9</v-col>

      </v-row>

      <v-row>
        <v-col cols="1"></v-col>
        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://www.blog.cazcarra.com/wp-content/uploads/2019/04/tecnicas-de-corte-de-cabello.jpg"></v-img>
              <v-card-title>Corte de cabello</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="4">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://vanart.com/funciona/wp-content/uploads/2019/03/shutterstock_609230225-400x280.jpg"></v-img>
              <v-card-title>Keratina</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250" src="https://i.pinimg.com/originals/dc/ba/d5/dcbad53a4fd148e4d136af18d6298b58.jpg">
              </v-img>
              <v-card-title>Cepillados</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>
        <v-col cols="1"></v-col>
      </v-row>

      <v-row>
        <v-col cols="1"></v-col>
        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://cms.modumb.com/assets/img/web/images/u%C3%B1as_de_gel_con_aplicaciones.jpg"></v-img>
              <v-card-title>Uñas acrilicas</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="4">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://www.solopelos.com/img/cms/lifting%20de%20pesta%C3%B1as%20portada%20solopelos%20blog.jpg">
              </v-img>
              <v-card-title>lifting Pestañas</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://personalitia.com/wp-content/uploads/2020/03/diferencia-esmalte-de-u%C3%B1as.jpg"></v-img>
              <v-card-title>Esmalatado semipermanente</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>
        <v-col cols="1"></v-col>
      </v-row>

      <v-row>
        <v-col cols="1"></v-col>
        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250" src="https://www.yoypeluqueria.com/web/image/73861/hidratacion-renew-oil"></v-img>
              <v-card-title>Hidratacion capilar</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="4">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250" src="https://aprende.com/wp-content/uploads/2020/10/Unas-acrilicas-940x580.jpg">
              </v-img>
              <v-card-title>Uñas en gel</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>

        <v-col cols="3">
          <template>
            <v-card :loading="loading" class="mx-auto my-12" max-width="374">
              <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
              </template>
              <v-img height="250"
                src="https://www.elespectador.com/resizer/BejZU1dfqXagc8xuRpmS54C0Cv8=/631x420/filters:format(jpeg)/cloudfront-us-east-1.images.arcpublishing.com/elespectador/UZBWXWL4XVGCVNNAMKBD7CPBYI.jpg">
              </v-img>
              <v-card-title>pedicure</v-card-title>
              <v-card-text>
                <v-row align="center" class="mx-0">
                  <v-rating :value="5.0" color="amber" dense half-increments readonly size="14">
                  </v-rating>
                  <div class="grey--text ms-4">5.0 (413)</div>
                </v-row>
                <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>
                <div>
                  Small plates, salads & sandwiches - an intimate setting with 12
                  indoor seats plus patio seating.
                </div>
              </v-card-text>
              <v-divider class="mx-4"></v-divider>
              <v-card-title>Tonight's availability</v-card-title>
              <v-card-actions>
                <v-btn color="deep-purple lighten-2" text @click="reserve">
                  Reserve
                </v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-col>
        <v-col cols="1"></v-col>
      </v-row>
      </div>
      
    
    <div>
      <v-row>
        <v-col cols="4"></v-col>


        <v-col cols="4">
          <template>
            <v-data-table
              :headers="headers"
              :items="desserts"
              class="elevation-1"
            ></v-data-table>
          </template>
        </v-col>
        <v-col cols="4"></v-col>
      </v-row>
    </div>
    <v-row>
        <v-col>
          <template>
            <v-footer color="primary lighten-1" padless>
              <v-row justify="center" no-gutters>
                <v-btn v-for="link in links" :key="link" color="white" text rounded class="my-2">
                  {{ link }}
                </v-btn>
                <v-col class="primary lighten-2 py-4 text-center white--text" cols="12">
                  {{ new Date().getFullYear() }} — <strong>Sala D' Mary</strong>
                </v-col>
              </v-row>
            </v-footer>
          </template>
        </v-col>
      </v-row>
  </v-container-fluid>
</template>

  <script>
export default {
  name: "HelloWorld",
  data: () => ({
    links: [
      'Siguenos en Facebook!',
      'About Us',
      'WhatsApp',
      'Servicios',
      'Contactanos!',
    ],
    headers: [
       {
            text: 'Dessert (100g serving)',
            align: 'start',
            value: 'name',
          },
      { text: 'Calories', value: 'calories' },
      { text: 'Fat (g)', value: 'fat' },
      { text: 'Carbs (g)', value: 'carbs' },
      { text: 'Protein (g)', value: 'protein' },
    ],
    desserts: [
      {
        name: 'Frozen Yogurt',
        calories: 159,
        fat: 6.0,
        carbs: 24,
        protein: 4.0,
        iron: '1%',
      },
      {
        name: 'Ice cream sandwich',
        calories: 237,
        fat: 9.0,
        carbs: 37,
        protein: 4.3,
        iron: '1%',
      },
      {
        name: 'Eclair',
        calories: 262,
        fat: 16.0,
        carbs: 23,
        protein: 6.0,
        iron: '7%',
      },
      {
        name: 'Cupcake',
        calories: 305,
        fat: 3.7,
        carbs: 67,
        protein: 4.3,
        iron: '8%',
      },
      {
        name: 'Gingerbread',
        calories: 356,
        fat: 16.0,
        carbs: 49,
        protein: 3.9,
        iron: '16%',
      },
      {
        name: 'Jelly bean',
        calories: 375,
        fat: 0.0,
        carbs: 94,
        protein: 0.0,
        iron: '0%',
      },
      {
        name: 'Lollipop',
        calories: 392,
        fat: 0.2,
        carbs: 98,
        protein: 0,
        iron: '2%',
      },
      {
        name: 'Honeycomb',
        calories: 408,
        fat: 3.2,
        carbs: 87,
        protein: 6.5,
        iron: '45%',
      },
      {
        name: 'Donut',
        calories: 452,
        fat: 25.0,
        carbs: 51,
        protein: 4.9,
        iron: '22%',
      },
      {
        name: 'KitKat',
        calories: 518,
        fat: 26.0,
        carbs: 65,
        protein: 7,
        iron: '6%',
      },
    ],
    loading: false,
    selection: 1,
    agregarr: 0
  }),
  methods: {
    reserve() {
      this.loading = true;
      setTimeout(() => (this.loading = false), 2000);
    },
    cambiar() {
      this.agregarr = 1
    },
    cambiarr() {
      this.agregarr = 0
    }

  },
};
</script>
  <style>
  #i {
    height: 40px;
  }
  
  #i2 {
    height: 450px;
    width: 100vw;
    background-image: url("https://i.ibb.co/W3RhxBL/Sin-t-tulo-2.png");
  }
  
  #b {
    width: 100vw;
    height: 100px;
    background-image: url("https://i.ibb.co/6PfLKv5/Sin-t-tulo-1.png");
  }
  </style>