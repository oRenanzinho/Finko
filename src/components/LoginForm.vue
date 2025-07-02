<template>
  <div class="login-container">
    <img src="@/assets/perfil.png" alt="Avatar" class="avatar">
    <h2>LOGIN</h2>
    <form @submit.prevent="handleLogin">
      <input type="text" v-model="nome" placeholder="Nome de usuário">
      <input type="password" v-model="senha" placeholder="Senha">
      <div class="actions">
        <a href="#" class="esqueci-senha">Esqueceu sua senha?</a>
      </div>
      <div class="botao">
        <button type="submit">Login</button>
      </div>
    </form>
    <div class="action-regi">
      <a href="#" class="registrar-se">Ainda não tem uma conta?</a>
    </div>
  </div>
</template>

<script>
//
</script>

<style scoped>
.login-container {
  background-color: #3A4060;
  width: 350px;
  padding: 50px;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  text-align: center;
  font-family: 'Segoe UI', sans-serif;
  align-content: center;
}

h2 {
  margin-bottom: 30px;
  letter-spacing: 2px;
  color: #E0E0E0;
  font-weight: 600;
  text-transform: uppercase;
}

input {
  width: 100%;
  margin: 15px 0;
  padding: 12px 15px;
  background-color: #2F3550;
  border: 1px solid #3A4060;
  border-radius: 8px;
  color: #E0E0E0;
  font-size: 15px;
  transition: all 0.3s ease;
}

input::placeholder {
  color: #A3E4D7;
}

input:focus {
  outline: none;
  box-shadow: 0 0 10px rgba(0, 212, 168, 0.3);
  border-color: #00D4A8;
}

.botao {
  text-align: center;
  margin-top: 20px;
}

button {
  background: linear-gradient(135deg, #00D4A8 0%, #A3E4D7 100%);
  border: none;
  padding: 15px;
  width: 50%;
  border-radius: 8px;
  color: #1A252F;
  font-size: 16px;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0, 212, 168, 0.3);
}

button:hover {
  background: linear-gradient(135deg, #00D4A8 0%, #A3E4D7 100%);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(0, 212, 168, 0.4);
}

button:active {
  transform: translateY(0);
  box-shadow: 0 2px 10px rgba(0, 212, 168, 0.2);
}

.avatar {
  width: 80px;
  height: 80px;
  margin-bottom: 20px;
  border-radius: 50%;
  border: 3px solid #A3E4D7;
}

.esqueci-senha,
.registrar-se {
  color: #00D4A8;
  font-size: 14px;
  text-decoration: none;
  transition: color 0.3s ease;
}

.esqueci-senha:hover,
.registrar-se:hover {
  color: #A3E4D7;
  text-decoration: underline;
}

.actions {
  text-align: center;
  margin: 15px 0;
}

.action-regi {
  text-align: center;
  margin-top: 20px;
}
</style>