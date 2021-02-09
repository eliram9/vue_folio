<template>
    <div id="projects">
        <h2 class="display-3">Pr<span class="o">o</span>jects</h2>
        <br />
        
            <v-container fluid>
                <v-layout justify-center>
                    <v-flex xs12 sm12 md10 lg8 xl6>
                        <v-timeline>
                            <v-timeline-item 
                                v-for="(project, index) in projects"
                                :key= index
                                color="#FFAB91"
                                small
                            > 
                                <template v-slot:opposite>
                                    <span><h3>{{ project.name }}</h3></span>
                                </template>
                                <v-hover > 
                                    <v-card flat slot-scope={hover}>
                                        <img v-bind:src="project.img"> 

                                        <!-- card expand after user hover -->
                                        <v-expand-transition>
                                            <div
                                                v-if="hover"
                                                class="d-flex transition-fast-in-fast-out 
                                                       blue-grey lighten-2 v-card--reveal 
                                                       white--text"
                                                style="height: 100%;"
                                            >
                                                <v-card-text>
                                                    {{ project.description }}
                                                </v-card-text>
                                            </div>
                                        </v-expand-transition>
                                        <!-- /end -->

                                        <p class="builtTitle">Built with</p>
                                            <span v-for="tool in project.tools" :key=tool>
                                                <img class="img-build" v-bind:src="tool" />
                                            </span>
                                        <br>
                                    </v-card> 
                                </v-hover>    
                                        <br>
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
                            // require('../assets/mate.png')
                    ], 
                    description: 'A simple web application that shows my favorite crypto-currency coin prices in real time. built with react.js',
                    link: 'https://eliram9.github.io/new_cryptoreact/'
                },
                {
                    name: 'Cryptocurrency',
                    img: require('../assets/oldCrypto.png'),
                    tools: [
                            require('../assets/html.png'),
                            require('../assets/css.png'),
                            require('../assets/js.png'),
                            require('../assets/api.png'),
                            require('../assets/boot.png')    
                    ],
                    description: 'My favorive crypto coins rate in real time',
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
                    description: 'Web Application for the quickest route comparing between Bing, Google and MapQuest GPS on one page.',
                    link: 'https://eliram9.github.io/QuickestWay/'
                },
                {
                    name: 'ReactFolio',
                    img: require('../assets/portfo.png'),
                    tools: [
                            require('../assets/react.png')
                    ],
                    description: 'Free Portfolio template for web developers',
                    link: 'https://github.com/eliram9/react_portfolio'
                },
                {
                    name: 'FireAuth',
                    img: require('../assets/profile.png'),
                    tools: [
                            require('../assets/react.png')
                    ],
                    description: 'User Authontication with React.js & firebase, coming soon...'
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

    .theme--light.v-sheet {
        background-color: #fefffa;
    }

    .v-timeline-item .v-card:before, .v-timeline-item .v-card:after {
        position: fixed !important; 
    }

    .img-build {
        width: 2.5vmax;
        margin-left: 1%
    }

    .v-card--reveal {
        align-items: center;
        bottom: 0;
        justify-content: center;
        opacity: .85;
        position: absolute;
        width: 100%;
        border-radius: 12%; 
        
    }
    .d-flex {
        font-size: 1.5vmax;
        font-weight: bold;
        font-family: 'Dosis', sans-serif;
        /* padding: 15% 5% 7% 15%; */
    }
    .builtTitle {
        margin-top: 10%;
        color:#78909C; 
        font-size: 1.1vmax;
        font-family: 'Dosis', sans-serif;
    }
</style>
