<template>
    <footer>
        <div class="cont-details">
            <p class="desc">
                Recibe notificaciones de TyposLearning para saber mas de nosotros y nuestro blog
            </p>
            <div class="mini-form">
                <input class="input" type="email" placeholder="Introduce tu correo">
                <ButtonTL class="boton" texto="Enviar"/>
            </div>
        </div>
    </footer>
</template>
<script>
import ButtonTL from '../components/ButtonTL.vue'
export default {
    name:"Footer",
    components:{
        ButtonTL
    }
}
</script>
<style scoped>
    footer{
        background-color: #E6EAF4;
        margin:1em 0;
    }
    .cont-details{
        display:flex;
        justify-content:space-around;
        margin:0 auto;
        max-width:1024px;
    }
    .desc{
        font-size:36px;
        width:60%;
    }
    .mini-form{
        margin:auto;
        width:40%;
    }
    .input{
        border:1px solid #ABB3C7;
        border-radius:5px;
        display:flex;
        height:40px;
        margin:10px auto;
        font-size:20px;
        width: 90%;
    }
    .boton{
        display:flex;
        margin:.5em auto;
        width:90%;
    }

</style>