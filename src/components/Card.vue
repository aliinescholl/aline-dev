<script setup="ts">
import IconTooltip from '../components/IconTooltip.vue';

const props = defineProps({
    descricao: {
      type: String, 
      default: 'Clique para ver mais'    
    },
    caminhoImagem: {
        type: String,
        default: "./assets/midia/images/avestruz.jpg"
    },
    titulo: {
        type: String,
        default: "Avestruz"
    }
  })

</script>

<template>
    <div class="card">
        <div style="width: 100%; height: 100%;">
            <img :src="props.caminhoImagem" alt="imagem do projeto" style="max-height: 120px; max-width: 350px; border-radius: 10%;">
            <h1 class="centralize">{{ props.titulo }}</h1>
            <p style="font-size: small;">{{ props.descricao }}</p>
            
            <div style="display: flex; width: 100%; gap: 5px; justify-content: center;">
                <IconTooltip
                    classe-icone="fa-brands fa-github"
                    link-redirecionamento="https://github.com/aliinescholl/aline-dev"
                />
                <IconTooltip
                    classe-icone="fa-solid fa-code"
                    link-redirecionamento="https://github.com/aliinescholl/aline-dev"
                />
            </div>
        </div>
    </div>
</template>

<style>
@media (min-width: 425px) {
    .card {
        height: 500px; 
        width: 380px; 
        background-color: var(--white-rose2); 
        border-radius: 10%; 
        align-items: center; 
        display: flex; 
        flex-direction: column; 
        padding: 10px;
        box-shadow: 5px 5px 20px rgb(44, 0, 73);
    }
}
</style>