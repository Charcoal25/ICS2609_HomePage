<template>
  <div id="app">
    <nav class="navbar">
      <h1 class="logo">My Homepage</h1>
      <ul class="nav-links">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/login">Log In</router-link></li>
      </ul>
    </nav>
    <router-view />
  </div>
</template>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #e9f2ff;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #3b82f6;
  padding: 1rem 2rem;
}
.logo {
  color: white;
  font-size: 1.5rem;
}
.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}
.nav-links a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}
.nav-links a.router-link-active {
  text-decoration: underline;
}
</style>
