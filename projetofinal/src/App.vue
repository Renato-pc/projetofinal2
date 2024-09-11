<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="logo">
            <a href="#">
              <img src="./img/logo.png" alt="">
            </a>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="navbar">
            <nav>
              <a href="#">Home</a>
              <a href="#">Sobre</a>
              <a href="#">Contato</a>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </header>
  <section class="login" id="login">
    <div class="container">
      <div class="login-box">
        <img src="./img/user.png" />
        <h1>Login</h1>
        <div class="inputs">
          <input placeholder="Insira seu e-mail" type="email">
          <input placeholder="Digite sua senha" type="password">
        </div>
        <a href="">esqueci minha senha</a>
        <button type="submit">Entrar</button>
      </div>
    </div>
  </section>
  <footer>
    <p>All Rights Reserved</p>
  </footer>
  <!-- <div class="content">

  </div>
  <div class="login-container">
    <div class="login-form">
      <img src="./img/user.png" alt="">
      <h2>Login</h2>
      <form @submit.prevent="handleSubmit">
        <div class="form-group">
          <input placeholder="Insira seu e-mail" type="email" id="email" v-model="email" required>
          <input placeholder="Digite sua senha" type="password" id="password" v-model="password" required>
          <span class="show-password" @click="showPassword = !showPassword">
            {{ showPassword ? 'Ocultar' : 'Mostrar' }}
          </span>
          <button type="submit">Entrar</button>
          <a href="#">Esqueci minha senha</a>
          <p>Não tem cadastro? <a href="#">Cadastre-se</a></p>
        </div>
      </form>
    </div>
  </div> -->
</template>

<!-- <script>
export default {
  data() {
    return {
      email: '',
      password: '',
      showPassword: false
    }
  },
  methods: {
    handleSubmit() {
      // Lógica para enviar os dados do formulário para o backend
      console.log('Email:', this.email)
      console.log('Senha:', this.password)
    }
  }
}
</script> -->

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Lato";
}

:root {
  --primary-color: #2B79C3;
  --secondary-color: #C8DFF0;
  --bg-primary-color: #FFF;
  --bg-secondary-color: #F0F0F0;
  --bg-input-color: #E4E4E4;
  --border-color: #3B4651;
  --text-dark-color: #3B4651;
  --text-light-color: #FFF;
}

header {
  background-color: var(--primary-color);
  width: 100%;
  height: 135px;
  display: flex;
  align-items: center;
}

header .navbar {
  display: flex;
  align-items: center;
  color: var(--text-dark-color);
}

header .navbar a {
  text-decoration: none;
}

#login .container {
  background-color: var(--bg-secondary-color);
  display: flex;
  justify-content: center;
  height: 80vh;
  padding: 25px;
}

#login .img1 {
  /* width: 500px; */
}

section .login-box {
  background-color: var(--secondary-color);
  border: solid 3px var(--primary-color);
  border-radius: 8px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 420px;
  padding: 40px 38px 55px;
}

section .login-box h1 {
  color: var(--primary-color);
  font-weight: 700;
  margin: 13px 0 35px;
}

section .login-box .inputs {
  display: flex;
  flex-direction: column;
  gap: 8px;
  width: 100%;
}

section .login-box input {
  height: 40px;
  background-color: var(--bg-secondary-color);
  border: solid 2px var(--border-color);
  border-radius: 8px;
  padding-left: 10px;
}

section .login-box a {
  display: flex;
  align-items: start;
  text-decoration: none;
  float: right;
}

section .login-box button {
  width: 100%;
  height: 40px;
  background-color: var(--primary-color);
  border: solid 2px var(--border-color);
  border-radius: 8px;
  color: var(--text-light-color);
}

footer {
  width: 100%;
  height: 180px;
  background-color: var(--primary-color);

}

/* Outros estilos para os elementos da página */
</style>
<!-- <template>

  <header>
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="logo">
            <a href="#">
              <img src="./img/logo.png" alt="">
            </a>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="navbar">
            <nav>
              <a href="#">Home</a>
              <a href="#">Sobre</a>
              <a href="#">Contato</a>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </header>
  <section class="login" id="login">
    <div class="container">
      <div class="login-box">
        <img src="./img/user.png" />
        <h1>Login</h1>
        <div class="inputs">
          <input placeholder="Insira seu e-mail" type="email">
          <input placeholder="Digite sua senha" type="password">
        </div>
        <a href="">esqueci minha senha</a>
        <button type="submit">Entrar</button>
      </div>
    </div>
  </section>
</template> -->
<!-- <template>
  <header>
    <img alt="Logo" class="logo" src="./img/logo.png" width="125" height="125" />
    
    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/login">Login</RouterLink>
      </nav>
    </div>
  </header>
  
  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style> -->
