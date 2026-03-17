<script>
   export default{
    data(){
        return{
            contador:0,
            nombre:"kjvcklvccvcv"
        }
    },

    methods:{
        saludar(){
            alert("Alerta")
        },
        incrementar(){
            this.contador++
        },
        escribir(event){
            this.nombre = event.target.value
        }
    }




   }

</script>


<template>
    <button @click="saludar">Presiona aqui</button>
    <button v-on:click="saludar">Click aqui</button>

   <p>{{ contador }}</p>
   <button @click="incrementar">Aumentar</button>

   <input @input="Escribir"  type="text" placeholder="Escribe">
   <p>Hola {{ nombre }}, como te encuentras</p>

</template>


<style>

</style>