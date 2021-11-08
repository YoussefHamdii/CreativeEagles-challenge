<template>
    <div>
        <ul class="flex border-b-2 ">
            <li class="pr-7 pl-5 pb-3" @click="selected=1" :class="selected == 1?' border-b-2 border-black':''">
                <button>
                    All
                </button>
            </li>
            <li class="px-7 pb-3" @click="selected=2" :class="selected ==2?'border-b-2 border-black':'border-gray-300'">
                <button>
                    Active
                </button>
            </li>
            <li class="px-7 pb-3" @click="selected=3" :class="selected ==3?'border-b-2 border-black':'border-gray-300'">
                <button>
                    Coming soon
                </button>
            </li>
        </ul>
    </div>
</template>

<script>

export default {
    name: "CategoryComponent",
    data(){
        return{
            hover: false,
            hover1: false,
            selected: 2
        };
    }
}
</script>

<style scoped>

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
