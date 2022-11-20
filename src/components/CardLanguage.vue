<template>
    <div class="card">
        <div class="cont-img">
            <img class="img-logo" :src="img">
        </div>
        <div class="cont-info">
            Palabras por minuto: {{ppm}}<br/>
            Porcentaje de aciertos: {{pa}}%<br/>
            Porcentaje de errores: {{100-pa}}%<br/>
            Horas dedicadas: {{hd}}<br/>
        </div>
        <div class="cont-btn">
            <ButtonTL class="btn-tl" texto="Practicar"/>
        </div>
    </div>
</template>
<script>
import ButtonTL from '../components/ButtonTL.vue'
export default {
    name:"CardLanguage",
    components: {
        ButtonTL
    },
    props:{
        name:String,
        img:String,
        ppm:Number,
        pa:Number,
        hd:String
    }
}
</script>
<style scoped>
    .card{
        border: 1px solid #A3A3A3;
        border-radius: 20px;
        height:310px;
        padding:1em;
        width:250px;
    }
    .cont-img, .cont-info, .cont-btn{
        margin: 0 auto;
    }
    .cont-info{
        text-align: center;
    }
    .cont-img{
        height:50%;
        width:60%;
    }
    .img-logo{
        display:flex;
        height:100%;
        width:100%;
    }
    .cont-btn{
        display:flex;
        flex-flow:wrap;
        justify-content:space-around;
    }
</style>