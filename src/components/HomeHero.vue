<template>
  <section class="home">
    <div class="hero-content">
      <h1 class="hero-title">Welcome to My Homepage</h1>
      <p class="hero-subtitle">
        Explore the features and click <strong>Log In</strong> on the navigation bar to continue.
      </p>
      <div class="hero-line"></div>
    </div>
  </section>
</template>

<style>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
  background: linear-gradient(135deg, #93c5fd, #3b82f6);
  color: white;
  text-align: center;
}

.hero-content {
  max-width: 700px;
  padding: 2rem;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 20px;
  backdrop-filter: blur(10px);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.hero-title {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1rem;
  text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.3);
}

.hero-subtitle {
  font-size: 1.3rem;
  line-height: 1.6;
  color: #f0f9ff;
}

.hero-line {
  width: 80px;
  height: 4px;
  background-color: #ffffff;
  margin: 2rem auto 0;
  border-radius: 2px;
}
</style>
