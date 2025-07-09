<script setup>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
import IconTooltip from './components/IconTooltip.vue';

</script>

<template>
  <header class="header">
    <NavBar />
  </header>

  <main style="width: 100%;">
    <section class="centralize" style="width: 100vw;">
      <div class="container centralize">
        <div class="d-flex" style="gap: 40px; margin-top: 30px;">
          <img 
            class="profile-image"
            src="https://avatars.githubusercontent.com/u/76217058?v=4" 
            alt="Foto perfil do GitHub" 
          />
          <div class="centralize" style="align-items: center; flex-direction: column;">
            <h1 style="color: var(--rose2)">👩‍💻 Aline Scholl Santos — Desenvolvedora Full Stack</h1>
            <p style="color: var(--light-rose)">Transformando ideias em soluções com código, café e paixão por tecnologia.</p> 
            <div class="d-flex" style="gap: 1vw; margin-top: 10px;">
              <button style="background-color: var(--rose2); border: none; font-size: medium; padding: 10px; color: var(--white-rose); border-radius: 5px;">Entre em contato</button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <hr style="margin: 20px 50px 10px 50px">
    <section class="centralize" style="width: 100vw;  display: flex; flex-direction: column;">  
      <div class="centralize">
        <h1 style="color: var(--rose2); padding-bottom: 10px;">Meus projetos</h1>
      </div>

      <div class="centralize" style="align-items: center; gap: 20px;">
        
        <div style="height: 300px; width: 200px; background-color: var(--white-rose2); border-radius: 10%; align-items: center; display: flex; flex-direction: column; padding: 10px;">
          <div style="width: 100%; height: 100%;">
            <img src="././assets/midia/images/avestruz.jpg" alt="avestruz" style="max-height: 120px; max-width: 190px; border-radius: 10%;">
            <h1 class="centralize">Título projeto</h1>
            <p style="font-size: small;">Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero eos eligendi, optio doloribus dignissimos alias nulla distinctio officia </p>
            
            <div style="display: flex; width: 100%; gap: 5px; justify-content: center;">
              <IconTooltip
                texto-tooltip="GitHub"
                classe-icone="fa-brands fa-github"
                link-redirecionamento="https://github.com/aliinescholl/aline-dev"
              />
              <IconTooltip
                texto-tooltip="Deploy"
                classe-icone="fa-solid fa-code"
                link-redirecionamento="https://github.com/aliinescholl/aline-dev"
              />
            </div>
            
          </div>
        </div>

       <div style="height: 300px; width: 200px; background-color: var(--white-rose2); border-radius: 10%; align-items: center; display: flex; flex-direction: column; padding: 10px;">
          <div style="width: 100%; height: 100%;">
            <img src="././assets/midia/images/avestruz.jpg" alt="avestruz" style="max-height: 120px; max-width: 190px; border-radius: 10%;">
            <h1 class="centralize">Título projeto</h1>
            <p style="font-size: small;">Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero eos eligendi, optio doloribus dignissimos alias nulla distinctio officia </p>
            
            <div style="display: flex;">
              <IconTooltip
                texto-tooltip="GitHub"
                classe-icone="fa-brands fa-github"
              />
  
              <IconTooltip
                texto-tooltip="Deploy"
                classe-icone="fa-solid fa-code"
              />
            </div>            
          </div>
        </div>
      </div>
    </section>

    <!-- <section>sobre</section> -->
    <!-- <section>contatos</section> -->
  </main>

  <footer>
    <Footer />
  </footer>
</template>

<style scoped>
  .header {
    height: 8vh;
    background-color: #1a181a;
  }

  .profile-image {
    width: 250px;
    height: 250px;
    border-radius: 50%;
    box-shadow: 5px 5px 30px white;
  }

  .footer {
    height: 8vh;    
  }

  .container {
    width: 80vw;
  }

  .centralize {
    display: flex; 
    justify-content: center;
  }

</style>
