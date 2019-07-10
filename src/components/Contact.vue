<template>
    <div id=contact>
        <h2 class="display-3">Contact</h2>
            <v-container fill-height>
                <v-layout >
                    <v-flex>
                        <a v-bind:href="github"><img src="../assets/git.png" alt="git"></a>
                        <a :href="linkedin"><img src="../assets/linked.png"></a>
                        <a :href="instagram"><img src="../assets/insta.png"></a>
                        <img src="../assets/mail.png">
                    </v-flex>
                </v-layout>
            </v-container>
    </div>
</template>

<script>
export default {
    data() {
        return {
            github: 'https://github.com/eliram9',
            linkedin: 'https://www.linkedin.com/in/eliram9/',
            instagram: 'https://www.instagram.com/eliramalachi/?hl=en'
        }
    }
}
</script>

<style scoped>
    #contact {
        min-height: 22vh;
        background-color: #fefffa;
    }

    .display-3 {
        font-family: 'Poiret One', cursive !important;
    }

    img {
        max-width: 3.5vmax;
        margin: 1% 1%;
    }
</style>
