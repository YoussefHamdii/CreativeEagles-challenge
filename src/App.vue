<template>
  <div class="flex flex-auto">
    <NavigationComponent />
    <Home class="bg-gray-100"/>
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
