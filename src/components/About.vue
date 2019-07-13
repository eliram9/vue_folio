<template>
    <div id="about">
        <h2 class="display-3">Ab<sapn class="o">o</sapn>ut</h2>
            <v-container fluid>
                <v-layout row align-center>
                        <v-flex xs8 md10 lg6 xl5> 
                            <v-card flat color="#fefffa">
                                <a><img src="../assets/me.png" alt="me"></a>
                            </v-card>   
                        </v-flex>

                        <v-flex xs12 md10 lg5 xl6> 
                            <v-card flat color="#fefffa">
                                <h1>I'm Eliram,</h1>
                                <h1>A Front-End & UI/UX Developer. 
                                    <br>
                                    Entrepreneur with Engineering, Consulting and Management Experience.
                                </h1>    
                            </v-card>   
                        </v-flex>
                </v-layout>
            </v-container> 

            <div class="showMore">
                <v-container align-center>
                        <v-btn outline 
                               large 
                               round 
                               color="#4DB6AC"
                               @click="toggle">Show {{ showMore ? 'Less' : 'More' }}
                        </v-btn>
                    <br />

                        <!-- Technologies section -->
                            <v-layout justify-center>
                                <v-flex xs12 sm12 md10 lg8 xl7>
                                    <v-card flat color="#fefffa" v-if="showMore">
                                        <br>
                                        <h1  class="technologies">{{ techo }}</h1>
                                            <br>
                                                <h3>Javascript <span class="row1">|</span> jQuery 
                                                            <span class="row1">|</span> HTML5 
                                                            <span class="row1">|</span> Node.js 
                                                            <span class="row1">|</span> Express 
                                                            <span class="row1">|</span> JSON 
                                                            <span class="row1">|</span> AJAX 
                                                            <span class="row1">|</span> RESTful API's
                                                </h3>
                                            <br>    
                                            <hr>
                                            <br>
                                                <h3>UI/UX <span class="row2">|</span> CSS 
                                                        <span class="row2">|</span> CSS3 
                                                        <span class="row2">|</span> Bootstrap 
                                                        <span class="row2">|</span> Sass 
                                                        <span class="row2">|</span> Adobe Xd / Ai 
                                                        <span class="row2">|</span> Material-UI 
                                                        <span class="row2">|</span> Canva 
                                                        <span class="row2">|</span> Responsive design
                                                </h3>
                                            <br>    
                                            <hr>
                                            <br>
                                                <h3>MongoDB <span class="row3">|</span> SQL 
                                                            <span class="row3">|</span> Firebase
                                                </h3>
                                            <br>    
                                            <hr>
                                            <br>
                                                <h3>React.js <span class="row4">|</span> Vue.js 
                                                            <span class="row4">|</span> Ionic
                                                </h3> 
                                            <br>    
                                            <hr>
                                            <br>
                                                <h3>Git <span class="row5">|</span> Agile / Scrum methodologies 
                                                        <span class="row5">|</span> Jira 
                                                        <span class="row5">|</span> Testing 
                                                        <span class="row5">|</span> GitHub 
                                                        <span class="row5">|</span> Bitbucket
                                                </h3> 
                                            <br>    
                                                    
                                    </v-card> 
                                </v-flex>
                            </v-layout>
                    
                        <!-- Download option -->
                        <br> 
                        <v-btn outline 
                               round 
                               color="#FF8A65" 
                               v-if="showMore" 
                               a href="/myResume.pdf" 
                               download="Eliram Malachi - Resume.pdf">
                                View / Download Resume
                        </v-btn>
                </v-container>
            </div>       
    </div>      
</template>

<script>
export default {
    data () {
        return {
            showMore: false,
            techo: '< Technologies />'
        }
    },
    methods: {
        toggle() {
           this.showMore = !this.showMore
        }
    }
}
</script>

<style scoped>
    #about {
        min-height: 100vh;
        background-color: #fefffa !important;
    }

    .display-3 {
        color: #78909C;
        padding-top: 4.5%;
        font-size: 4vmax !important;
        font-family: 'Poiret One', cursive !important;
    }

    .o {
        color: #FFAB91;
    }

    img {
        width: 25vmax;
    }

    h1 {
        color: #78909C;
        font-size: 2.9vmax;
        font-family: 'Dosis', sans-serif;
        font-weight: 300;
    }

    /* Technologies */
    .technologies {
        color: #78909C;
        font-weight: 300 !important;
        font-family: 'Source Code Pro', monospace;
    }
    h3 {
        color: #78909C;
        font-weight: 300 !important;
        font-family: 'Source Code Pro', monospace;
    }
    .row1 {
        color: #F48FB1;
    }
    .row2 {
        color: #9FA8DA;
    }
    .row3 {
        color: #B39DDB;
    }
    .row4 {
        color: #C5E1A5;
    }
    .row5 {
        color: #FFCC80;
    }
</style>

