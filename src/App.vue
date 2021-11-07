<template>
  <div class="flex">
    <NavigationComponent class="w-75" />
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
