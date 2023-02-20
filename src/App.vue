<template>
  <link href='https://fonts.googleapis.com/css?family=Roboto' rel='stylesheet'>
  <MenuHorizontal Titulo="Leonardo Wolber da Mota" />
  <PageHome />
  <PageFooter Creditos="Desenvolvido por Leonardo Wolber da Mota" />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import MenuHorizontal from './components/MenuHorizontal.vue';
import PageHome from './components/PageHome.vue';
import PageFooter from './components/PageFooter.vue';

export default defineComponent({
  name: 'App',
  components: {
    MenuHorizontal,
    PageHome,
    PageFooter
  }
});
</script>

<style>

body {
    margin: 0;
    background: #f6f6f6;
}

p {
  margin: 0;
  font-family: roboto;
}

</style>
