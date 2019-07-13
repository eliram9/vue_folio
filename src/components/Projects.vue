<template>
    <div id="projects">
        <h2 class="display-3">Pr<sapn class="o">o</sapn>jects</h2>
        <br />
        
            <v-container fluid>
                <v-layout justify-center>
                    <v-flex xs12 sm12 md10 lg8 xl6>
                        <v-timeline>
                            <v-timeline-item 
                                v-for="project in projects"
                                :key= project
                                color="#FFAB91"
                                small
                            > 
                                <template v-slot:opposite>
                                    <span><h3>{{ project.name }}</h3></span>
                                </template>
                                    <v-card flat>
                                        <!-- <v-card-title class="headline">Hi</v-card-title> -->
                                        <img v-bind:src="project.img"> 
                                        <v-card-text>
                                            {{ project.description }}
                                        </v-card-text>

                                        <p>built with</p>
                                        <span v-for="tool in project.tools" :key=tool>
                                            <img class="img-build" 
                                                v-bind:src="tool" />
                                        </span>

                                        <br>
                                    </v-card> 
                                        <a v-bind:href="project.link" 
                                           class="liveApp">
                                            Live App
                                        </a> 
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
                    tools: [
                            require('../assets/react.png'),
                            require('../assets/api.png'),
                            require('../assets/mate1.png')
                    ], 
                    description: 'amazing',
                    link: 'https://eliram9.github.io/cryptoreact/'
                },
                {
                    name: 'Cryptocurrrnecy',
                    img: require('../assets/oldCrypto.png'),
                    tools: [
                            require('../assets/html.png'),
                            require('../assets/css.png'),
                            require('../assets/js.png'),
                            require('../assets/api.png'),
                            require('../assets/boot.png')    
                    ],
                    description: 'old',
                    link: 'https://eliram9.github.io/crypto/'
                },
                {
                    name: 'QuickestWay',
                    img: require('../assets/navi.png'),
                    tools: [
                            require('../assets/html.png'),
                            require('../assets/css.png'),
                            require('../assets/js.png'),
                            require('../assets/api.png'),
                            require('../assets/boot.png')    
                    ],
                    description: 'fast',
                    link: 'https://eliram9.github.io/QuickestWay/'
                },
                {
                    name: 'PortFolio',
                    img: require('../assets/portfolio.png'),
                    tools: [
                            require('../assets/react.png')
                    ],
                    description: 'great',
                    link: 'https://github.com/eliram9/react_portfolio'
                }
            ]
        }
    }
}
</script>

<style scoped>
    #projects {
        height: 100%;
        background-color: #fefffa;
    }

    /* Cards */
    .display-3 {
        color: #78909C;
        padding-top: 4.5%;
        font-size: 4vmax !important;
        font-family: 'Poiret One', cursive !important;
    }

    .o {
        color: #FFAB91;
    }

    h3 {
        color:#78909C; 
        font-size: 2vmax;
        font-family: 'Dosis', sans-serif;
    }

    img{
        width: 13vmax;
    }

    .liveApp {
        color: #80CBC4;
        font-size: 2.5vmin;
        text-decoration: none;
    }

    .v-timeline-item .v-card:before, .v-timeline-item .v-card:after {
        position: fixed !important; 
    }

    .img-build {
        width: 3vmax;
        margin-left: 1%
    }

    .theme--light.v-sheet:hover {
        background-color: red;
        opacity: .1;
    }
</style>
