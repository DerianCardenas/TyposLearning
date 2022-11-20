<script>
import CardLanguage from '../components/CardLanguage.vue'
export default {
    name:"DashboardUser",
    components:{
        CardLanguage
    },
    data(){
        return{
            lenguajes:[
                {name:"C++",img:"https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/1822px-ISO_C%2B%2B_Logo.svg.png",ppm:75,pa:80,hd:"01:25"},
                {name:"Python",img:"https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/640px-Python-logo-notext.svg.png",ppm:75,pa:80,hd:"01:25"},
                {name:"Java",img:"https://www.manualweb.net/img/logos/java.png",ppm:75,pa:80,hd:"01:25"},
                {name:"JavaScript",img:"https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/1200px-Unofficial_JavaScript_logo_2.svg.png",ppm:75,pa:80,hd:"01:25"}
            ]
        }
    }
}
</script>
<template>
    <div class="cont-dashboard">
        <div class="container-languages">
            <div class="language" v-for="(lenguaje) of lenguajes" :key="lenguaje">
                <CardLanguage
                    :name="lenguaje.name"
                    :img="lenguaje.img"
                    :ppm="lenguaje.ppm"
                    :pa="lenguaje.pa"
                    :hd="lenguaje.hd"
                    />
            </div>
        </div>
    </div>
</template>
<style scoped>
    .container-languages{
        display:flex;
        flex-flow:wrap;
        justify-content:space-around;
        margin: 1em auto;
        margin-bottom: 0;
        width:90%;
    }
    .language{
        margin: 1em auto;
        width: auto;
    }
</style>