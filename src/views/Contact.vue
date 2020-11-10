<template>

    <h1> Hola soy el contacto 
        <p>  {{message}} </p>

      
    </h1>

      <Formulario/>
      <Formulario/>
      <Formulario/>

</template>

<script>

import Formulario from './../components/Formulario';


export default {

    name:'Contact',
    components: {

        Formulario
    },


    data(){

        return{
            
            message:'hola mundo',
        }
    }
    
}
</script>


<style lang='scss'>

    h1{

        color: blueviolet;

        & p {
            color: rgb(22, 71, 177);
        }
    };



</style>

