<template>
<v-card
    :loading="loading"
    class="mx-auto"
    max-width="350"
  >
    <v-img
      height="125"
      :src="item.banner"
    ></v-img>

    <div class="my-2 mx-3.5 text-sm py-0.5 text-white bg-cyan-900 w-25 text-center rounded-md">2 Days left </div>

    <v-card-title class="text-cyan-900 font-mono font-bold py-0">{{item.title}}</v-card-title>
    
    <v-card-text class="font-mono text-sm font-bold py-0">
      <div class="text-cyan-900">
         <span class=" text-lg text-lime-500 align-middle">{{Math.round(item.current_investment/item.investment_goal*100)}}%</span>
          {{item.investment_goal - item.current_investment}} € left to fund
      </div>
      </v-card-text>
      
    <progress :value="item.current_investment/item.investment_goal*100" max="100" class="h-1 mx-4 wid"></progress>

    <v-card-text class="py-0 font-mono text-sm font-medium">
      <div class="text-cyan-900">{{item.teaser}}</div>
    </v-card-text>

    <v-card-text>
      <v-chip-group
        column
      >
        <v-chip>Active</v-chip>

        <v-chip>Startup</v-chip>

      </v-chip-group>
      
    </v-card-text>

    <v-divider></v-divider>
    <div class="flex">

      <div class="w-50 text-center">
        <v-card-text class="py-0 pt-4 text-lg font-medium text-cyan-900">{{item.investor_count}}</v-card-text>
        <v-card-text class="py-0 pb-4 text-cyan-700">Want to invest</v-card-text>
      </div>

      <v-divider
      class="mx-4"
      vertical
      ></v-divider>

      <div class="w-50 text-center">
        <v-card-text class="py-0 pt-4 text-lg font-medium text-cyan-900">{{item.current_investment}} €</v-card-text>
        <v-card-text class="py-0 pb-4 text-cyan-700">Funding Round</v-card-text>
      </div>

    </div>
    
      <button
        class="wid p-3.5 rounded-md mx-5 my-2 bg-cyan-900 text-white"
      >
        Learn more
      </button>
    
  </v-card>
</template>

<script>
//import vuetify from 'vuetify';
export default {
    name: "CardComponent",
    props:['item'],
}
</script>

<style scoped>
.wid{
  width: 90%;
}

progress{
  padding: 0;
}

progress[value]::-webkit-progress-bar {
  background-color: #EAF5EB;
  border-radius: 2px;
}

progress[value]::-webkit-progress-value {
  background-image:
    -webkit-linear-gradient(-45deg, transparent 33%, rgba(0, 0, 0, .1) 33%, rgba(0,0, 0, .1) 66%, transparent 70%);
    border-radius: 2px; 
    background-size: 15px 5px, 100% 100%, 100% 100%;
    background-color: #84bd62;
}

</style>
