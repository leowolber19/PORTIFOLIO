<template>
  <div class="ContainerMainHome">
    <div class="ContainerHome">
      <div>
        <p class="HomeTextoBottom"> Olá pessoas, </p>
        <p class="HomeNegrito"> EU SOU UM </p> 
        <p class="HomeNegrito"> PROGRAMADOR </p>
        <p class="HomeTextoTop"> Seja bem-vindo ao meu portifólio website </p>

        <div class="ButtonSaibaMais"> Saiba mais sobre mim </div>
      </div>
      <img src="../assets/imagem-home.png" style="height: 26em;">
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'PageHome',
});
</script>

<style scoped>

.ContainerHome{
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 65%;
}

.HomeNegrito {
  font-size: 3em;
  font-weight: bolder;
  color: #263138;
  font-family: system-ui;
}

.HomeTextoBottom {
  font-size: 1.6em;
  color: #263138;
  margin-bottom: 0.5em;
}


.HomeTextoTop {
  font-size: 1.6em;
  color: #263138;
  margin-top: 0.5em;
}

.ContainerMainHome{
  display: flex;
  justify-content: center;
  height: calc(100vh - 160px);
}

.ButtonSaibaMais{
  margin-top: 3em;
  background: #263138;
  padding: 0.5em 0.5em 0.7em;
  border-radius: 10px;
  color: white;
  text-align: center;
  width: 50%;
  font-weight: 600;
  font-family: system-ui;
  box-shadow: 0px 2px 10px -1px #888888;
  cursor: pointer;
  transition: .2s;
}

.ButtonSaibaMais:hover{
  background: #2b353ceb;
}

</style>
