<template>
    <div> 
        <h2> <strong> Cadastro Pessoa </strong></h2>
    <p> <input v-model="nome" />
        <button v-on:click= "inserir"> NOME </button> </p>
        
         <div>
             
        </div>    
    </div>
   
</template>
<script>
export default {
    data: function () { 
        return {
            nomes: ''
        }
    },
    methods: {
        inserir: function (){
            this.nome.push(this.nome)
        }
    }
}
</script>