<template>
    <div> 
        <h2> <strong> Cadastro Pessoa </strong></h2>
    <p>        <input v-model="nome" />
        <button v-on:click= "inserir"> NOME </button> </p>
       
    </div>
</template>
<script>
export default {
    data: function () { 
        return {
            nome: ''
        }
    },
    methods: {
        inserir: function (){
            this.nome = ''
        }
    }
}
</script>