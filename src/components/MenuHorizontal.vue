<template>
    <link href="//maxcdn.bootstrapcdn.com/font-awesome/4.1.0/css/font-awesome.min.css" rel="stylesheet">
    <div class="MainContainer">
        <div class="Container">
            <p class="TituloPage">
                <i class="fas fa-code"></i> {{ Titulo }}
            </p>
            <div class="ModulosContainer">
                <ButtonModulo Texto="Home" />
                <ButtonModulo Texto="Sobre" />
                <ButtonModulo Texto="Portifólio" />
                <ButtonModulo Texto="Contato" />

                <i class="fas fa-bell Notificacao" title="Veja as novidades"></i>
            </div>  
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ButtonModulo from './ButtonModulo.vue';

export default defineComponent({
  name: 'MenuHorizontal',
  components: {
    ButtonModulo
  },
  props: {
    Titulo: {
      type: String,
      default: "Seu Nome Aqui"
    },
  },
  
});
</script>

<style scoped>

.MainContainer{
    background: #263138;
    padding: 1.25em 5em;
    color: white;
    letter-spacing: 1px;
    box-shadow: 5px 2px 8px 3px #888888;
}

.Container{
    display: flex;
    justify-content: space-between;
    width: 90%;
    align-items: center;
}

.ModulosContainer{
    display: flex;
    gap: 4em;
    font-size: .9em;
}

.TituloPage{
    font-size: 1.1em;
    display: flex;
    align-items: center;
}

.fa-code{
    font-size: 1.4em;
    margin-right: 0.5em;
}

@keyframes ani-ring {
    50% {
        -webkit-transform: translateX(1px) rotate(4deg);
        transform: translateX(1px) rotate(4deg);
    }
    
    100% {
        -webkit-transform: translateX(-1px) rotate(-1deg);
        transform: translateX(-1px) rotate(-1deg);
    }
}

.Notificacao{
    margin-left: 2em;
    font-size: 1.3em;
    cursor: pointer;
    animation: ani-ring .2s ease infinite;
}

</style>