<template>
    <v-main>
        <v-container id="carousel">
            <v-row>
                
                <v-carousel cycle hide-delimiter-background show-arrows-on-hover>
                    <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src"></v-carousel-item>
                </v-carousel>

            </v-row>
        </v-container>
    </v-main>
</template>

<script>
export default {
    name: 'carousel-S',

    data() {
        return {
            items: [
                {
                    src: require('@/assets/C1.jpg'),
                },
                {
                    src: require('@/assets/C2.jpg'),
                },
                {
                    src: require('@/assets/C3.jpg'),
                },
                {
                    src: require('@/assets/C4.jpg'),
                },
            ],
        }
    },
}
</script>

<style lang="scss">
#carousel {
    margin-top: 5%;
    max-width: 85%;
    
}
</style>