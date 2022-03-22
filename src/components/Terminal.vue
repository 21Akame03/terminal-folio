<template>
  <textarea autofocus data-gramm="false" data-gramm_editor="false" data-enable-grammarly="false"
 class="terminal-area"></textarea>

</template>

<style scoped>
@font-face {
  font-family: Hack;
  src: url("src/assets/Hack Regular Nerd Font Complete.ttf")
}


a {
  color: #42b983;
}

.terminal-area {
  background-color: rgba(0, 0, 0, 0.4);
  resize: none;
  color: hsl(140, 100%, 50%);
  font-family: Hack;
  font-size: 0.75rem;
  padding: 10px;

}
</style>


/*
TODO: line by line buffer where 

*/

<script>
import Typed from 'typed.js';
import { onMounted } from '@vue/runtime-core';
export default {
  setup() {
    

    onMounted(() => {
      var options = {
        strings: ["^2000Initialising...^2000\n`Hello World!!` \n\n`We trust you have received the usual lecture from the local System` \n`Administrator. It usually boils down to these three things:` \n\n `    #1) Respect the privacy of others.`\n `    #2) Think before you type.` \n `    #3) With great power comes great responsibility.` ^1000 \n\n` Akame's password: `"],
        loop: false,
        smartBackspace: false,
      }
      var typed = new Typed('.terminal-area', options);

    });
  },
}
</script>