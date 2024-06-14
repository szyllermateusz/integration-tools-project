<template>
  <div>
    <header class="header">
      <nav class="navbar">
        <div class="logo">Integrations Tools</div>
      </nav>
    </header>
    <main class="main-content">
      <section class="intro">
        <h1>Welcome to Integrations Tools</h1>
        <p>Find tools dedicated for Customer Success.</p>
      </section>
      <section class="tools">
        <div class="tool-card">
          <h2>Bookings Checker</h2>
          <p>Check and manage integration with ease.</p>
          <button @click="goToBookingsChecker">Learn More</button>
        </div>
        <div class="tool-card">
          <h2>Queues Checker</h2>
          <p>Monitor integration queues effectively.</p>
          <button @click="goToQueueChecker">Learn More</button>
        </div>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: 'IntegrationTools.vue',
  methods: {
  goToBookingsChecker() {
    window.location.href = 'https://www.znanylekarz.pl/integrations-tools/bookings-checker/search#/';
  },
  goToQueueChecker() {
    window.location.href = 'https://www.znanylekarz.pl/integrations-tools/alerting-system/queues-checker#/'
  }
}
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

body {
  font-family: 'Roboto', sans-serif;
  line-height: 1.6;
  color: #333;
  background-color: #f9f9f9;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  margin: 0;
}

.header {
  background-color: #00b39b;
  color: #fff;
  padding: 1rem 2rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: 700;
  margin: auto;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  font-weight: 500;
}

.main-content {
  flex: 1;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.intro {
  margin-bottom: 3rem;
}

.intro h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.intro p {
  font-size: 1.2rem;
  color: #666;
}

.tools {
  display: flex;
  gap: 2rem;
}

.tool-card {
  background: #fff;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.05);
  width: 300px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.tool-card h2 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.tool-card p {
  font-size: 1rem;
  color: #666;
  margin-bottom: 1.5rem;
}

.tool-card button {
  background-color: #3d83df;
  color: #fff;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1rem;
  transition: background-color 0.3s ease;
}

.tool-card button:hover {
  background-color: #316ac5;
}

.tool-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
}

.footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 1rem;
  position: relative;
  bottom: 0;
  width: 100%;
}
</style>
