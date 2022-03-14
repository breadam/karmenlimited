<template>
    <div>
        <img :src="image"/>
        <div class="text">
            asdasdasdasdasdsd
        </div>
    </div>
</template>
<script>
export default {
    name:'KarmenSection',
    props:["image"],
}
</script>
<style scoped>
img{
    width:196px;
}
.text{
    margin-top: 16px;
    text-align:center;
}
</style>
