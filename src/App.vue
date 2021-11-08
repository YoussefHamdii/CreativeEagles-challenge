<template>
  <div class="flex flex-auto">
    <NavigationComponent />
    <Home />
  </div>
</template>

<script>
import Home from './components/Home.vue';
import NavigationComponent from './components/NavigationComponent.vue';


export default {
  name: 'App',

  components: {
    Home,
    NavigationComponent
  }
};
</script>

<style>
/* global styles */
.wid{
  width: 100%;
}
button {
    border: none;
}

button:focus {
    border: none;
    outline: none;
}

button:focus{
    outline:none;
}

</style>
