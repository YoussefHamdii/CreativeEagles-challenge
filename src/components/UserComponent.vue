<template>
    <div class="flex flex-row justify-between">
        <p>Investment Opportunities ({{items.length}})</p>
        <div class="flex flex-row justify-end mr-2">
            <div class="bg-blue-100 rounded-md mr-2">
                <img class="inline ml-3 mr-1" src="../assets/Oval.png"/>
                <span class="align-middle mr-3">Youssef Hamdi</span>
            </div>
            <img src="../assets/On.png" class="mr-2" />
            <img src="../assets/Language.png" class="mr-2" />
        </div>
    </div>
</template>

<script>

export default {
    name: "UserComponent",
    props:['items'],

}
</script>
