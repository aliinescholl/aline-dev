<script setup>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
import Card from './components/Card.vue';
import IconTooltip from './components/IconTooltip.vue';

</script>

<template>
  <header class="header">
    <NavBar />
  </header>

  <main style="width: 100%;">
    <section class="centralize" style="width: 100vw;">
      <div class="container">
        <div class="d-flex" style="margin-top: 30px;">
          <img 
            class="profile-image"
            src="https://avatars.githubusercontent.com/u/76217058?v=4" 
            alt="Foto perfil do GitHub" 
          />
          <div class="centralize" style="align-items: center; flex-direction: column;">
            <h1 style="color: var(--rose2)">Aline Scholl Santos</h1>
            <h2 style="color: var(--rose2)">Desenvolvedora Full Stack</h2>
            <p style="color: var(--light-rose)">Transformando ideias em soluções com código, café e paixão por tecnologia.</p> 
            <div class="d-flex" style="gap: 2vw; margin-top: 10px;"> 
              <IconTooltip
                classe-icone="fa-brands fa-linkedin"
                link-redirecionamento="https://www.linkedin.com/in/aliinescholl"
              />

              <IconTooltip
                classe-icone="fa-brands fa-github"
                link-redirecionamento="https://github.com/aliinescholl"
              />
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

      <div style="display: flex; align-items: center; flex-direction: column;">
        <Card></Card>
        <br>
        <Card></Card>
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

  @media (min-width: 425px) {
    .header{
      box-shadow: 5px 5px 20px rgb(44, 0, 73);
    }

    .profile-image {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      box-shadow: 5px 5px 30px rgb(44, 0, 73);
    }

    .container>div {
      flex-direction: column;
      align-items: center;

      h1 {
        font-size: 2rem;
      }
      
      h2 {
        font-size: 1rem;
        margin-bottom: 8px;
      }

      p {
        font-size: 0.8rem;
        text-align: center;
        margin-bottom: 6px;
        margin-top: 12px;
      }

      img {
        margin-bottom: 15px;
      }
    }
  }

</style>
