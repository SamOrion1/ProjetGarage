<template>
  <v-app id="app">
    <header>
      <v-app-bar color="#333333">

        <!-- Icon Burger -->
        <v-app-bar-nav-icon @click="drawer = true" class="d-flex d-sm-none" color="white"></v-app-bar-nav-icon>

        <!-- Titre navbar -->
        
        <v-toolbar-title><v-img id="logoGarage" max-height="40" max-width="280" src="@/assets/logoGarage.jpg"></v-img></v-toolbar-title>

        <v-spacer></v-spacer>

        <!-- Bouton navbar -->
        <template>
          <v-tabs align-with-title class="d-none d-sm-flex" color="yellow">
            <v-tabs-slider color="yellow"></v-tabs-slider>
            <v-tab v-for="item in navbars" v-bind:key="item.id" :to="{ path: item.router }">
              {{  item.names  }}
            </v-tab>
          </v-tabs>
        </template>

      </v-app-bar>

      <!-- Burger -->
      <v-navigation-drawer v-model="drawer" absolute temporary color="#333333">
        <v-list nav dense>
          <v-list-item-group>
            <v-list-item v-for="item in navbars" v-bind:key="item.id" :to="{ path: item.router }">{{  item.names  }}
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>

      <router-view></router-view>
    </header>

    <v-main></v-main>


    <v-footer dark padless>
      <v-card flat tile class="lighten-1 white--text text-center" color="#333333">
        <v-card-text>
          <v-btn v-for="icon in icons" :key="icon" class="mx-4 white--text" icon>
            <v-icon size="24px">
              {{  icon  }}
            </v-icon>
          </v-btn>
        </v-card-text>

        <v-card-text class="white--text pt-0">
          Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent
          ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet
          dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum
          ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci
          varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{  new Date().getFullYear()  }} — <strong>Vuetify</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>


export default {

  name: 'App',

  data: () => ({

    drawer: false,
    tab: null,

    navbars: [
      { names: 'Accueil', router: '/', id: 1 },
      { names: 'Services', router: '/Services', id: 2 },
      { names: 'xx', router: '/xx', id: 3 },
      { names: 'xx', router: '/xx', id: 4 },
      { names: 'xx', router: '/xx', id: 5 }
    ],


    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ]

  })
}
</script>

<style lang="scss">
  
#logoGarage {
  
}

//Couleur des bouttons navbar
.theme--light.v-tabs>.v-tabs-bar .v-tab:not(.v-tab--active),
.theme--light.v-tabs>.v-tabs-bar .v-tab:not(.v-tab--active)>.v-icon,
.theme--light.v-tabs>.v-tabs-bar .v-tab:not(.v-tab--active)>.v-btn,
.theme--light.v-tabs>.v-tabs-bar .v-tab--disabled {
  color: white;
}

//Couleur des bouttons Burger
.v-list--nav.v-list--dense .v-list-item:not(:last-child):not(:only-child),
.v-list--nav .v-list-item--dense:not(:last-child):not(:only-child),
.v-list--rounded.v-list--dense .v-list-item:not(:last-child):not(:only-child),
.v-list--rounded .v-list-item--dense:not(:last-child):not(:only-child) {
  color: white;
}

* {
  margin: 0%;
  padding: 0%;
  border: 0%;
}

//Enlève l'espace entre le footer et le composent
.v-application--wrap {
  min-height: unset;
}
</style>