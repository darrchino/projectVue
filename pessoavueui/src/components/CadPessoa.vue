<template>
    <div id="pessoa">
            <h2><strong>Cadastro de Pessoas</strong></h2>

      <p><input v-model="nome" placeholder="Digite o nome:">
        <button v-on:click="inserir">Nome</button></p>
        <p>O seu nome e: {{nome}} .</p>
        <p><input v-model="idade" placeholder="Digite a idade">
        <button v-on:click="inserir">Idade</button></p>
        <p>Voce tem {{idade}} de idade.</p>
        <p><input v-model="residencia" placeholder="Digite a residencia">
        <button v-on:click="inserir">Residencia</button></p>
        <p>Voce vive em {{residencia}} .</p>
        <p><input v-model="estado_civil" placeholder="Digite o estado civil">
        <button v-on:click="inserir">Estado Civil</button></p>
        <p>Voce e {{estado_civil}} .</p>
    </div>
</template>

<script>
export default {
    props:{
        nome: String,
        idade: Number,
        residencia: String,
        estado_civil: String,
        pessoa: Object
    },
    methods: {
        inserir: function(){
            this.nome = ''
            this.idade = ''
            this.residencia = ''
            this.estado_civil = ''
        }
    }
}
</script>
<style scoped>
    #pessoa{
        text-align: inherit;
        background: grey;
        

    }

</style>