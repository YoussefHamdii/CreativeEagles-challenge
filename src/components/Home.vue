<template>
  <div class="flex">
    <CardComponent v-for="item in deals" :key="item" :item="item"/>
  </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
import axios from 'axios';

  export default {
    name: 'HelloWorld',
    components: {
      CardComponent,
    },
    data(){
      return{
        deals: []
      }
    },

    mounted(){
      axios.get('https://prime-crowd.com/api/mock/rounds')
      .then(res => {this.deals = res.data;})
    }

  }
</script>
