<template>
    <div id=contact>
        <h2 class="display-3">Contact</h2>
        <br />
        <a v-bind:href="github"><img src="../assets/git.png" alt="git"></a>
        <a :href="linkedin"><img src="../assets/linked.png"></a>
        <a :href="instagram"><img src="../assets/insta.png"></a>
        <img src="../assets/mail.png">
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
        height: 50vh;
        background-color: #fefffa;
    }
    img {
        max-width: 3.5vmax;
        margin: 1% 1%;
    }
</style>
