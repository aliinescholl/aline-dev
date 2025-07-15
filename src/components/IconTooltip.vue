<script setup="ts">
  const props = defineProps({
    classeIcone: {
      type: String,
      default: 'fa-solid fa-code',
    },
    linkRedirecionamento: {
      type: String,
    }
  })

</script>

<template>
  <li class="container">
    <a :href="props.linkRedirecionamento" target="_blank" style="color: black;">
      <i :class="props.classeIcone + ' icone'" />
    </a>
  </li>
</template>

<style scoped>
  .container {
    position: relative;
    display: inline-block;
    max-width: fit-content; 
  }

  .icone{
    background-color: #fff;
    padding: 7px;    
    border-radius: 50%;
    box-shadow: 0px 5px 5px var(--rose);
  }

</style>