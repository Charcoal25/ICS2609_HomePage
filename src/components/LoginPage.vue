<template>
  <div class="login-container">
    <h2>Log In</h2>
    <form @submit.prevent="login">
      <input type="text" placeholder="Username" v-model="username" required />
      <input type="password" placeholder="Password" v-model="password" required />
      <button type="submit">Submit</button>
    </form>
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
      alert(`Welcome, ${this.username}!`)
    }
  }
}
</script>

<style>
.login-container {
  max-width: 350px;
  margin: 5rem auto;
  background: white;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  text-align: center;
}
input {
  display: block;
  width: 100%;
  padding: 0.5rem;
  margin-bottom: 1rem;
}
button {
  background-color: #3b82f6;
  color: white;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
}
</style>
