<template>
    <div id="first">
        
        
        <h1 class="fadeLine">
            Hello, I'm <span class="name">Elir</span>
            <span class="a">a</span>
            <span class="name">m M</span>
            <span class="a">a</span>
            <span class="name">l</span>
            <span class="a">a</span>
            <span class="name">chi</span>.
            
        </h1>

           <h1 class="line anim-typewriter"> I'm a <span class="front">{{ front }}</span> Front-End <span class="front">{{ front2 }}</span> & 
                <span class="uiux">U<span class="oc">I</span>/<span class="oc">U</span>X</span> 
                Developer</h1>
                <br>    
                    <!-- <v-btn large 
                           outline
                           fab 
                           href="#about" 
                           color= #B2DFDB
                           class="explore">
                           Explore
                    </v-btn> -->
        
       <vue-particles
        color="#FFAB91"
        :particleOpacity="0.7"
        :particlesNumber="80"
        shapeType="circle"
        :particleSize="3"
        linesColor="#C7C7C7"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="3"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="true"
        clickMode="push"
      >
      </vue-particles>
     
    </div>
</template>

<script scope>
    export default {
        name: 'FirstScreen',

        data() {
            return {
                url: 'https://www.google.com',
                front: '<',
                front2: '/>'
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

    #particles-js {
        position: absolute;
        z-index: 0;
        top: 0;
        width: 100vw;
    }

    .name{
        color: #B2DFDB;
    }

    .a {
        color: #FFAB91;
    }

    .fadeLine {
        position: relative;
        top: 50%;
        margin: 0 auto;
        font-size: 3.1vmax;
        text-align: center;
        transform: translateY(-180%);
        color: #78909C;
        font-weight: 200;
        font-family: 'Dosis', sans-serif;
        animation: fadeIn 4s;
    }
    @keyframes fadeIn {
        from {
            opacity: 0;
        }
        to  {
            opacity: 1;
        }
    }

    .line {
        position: relative;
        top: 50%;
        width: 16em;
        margin: 0 auto;
        border-right: 2px solid #78909C;
        font-size: 3vmax;
        text-align: center;
        white-space: nowrap;
        overflow: hidden;
        transform: translateY(-175%);
        color: #78909C;
        font-weight: 200;
        font-family: 'Dosis', sans-serif;
    }  

    .anim-typewriter {
        transition-delay: 1s;
        animation: typewriter 4s steps(30) 1s 1 normal both,
        blinkTextCursor 500ms steps(30) infinite normal;
    } 

    @keyframes typewriter {
        from {
            width: 0;
        }
        to {
            width: 14.7em;
        }
    }
    @keyframes blinkTextCursor {
        from {
            border-right-color: #78909C; 
        }
        to {
            border-right-color: transparent;
        }
    }

    .front {
       font-weight: bold;
    }
    .uiux {
        transition-delay: 2.5s;
        text-shadow: 2.5px 1.5px #B2DFDB;
    }
    .oc {
        text-shadow: 2.5px 1.5px #FFAB91;
    }

    .explore {
        font-size: 1vmax;
        text-align: center;
        color: #78909C;
        font-weight: 600;
        position: relative;
        font-family: 'Dosis', sans-serif;
    }    

</style>
