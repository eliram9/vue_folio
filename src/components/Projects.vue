<template>
    <div>
        <h2>Projects</h2>
            <v-container fluid>
                <v-layout justify-center>
                    <v-flex xs12 sm12 md10 lg8 xl6>
                        <v-timeline>
                            <v-timeline-item 
                                v-for="project in projects"
                                :key= project
                                color="red lighten-2"
                                small
                            > 
                                <template v-slot:opposite>
                                    <span><h1>{{ project.name }}</h1></span>
                                </template>
                                    <v-card flat>
                                        <!-- <v-card-title class="headline">Hi</v-card-title> -->
                                        <img v-bind:src="project.img"> 
                                            <v-card-text>
                                            {{ project.description }}
                                        </v-card-text>
                                        <p>built with</p>
                                        <br>
                                        <v-btn>Live App</v-btn>
                                    </v-card>
                            </v-timeline-item>
                        </v-timeline>
                    </v-flex>
                </v-layout>    
            </v-container>
    </div>    
</template>

<script>
export default {
    data() {
        return {
            projects: [
                {
                    name: 'CryptoReact',
                    img: require('../assets/crypto.png'),
                    description: 'amazing',
                    build: 'vue',
                    link: 'https://www.google.com'
                },
                {
                    name: 'crypto',
                    img: require('../assets/oldCrypto.png'),
                    description: 'old',
                    build: 'vue',
                    link: 'https://www.google.com'
                },
                {
                    name: 'QuickestWay',
                    img: require('../assets/navi.png'),
                    description: 'fast',
                    build: 'vue',
                    link: 'https://www.google.com'
                },
                {
                    name: 'PortFolio',
                    img: require('../assets/portfolio.png'),
                    description: 'great',
                }
            ]    
        }
    }
}
</script>

<style scoped>
    /* .timeLine{
        justify-content: center;
    } */

    img{
        width: 15vmax;
    }
</style>
