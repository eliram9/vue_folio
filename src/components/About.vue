<template>
    <div id="about">
        <h2 class="display-3">About</h2>
            <v-container fluid>
                <v-layout row>
                        <v-flex xs12 lg6 xl5> 
                            <v-card flat color="#F1F8E9">
                                <a><img src="../assets/me.png" alt="me"></a>
                            </v-card>   
                        </v-flex>

                        <v-flex xs12 lg5 xl6> 
                            <v-card flat>
                                <h1>I'm Eliram Malachi,</h1>
                        <br>
                                <h1>A Front-End & UI/UX Developer Entrepreneur with Engineering, Consulting and Management Experience. </h1>    
                            </v-card>   
                        </v-flex>
                </v-layout>
            </v-container> 

            <div class="showMore">
                <v-container align-center>
                        <v-btn outline large round @click="toggle">Show {{ showMore ? 'Less' : 'More' }}</v-btn>
                    <br />

                        <!-- Technologies section -->
                            <v-layout justify-center>
                                <v-flex xs12 sm12 md10 lg8 xl7>
                                    <v-card color="#fefffa" v-if="showMore">
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
                        <v-btn outline round color="indigo" 
                               v-if="showMore" a href="/myResume.pdf" 
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
        min-height: 95vh;
        background-color: darkseagreen !important;
    }

    img {
        width: 25vmax;
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

