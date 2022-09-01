<template>
    <v-main id="card">
        <v-container>
        <v-row>
            <!-- Premier CARD -->
            <v-card class="mx-auto" max-width="344" elevation="24">
                <v-img src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" height="200px"></v-img>

                <v-card-title>
                    Top western road trips
                </v-card-title>

                <v-card-subtitle>
                    1,000 miles of wonder
                </v-card-subtitle>

                <v-card-actions>

                    <v-spacer></v-spacer>

                </v-card-actions>

                <v-expand-transition>
                    <div v-show="show">
                        <v-divider></v-divider>

                        <v-card-text>
                            I'm a thing. But, like most politicians, he promised more than he could deliver. You won't
                            have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go
                            with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do
                            his laundry? I've got to find a way to escape.
                        </v-card-text>
                    </div>
                </v-expand-transition>
            </v-card>

            <!-- Deuxième CARD -->
            <v-card class="mx-auto" max-width="344" elevation="24">
                <v-img src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" height="200px"></v-img>

                <v-card-title>
                    Top western road trips
                </v-card-title>

                <v-card-subtitle>
                    1,000 miles of wonder
                </v-card-subtitle>

                <v-card-actions>

                    <v-spacer></v-spacer>

                </v-card-actions>

                <v-expand-transition>
                    <div v-show="show">
                        <v-divider></v-divider>

                        <v-card-text>
                            I'm a thing. But, like most politicians, he promised more than he could deliver. You won't
                            have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go
                            with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do
                            his laundry? I've got to find a way to escape.
                        </v-card-text>
                    </div>
                </v-expand-transition>
            </v-card>
            <!-- Troisième CARD -->
            <v-card class="mx-auto" max-width="344" elevation="24">
                <v-img src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg" height="200px"></v-img>

                <v-card-title>
                    Top western road trips
                </v-card-title>

                <v-card-subtitle>
                    1,000 miles of wonder
                </v-card-subtitle>

                <v-card-actions>

                    <v-spacer></v-spacer>

                </v-card-actions>

                <v-expand-transition>
                    <div v-show="show">
                        <v-divider></v-divider>

                        <v-card-text>
                            I'm a thing. But, like most politicians, he promised more than he could deliver. You won't
                            have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go
                            with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do
                            his laundry? I've got to find a way to escape.
                        </v-card-text>
                    </div>
                </v-expand-transition>
            </v-card>
        </v-row>
    </v-container>
    </v-main>
</template>

<script>
export default {
    name: 'card-S',

    data: () => ({
        show: true,
    }),
}
</script>

  <style lang="scss">
  #card {
      margin: 5%;
  }
  </style>