<template>
  
  <div id="app">
    
    <header>
      <div class="logo">Mazinha Fotografias
        
      </div>
      <nav>
        <a href="#servicos">Serviços</a>
        <a href="#galeria">Galeria</a>
        <a href="#contato">Contato</a>
        <a href="#agendamento">Agendamento</a>
      </nav>
    </header>
<h1>Nova versão do site publicada 🎉</h1>


    <section class="hero">
      <h1>Capturando momentos com amor e sensibilidade</h1>
      <p>Newborn | Studio | Eventos | Ensaios Externos</p>
    </section>

    <section id="servicos">
      <h2>Serviços</h2>
      <ul>
        <li>👶 Newborn</li>
        <li>📸 Ensaio em Estúdio</li>
        <li>🎉 Eventos (aniversários, casamentos, batizados, etc.)</li>
        <li>🌳 Ensaios Externos (gestantes, família, etc.)</li>
      </ul>
    </section>

    <section id="galeria">
      <h2>Galeria</h2>
      <p>Em breve, algumas fotos incríveis por aqui!</p>
    </section>

    <section id="contato">
      <h2>Contato</h2>
      <p>📲 WhatsApp:
        <a href="https://wa.me/5588999563800" target="_blank" rel="noopener">88 9 9956-3800</a>
      </p>
      <p>📷 Instagram:
        <a href="https://instagram.com/mazinhafotografa" target="_blank" rel="noopener">@mazinhafotografa</a>
      </p>
    </section>

    <section id="agendamento">
      <h2>Agende seu ensaio</h2>
      <form @submit.prevent="enviarFormulario">
        <input type="text" v-model="form.nome" placeholder="Seu nome" required />
        <input type="email" v-model="form.email" placeholder="Seu e-mail" required />
        <input type="tel" v-model="form.telefone" placeholder="Seu telefone" required />
        <select v-model="form.tipo" required>
          <option value="">Tipo de Ensaio</option>
          <option>Newborn</option>
          <option>Studio</option>
          <option>Eventos</option>
          <option>Externos</option>
        </select>
        <input type="date" v-model="form.data" required />
        <textarea v-model="form.mensagem" placeholder="Mensagem adicional"></textarea>
        <button type="submit">Enviar</button>
      </form>
    </section>

    <footer>
      <p>&copy; 2025 Mazinha Fotografias. Todos os direitos reservados.</p>
    </footer>
  </div>
</template>

<script>
import logo from '@/assets/logo3.png'

export default {
  name: 'App',
  data() {
    return {
      form: {
        nome: '',
        email: '',
        telefone: '',
        tipo: '',
        data: '',
        mensagem: ''
      },
      logo
    };
  },
  methods: {
    enviarFormulario() {
      console.log('Formulário enviado:', this.form);
      alert('Formulário enviado com sucesso!');
      // Aqui você pode integrar com um backend ou Google Forms futuramente.
    }
  }
};
</script>

<style scoped>
@import "style.css";
</style>

