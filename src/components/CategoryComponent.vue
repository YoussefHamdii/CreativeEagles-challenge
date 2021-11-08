<template>
    <div>
        <ul class="flex ">
            <li class="pr-7 border-b-2 pb-3" @mouseover="hover=true" @mouseleave="hover=false" :class="hover?'border-black':'border-gray-300'">
                <button>
                    All
                </button>
            </li>
            <li class="px-7 border-b-2 border-black">
                <button>
                    Active
                </button>
            </li>
            <li class="px-7 border-b-2 pr-200" @mouseover="hover1=true" @mouseleave="hover1=false" :class="hover1?'border-black':'border-gray-300'">
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
        };
    }
}
</script>
