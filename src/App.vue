<template>
  <div id="app">
    <header>
      <img alt="Mazinha Fotografias" src="./assets/logo3.png" class="logo" />
      <h1>Mazinha Fotografias</h1>
      <p>25 anos registrando emoções</p>
    </header>

    <section class="galeria">
      <h2>Ensaios Recentes</h2>
      <div class="imagens">
        <img src="./assets/logo.png" alt="Ensaio Newborn" />
        <img src="./assets/logo01.png" alt="Evento" />
        <img src="./assets/logo2.jpeg" alt="Ensaio Externo" />
      </div>
    </section>

    <section class="contato">
      <a
        href="https://wa.me/5588999563800"
        target="_blank"
        class="botao-whatsapp"
      >
        📲 Agende seu ensaio agora!
      </a>
      <p>
        📸 Instagram:
        <a href="https://instagram.com/mazinhafotografa" target="_blank">
          @mazinhafotografa
        </a>
        <br />
        ✉️ Email: <a href="mailto:mazinhaartcores@gmail.com">mazinhaartcores@gmail.com</a>
      </p>
    </section>

    <footer>
      <p>&copy; 2025 Mazinha Fotografias - Todos os direitos reservados.</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
body {
  margin: 0;
  font-family: 'Helvetica Neue', sans-serif;
  background-color: #0c2340; /* Azul egípcio */
  color: #fcd116; /* Dourado */
}

#app {
  text-align: center;
  padding-bottom: 40px;
}

header {
  background-color: #08182b;
  padding: 2rem;
}

.logo {
  width: 120px;
  margin-bottom: 1rem;
}

h1 {
  margin: 0;
  font-size: 2.5rem;
}

h2 {
  font-size: 2rem;
  margin-bottom: 1rem;
}

.galeria {
  padding: 2rem;
}

.imagens {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
}

.imagens img {
  max-width: 300px;
  border: 4px solid #fcd116;
  border-radius: 12px;
}

.contato {
  margin-top: 3rem;
}

.botao-whatsapp {
  display: inline-block;
  padding: 12px 24px;
  background-color: #fcd116;
  color: #0c2340;
  font-weight: bold;
  border-radius: 8px;
  text-decoration: none;
  margin-bottom: 1rem;
}

footer {
  background-color: #08182b;
  padding: 1rem;
  font-size: 0.9rem;
}
</style>
