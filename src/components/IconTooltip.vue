<script setup="ts">
  const props = defineProps({
    textoTooltip: {
      type: String, 
      default: 'Clique para ver mais'    
    },
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
    <a :href="props.linkRedirecionamento" style="color: black;">
      <i :class="props.classeIcone + ' icone'"/>
    </a>
    <span class="text">{{ props.textoTooltip }}</span>
  </li>
</template>

<style scoped>
  .container {
    position: relative;
    display: inline-block;
    max-width: fit-content; 
  }

  .container:hover .text {
    visibility: visible;
    opacity: 1;    
  }

  .text {
    visibility: hidden;
    width: 120px;
    background-color: var(--dark);
    color: #fff;
    text-align: center;
    padding: 5px 0;
    border-radius: 6px;
    position: absolute;
    z-index: 1;
    bottom: 125%;
    left: 50%;
    margin-left: -60px;
    opacity: 0;
    transition: opacity 0.3s;        
  }

  .icone{
    background-color: #fff;
    padding: 7px;    
    border-radius: 50%;
    box-shadow: 0px 5px 5px var(--rose);
  }

</style>