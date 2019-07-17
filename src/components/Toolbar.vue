<template>
    <div id="toolbar">
        <v-toolbar inverted-scroll app color="blue-grey lighten-2">
            <v-toolbar-title>E<span class="M">M</span></v-toolbar-title>
                <v-toolbar-items>
                    <v-btn round flat href="#about" class="btn">About</v-btn>
                    <v-btn round flat href="#projects" class="btn">Projects</v-btn>
                    <v-btn round flat href="#contact" class="btn">Contact</v-btn> 
                </v-toolbar-items>
        </v-toolbar>
    </div>    
</template>

<script>
export default {
    data() {
        return {
            
        }
    }
}
</script>

<style scoped>
    /* Toolbar tile */
    .v-toolbar__title {
        /* color: #78909C; */
        color: #F1F8E9;
        font-size: 2vmax;
        font-size: 5.5vmin;
        font-family: 'Poiret One', cursive;
    }
    .M {
        color: #FFAB91;
        font-weight: bolder;
    }

    /* Tollbat items */
    .btn {
        color: #F1F8E9;
        font-weight: 600;
        font-family: 'Poiret One', cursive;
    } 
    .btn:hover {
        background-color: rgba(255, 171, 145, 0.342);
        color: white;
        transform: rotateZ(-30deg);
        height: 50%;
    }  
</style>
