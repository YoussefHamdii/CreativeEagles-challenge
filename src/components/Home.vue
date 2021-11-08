<template>
  <div class="pl-10 w-400 bg-gray-100">
  <UserComponent class="pt-10" :items="deals" />
  <hr />
  <CategoryComponent class="py-5"/>
  <div class="flex flex-initial">
    <CardComponent v-for="item in deals" :key="item" :item="item"/>
  </div>
  </div>
</template>

<script>
import CardComponent from './CardComponent.vue';
import CategoryComponent from './CategoryComponent.vue';
import UserComponent from './UserComponent.vue';
import axios from 'axios';

  export default {
    name: 'HelloWorld',
    components: {
      CardComponent,
      CategoryComponent,
      UserComponent,
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
