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

  <main style="width: 100vw;">
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

    <section style="width: 100vw; flex-direction: column;" class="centralize">
      <h1 style="color: var(--rose2); text-align: center; margin-bottom: 1rem;">Competências</h1>
       <div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: center;">
        <div class="tag">C#</div>
        <div class="tag">Asp .Net</div>
        <div class="tag">Entity Framework</div>
        <div class="tag">Quartz</div>
        <div class="tag">Git</div>
        <div class="tag">GitHub</div>
        <div class="tag">HTML</div>
        <div class="tag">Vue Js</div>
        <div class="tag">JavaScript</div>
        <div class="tag">TypeScript</div>
        <div class="tag">Scrum</div>
        <div class="tag">KanBan</div>
        <div class="tag">PostgreSql</div>
        <div class="tag">Vuetify</div>
        <div class="tag">CSS</div>
        <div class="tag">BootStrap</div>
        <div class="tag">SQL</div>
        <div class="tag">Metodologias ágeis</div>
        <div class="tag">Delphi</div>
        <div class="tag">Unigui</div>
      </div>
    </section>

    <hr style="margin: 20px 50px 10px 50px">
    <section style="width: 100vw;">  
      <div>
        <h1 style="color: var(--rose2); padding-bottom: 10px; text-align: center;">Meus projetos</h1>
      </div>

      <div style="display: flex; align-items: center; flex-direction: column;">
        <Card></Card>
        <br>
        <Card></Card>
      </div>
    </section>

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

  .tag{
    padding: 5px;
    background-color: var(--light-rose);
    border-radius: 15px;
    color: rgb(44, 0, 73);
    box-shadow: 5px 5px 20px rgb(83, 15, 128);
    font-size: 1rem;
    white-space: nowrap;
  }

  @media (min-width: 425px) {
    .header{
      box-shadow: 5px 5px 10px rgb(44, 0, 73);
    }

    .profile-image {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      box-shadow: 5px 5px 30px ;
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
