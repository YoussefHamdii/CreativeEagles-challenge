<template>
  <div class="flex">
    <CardComponent />
    <CardComponent />
    <CardComponent /> 
  </div>
</template>

<script>
import CardComponent from './CardComponent.vue';

  export default {
    name: 'HelloWorld',
    components: {
      CardComponent,
    }

  }
</script>
