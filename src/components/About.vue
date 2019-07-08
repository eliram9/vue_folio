<template>
    <div class="about">
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
                    <v-btn @click="toggle">Show {{ showMore ? 'Less' : 'More' }}</v-btn>
                <br />
                        <v-card v-if="showMore">
                            <h1>Technologies</h1>
                        </v-card>

                    <v-btn v-if="showMore" a href="/myResume.pdf" download="Eliram Malachi - Resume.pdf">
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
            showMore: false
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
    .about {
        height: 100vh;
        background-color: darkseagreen !important;
    }

    img {
        width: 25vmax;
    }
</style>

