<template>
    <div> 
        <input v-model="nome" />
        <button v-on: click="inserir"> Click </button>
    </div>
</template>
<script>
export default {
    data: function () { 
        return {
            nome: '',
        }
    },
    methods: {
        inserir : function (){
            this.nome = ''
        }
    }
}
</script>