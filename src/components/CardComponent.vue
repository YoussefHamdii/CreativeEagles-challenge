<template>
<v-card
    :loading="loading"
    class="mx-auto my-12"
    max-width="374"
  >

    <v-img
      height="125"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

    <div class="my-2 mx-3.5 text-sm py-0.5 text-white bg-cyan-900 w-25 text-center rounded-md">2 Days left </div>

    <v-card-title class="text-cyan-900 font-mono font-bold py-0">Cafe Badilico</v-card-title>

    <progress value="25" max="100" class="h-1 mx-4 wid"></progress>

    <v-card-text>
      <div class="my-2 text-subtitle-1">
        $ • Italian, Cafe
      </div>

      <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
    </v-card-text>

    <v-card-text>
      <v-chip-group
        v-model="selection"
        active-class="deep-purple accent-4 white--text"
        column
      >
        <v-chip>Active</v-chip>

        <v-chip>Startup</v-chip>

      </v-chip-group>
      
    </v-card-text>

<v-divider class="mx-4"></v-divider>

    

    <v-card-title>Tonight's availability</v-card-title>
    
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
}
</script>

<style scoped>
.wid{
  width: 90%;
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
