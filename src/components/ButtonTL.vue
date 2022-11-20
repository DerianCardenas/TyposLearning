<template>
    <div>
        <button class="boton-vue">{{texto}}</button>
    </div>
</template>
<script>
export default {
    name:"ButtonTL",
    props:{
        texto:String
    }
}
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Baloo Da 2");
    .boton-vue{
        background-color: hsl(0, 100%, 70%);
        border:none;
        border-radius:10px;
        color:white;
        font-family: "Baloo Da 2";
        margin: .7em auto;
        padding:.5em 1em;
    }
</style>