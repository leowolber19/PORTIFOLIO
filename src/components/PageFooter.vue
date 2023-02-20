<template>
    <div class="ContainerMainFooter">
        <div class="ContainerFooter">
            <div class="ContainerLinks">
            <i class="fab fa-github"></i>
            <i class="fab fa-linkedin-in"></i>
            <i class="fab fa-instagram"></i>
            </div>
            <div class="ContainerCreditos"> {{ Creditos }} </div>
        </div>
    </div>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    name: 'PageHFooter',
    props:{
        Creditos: {
            type: String,
            default: "Seus Créditos"
        }
    },
  });
  </script>

<style scoped>

.ContainerMainFooter{
    display: flex;
    justify-content: center;
}

.ContainerFooter{
    display: flex;
    justify-content: space-between;
    width: 65%;
}

.ContainerLinks{
    display: flex;
    gap: 1em;
    font-size: 1.8em;
    color: #263138;
}

.ContainerCreditos{
    font-size: .9em;
    color: #263138;
    font-family: 'Roboto';
}

</style>