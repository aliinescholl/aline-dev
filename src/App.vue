<script setup lang="ts">
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
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
            alt="imagem" 
          />
          <div class="centralize" style="align-items: center; flex-direction: column;">
            <h1 style="color: var(--rose2)">👩‍💻 Aline Scholl Santos — Desenvolvedora Full Stack</h1>
            <p style="color: var(--light-rose)">Transformando ideias em soluções com código, café e paixão por tecnologia.</p> 
            <div class="d-flex" style="gap: 1vw; margin-top: 10px;">
              <button>Entre em contato</button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <hr style="margin: 20px 50px 10px 50px">
    <section class="centralize" style="width: 100vw;">  
      <div>
        <h1 style="color: var(--rose2)">Quem sou eu?</h1>
      </div>
    </section>

    <section></section>
    <section></section>
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
