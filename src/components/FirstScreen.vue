<template>
    <div class="first">
        <v-container fill-height>
            <v-layout row wrap align-center>
                <v-flex class="text-xs-center"> 
                    <h1>Hello, I'm Eliram</h1>
                    <h1>I'm a Front-End & UI/UX Developer</h1>
                <br>    
                    <v-btn>Explore</v-btn>
                </v-flex>
            </v-layout>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'FirstScreen',
    props: {
        msg: String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .first {
        height: 100vh;
        background-color: pink;
    }
    
    h1 {
        color: blue;
        font-size: 3vmax;
        font-weight: 200;
        font-family: 'Dosis', sans-serif;
    }
</style>
