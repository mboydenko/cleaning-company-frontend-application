<template>
    <div class="application">
        <router-view/>
    </div>
</template>

<script lang="ts">

import {Vue, Options} from 'vue-class-component'
import { RouterView } from 'vue-router'

import Home from './views/Home.vue'
import Header from './components/Header.vue'

@Options({
    name: 'application',
    components: {
        Home,
        Header,
        RouterView
    }
})
export default class Application extends Vue {

}

</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

* {
    margin: 0;
    padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html, body {
    min-height: 100vh;
}

#app,.application {
    min-height: 100vh;
}

.container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 1175px;
    margin:auto;
}


</style>
