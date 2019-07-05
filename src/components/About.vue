<template>
    <div class="about">
        <v-container fluid>
            <v-layout row>
                    <v-flex xs12 lg6 xl5> 
                        <v-card flat>
                            <a><img src="./me.png" alt="me"></a>
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
    </div>      
</template>

<script>
export default {

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

