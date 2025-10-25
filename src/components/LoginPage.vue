<template>
  <div class="login-wrapper">
    <div class="login-box">
      <h2 class="login-title">Log In</h2>
      <form @submit.prevent="login">
        <input type="text" placeholder="Username" v-model="username" required />
        <input type="password" placeholder="Password" v-model="password" required />
        <button type="submit">Sign In</button>
      </form>
      <p class="note">Don’t have an account yet? <a href="#">Sign up here</a></p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    login() {
      if (this.username && this.password) {
        alert(`Welcome, ${this.username}!`)
      } else {
        alert('Please enter both username and password.')
      }
    }
  }
}
</script>

<style>
.login-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
  background: linear-gradient(135deg, #3b82f6, #1e40af);
}

.login-box {
  background: rgba(255, 255, 255, 0.9);
  padding: 2.5rem;
  border-radius: 20px;
  width: 340px;
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
  text-align: center;
  animation: fadeIn 0.8s ease-in-out;
}

.login-title {
  font-size: 2rem;
  color: #1e3a8a;
  margin-bottom: 1.5rem;
  font-weight: bold;
}

input {
  display: block;
  width: 100%;
  padding: 0.7rem;
  margin-bottom: 1rem;
  border: 1px solid #cbd5e1;
  border-radius: 8px;
  font-size: 1rem;
  outline: none;
}

input:focus {
  border-color: #3b82f6;
  box-shadow: 0 0 5px rgba(59, 130, 246, 0.5);
}

button {
  width: 100%;
  padding: 0.7rem;
  background-color: #3b82f6;
  color: white;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1rem;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #2563eb;
}

.note {
  margin-top: 1rem;
  font-size: 0.9rem;
  color: #334155;
}

.note a {
  color: #1d4ed8;
  text-decoration: none;
  font-weight: bold;
}

.note a:hover {
  text-decoration: underline;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(-15px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>
