<template>
    <div id=contact>
        <h2 class="display-3">C<sapn class="o">o</sapn>ntact</h2>
            <v-container fill-height>
                <v-layout >
                    <v-flex>
                        <a v-bind:href="github"><img src="../assets/git.png" alt="git"></a>
                        <a :href="linkedin"><img src="../assets/linked.png"></a>
                        <a :href="instagram"><img src="../assets/insta.png"></a>
                        <a :href="mail"><img src="../assets/mail.png"></a>
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
            instagram: 'https://www.instagram.com/eliramalachi/?hl=en',
            mail: 'mailto:eliram9@gmail.com'
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
        color: #78909C;
        font-family: 'Poiret One', cursive !important;
    }

    .o {
        color: #FFAB91;
    }

    img {
        max-width: 4vmax;
        margin: 1% 1%;
    }
</style>
