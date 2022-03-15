<template>
    <a :href="link">
        <div class="section">
            <img :src="image"/>
            <h2 class="title">
                {{title}}
            </h2>
            <h5 class="subtitle">
                {{subtitle}}
            </h5>
        </div>
    </a>
</template>
<script>
export default {
    name:'KarmenSection',
    props:['link','image','title','subtitle'],
}
</script>
<style scoped>

a,a:visited,a:hover, a:focus, a:active{
    text-decoration: none;
    color:inherit;
}

.section{
    text-align:center;
    max-width:256px;
    padding:48px;
    background-color:rgb(248,247,239);
    border-radius:4px;
    transition:1s all;
}

.section:hover{
    box-shadow:0px 2px 4px #333;
    transform: translate(0px,-4px);
}

.title{
    color:#333;
    margin:0px;
}

.subtitle{
    color:#555;
    margin-top:2px;
}

img{
    width:196px;
    margin-bottom: 32px;
}

</style>
