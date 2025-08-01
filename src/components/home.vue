<template>
  <div class="home" :style="backgroundStyle">
    <header class="header">
      <img src="../assets/logo067.png" alt="Logo" class="logo" />
    </header>

    <main class="content">
      <h1>O verdadeiro sabor do Açaí</h1>
      <p>A qualidade que refresca o seu dia!</p>
      <div class="botao">
        <button class="cta-button">Peça agora</button>
      </div>
      <div class="anunciadoForca">
        <h1> A PAIXÃO PELO VERDADEIRO AÇAÍ</h1>
      </div>
    </main>

    <footer class="footer">
      <small>© 2025 Açaí Company - Todos os direitos reservados</small>
    </footer>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  computed: {
    backgroundStyle() {
      return {
        backgroundImage: "url('../assets/background.png')",
        backgroundSize: 'cover',
        backgroundPosition: 'center',
        minHeight: '100vh'
      }
    }
  }
}
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  color: white;
  text-align: center;
}

.header {
  padding: 20px;
}

.logo {
  height: 80px;
}

.content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 20px;
  padding: 20px;
}

h1 {
  font-size: 2.5rem;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.6);
}

.cta-button {
  background-color: #6a1b9a;
  color: white;
  border: none;
  padding: 15px 30px;
  font-size: 1.1rem;
  border-radius: 8px;
  cursor: pointer;
  transition: 0.3s ease;
}

.cta-button:hover {
  background-color: #8e24aa;
}

.footer {
  padding: 10px;
  background: rgba(0,0,0,0.4);
}
</style>
