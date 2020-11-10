<template>
 
        <h1> Lista de Usuarios pintando arrays obejtos </h1>

        <li v-for="usuario in usuarios">

                {{usuario.name}}

        </li>
        
</template>

<script>
export default {
    name:'Users',
    data(){

        return{

                
                    usuarios:[], //
               

        }
    },

    methods:{

        async getInfoUsers(){
            const info = await fetch ('https://jsonplaceholder.typicode.com/users')
            const data = await info.json();

            console.log(data);
            this.usuarios = data;
        }

    },

    created(){
        this.getInfoUsers();
    }
}
</script>

<style>

</style>