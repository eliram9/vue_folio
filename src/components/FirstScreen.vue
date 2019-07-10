<template>
    <div id="first">

        <v-container fill-height>
            <v-layout row wrap align-center>
                <v-flex class="text-xs-center"> 
                    <h1>Hello, I'm Elir<span class="a">a</span>m M<span class="a">a</span>l<span class="a">a</span>chi.</h1>
                    <h1>I'm a Front-End & UI/UX Developer</h1>
                <br>    
                    <v-btn style="color:red">Explore</v-btn>
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

    .a {
        color: #FFAB91;
    }
</style>
