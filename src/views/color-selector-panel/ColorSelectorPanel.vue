<template>
<div>

<button type="button" > TEXTO DO BOTAO </button>
<button type="button" > TEXTO DO BOTAO </button>
<button type="button" > TEXTO DO BOTAO </button>

<div class="conteudo">
texto do conteudo
</div>

</div>
</template>



<script>


export default {
 name: 'ColorSelectorPanel', 

 data() {
    return {

       cores:[{cor: 'azul',
        conteudo: 'conteudo do componente vermelho'},
        {cor: 'verde',
        conteudo: 'conteudo do componente vermelho'},
        {cor: 'vermelho',
        conteudo: 'conteudo do componente vermelho'},
        
        ]
    };
  },
}

</script>

<style scoped>
.conteudo{
    background-color: blue;
}
</style>