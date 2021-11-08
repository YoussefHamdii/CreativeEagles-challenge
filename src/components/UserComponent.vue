<template>
    <div class="flex">
        <p>Investment Opportunities ({{items.length}})</p>
        <div class="flex pl-175">
            <div class="bg-blue-100 rounded-md">
                <img class="inline ml-3 mr-1" src="../assets/Oval.png"/>
                <span class="align-middle mr-3">Youssef Hamdi</span>
            </div>
            <img src="../assets/On.png" />
            <img src="../assets/Language.png" />
        </div>
    </div>
</template>

<script>

export default {
    name: "UserComponent",
    props:['items'],

}
</script>
