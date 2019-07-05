<template>
    <div id="toolbar">
        <v-toolbar inverted-scroll app color="cyan lighten-5">
            <v-toolbar-title>E<span class="M">M</span></v-toolbar-title>
                <v-toolbar-items>
                    <v-btn flat>About</v-btn>
                    <v-btn flat>Projects</v-btn>
                    <v-btn flat>Contact</v-btn>
                </v-toolbar-items>
        </v-toolbar>
    </div>    
</template>

<script>
export default {

}
</script>

<style scoped>
    .v-toolbar__title {
        color: red;
        font-size: 2vmax;
        font-size: 5.5vmin;
        font-family: 'Poiret One', cursive;
    }
    .M {
        color: green;
        font-weight: bolder;
    }
</style>
