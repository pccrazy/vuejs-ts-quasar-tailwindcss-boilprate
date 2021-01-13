<template>
  <div class=" bg-gray-100">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <Login msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Login from './components/Login.vue';

@Component({
  components: {
    Login,
  },
})
export default class App extends Vue {}
</script>

<style>

</style>
