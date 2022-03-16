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
            <div>
                <button>{{$t('visit')}}</button>
            </div>
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
    width:216px;
    margin-bottom: 32px;
    border-radius:50%;

    transition:1s all;
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
    width:100%;
    padding:8px 48px;
    font-family: inherit;
    border:none;
    border-radius:2px;
    background-color:inherit;
    background-color: rgb(214,233,216);
    opacity:0;
    transition:1s all;
    cursor:pointer;
}

button:hover{
    background-color: rgba(194,213,196,1);
}

.section:hover button{
    opacity:1;
    box-shadow:0px 2px 3px #333;
    transform:translateY(-4px);
}

</style>
