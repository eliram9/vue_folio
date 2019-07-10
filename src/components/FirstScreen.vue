<template>
    <div id="first">

        <v-container fill-height>
            <v-layout row wrap align-center>
                <v-flex class="text-xs-center"> 
                    <h1>Hello, I'm <span class="name">Elir</span>
                                   <span class="a">a</span>
                                   <span class="name">m M</span>
                                   <span class="a">a</span>
                                   <span class="name">l</span>
                                   <span class="a">a</span>
                                   <span class="name">chi</span>.
                    </h1>
                    <h1>I'm a Front-End & UI/UX Developer</h1>
                <br>    
                    <v-btn large 
                           outline
                           fab 
                           href="#about" 
                           color="blue-grey lighten-1"
                           class="explore">
                           Explore
                    </v-btn>
                </v-flex>
            </v-layout>
        </v-container>
        
    </div>
</template>

<script>
    export default {
        name: 'FirstScreen',

        data() {
            return {
                url: 'https://www.google.com'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    #first {
        height: 100vh;
        background-color: #fefffa;
    }
    
    h1 {
        color: #78909C;
        font-size: 3vmax;
        font-weight: 200;
        font-family: 'Dosis', sans-serif;
    }

    .name{
        color: #B2DFDB;
    }

    .a {
        color: #FFAB91;
    }

    /* .explore:hover {
        font-size: 20vmax;
    } */
</style>
