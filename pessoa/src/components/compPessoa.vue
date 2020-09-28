<template>
    <div> 
        <h2> <strong> Cadastro Pessoa </strong></h2>
    <p> <input v-model="nome" />
        <button v-on:click= "inserir"> NOME </button> </p>
        <p> {{nome}} </p>
        
        <p> <input v-model="idade" />
        <button v-on:click= "inserir"> IDADE </button> </p>
        <p> {{idade}} </p>

        <p> <input v-model="residencia" />
        <button v-on:click= "inserir"> RESIDENCIA </button> </p>
        <p> {{residencia}} </p>

        <p> <input v-model="estado_civil" />
        <button v-on:click= "inserir"> ESTADO </button> </p>
        <p> {{estado_civil}} </p>
    </div>
   
</template>
<script>
export default {
    data: function () { 
        return {
            nome: '',
            idade: '',
            residencia: '',
            estado_civil: ''
        }
    },
    methods: {
        inserir: function (){
            this.nome = ''
            this.idade=''
            this.residencia= ''
            this.estado_civil=''
            
        }
    }
}
</script>