<template>
<div class="panel">

<button type="button" @click="corSelecionada= 'Vermelho'"> CARREGAR COMPONENTE VERMELHO </button>
<button type="button" @click="corSelecionada= 'Verde'"> CARREGAR COMPONENTE VERDE </button>
<button type="button" @click="corSelecionada= 'Azul'"> CARREGAR COMPONENTE AZUL </button>

<component :is="corSelecionada" >
<span slot="conteudo">Conteúdo do Componente <strong>{{ corSelecionada }}</strong></span>
</component>

</div>
</template>



<script>
import SelectedColor from './components/SelectedColor.vue'
import Azul from './components/Azul.vue'
import Verde from './components/Verde.vue'
import Vermelho from './components/Vermelho.vue'

export default {
 name: 'ColorSelectorPanel', 
components: {SelectedColor, Azul, Verde, Vermelho},
 data() {
    return {
        corSelecionada: '',
       
    };
  },
}

</script>

<style scoped>
    .caixa {
        color: #FFF;
        font-size: 1.8rem;
        padding: 25px;
		margin: 10px 0px;
    }

	.vermelho {
        border: 2px solid red;
        background-color: #f54235;
    }

	.verde {
        border: 2px solid green;
        background-color: #49b057;
    }

	.azul {
        border: 2px solid blue;
        background-color: #2594f0;
    }
</style>