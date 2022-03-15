<template>
    <a :href="link">
        <div class="section">
            <img class="logo" :src="image"/>
            <h2 class="title">
                {{title}}
            </h2>
            <h5 class="subtitle">
                {{subtitle}}
            </h5>
            <!--<div>
                <button>Visit</button>
            </div>-->
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
}

.logo{
    transition:1s all;
    width:216px;
    margin-bottom: 32px;
    border-radius:50%;
}

.section:hover .logo{
    box-shadow:0px 2px 6px #333;
    transform: translate(0px,-12px);
}

.title{
    color:#444;
    margin:0px;
}

.subtitle{
    color:#666;
    margin-top:2px;
}

button{
    padding:8px 48px;
    font-family: inherit;
}

</style>
