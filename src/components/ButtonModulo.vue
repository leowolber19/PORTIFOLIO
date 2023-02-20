<template>
    <p class="TextoButton"> {{Texto}} </p>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ButtonModulo',
  props: {
    Texto: {
      type: String,
      default: "Home"
    },
  },
  
});
</script>

<style scoped>

.TextoButton{
    cursor: pointer;
}

.TextoButton:hover{
    padding-top: -2px;
}

</style>