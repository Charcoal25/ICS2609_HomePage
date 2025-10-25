<template>
  <nav class="navbar">
    <div class="navbar-logo">
      🌐 <span>My Homepage</span>
    </div>
    <ul class="navbar-links">
      <li><a href="/">Home</a></li>
      <li><router-link to="/login">Log In</router-link></li>
    </ul>
  </nav>
</template>

<script>
export default {}
</script>

<style>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: linear-gradient(90deg, #2563eb, #1e3a8a);
  padding: 1rem 2rem;
  color: white;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  position: sticky;
  top: 0;
  z-index: 1000;
}

.navbar-logo {
  font-size: 1.5rem;
  font-weight: 700;
  letter-spacing: 1px;
  display: flex;
  align-items: center;
  gap: 0.4rem;
  animation: slideIn 0.8s ease-in-out;
}

.navbar-logo span {
  font-family: 'Poppins', sans-serif;
  text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.3);
}

.navbar-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
  margin: 0;
  padding: 0;
  animation: fadeIn 1s ease;
}

.navbar-links a,
.navbar-links router-link {
  color: white;
  text-decoration: none;
  font-size: 1rem;
  font-weight: 500;
  transition: color 0.3s ease;
}

.navbar-links a:hover,
.navbar-links router-link:hover {
  color: #93c5fd;
}

@keyframes slideIn {
  from { transform: translateX(-20px); opacity: 0; }
  to { transform: translateX(0); opacity: 1; }
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
</style>
