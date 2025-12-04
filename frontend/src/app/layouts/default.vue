<template>
  <div class="layout-default">
    <header class="header">
      <nav class="nav">
        <NuxtLink
          to="/"
          class="logo"
        >
          RoyalCode
        </NuxtLink>
        <div class="nav-links">
          <NuxtLink to="/">Главная</NuxtLink>
          <NuxtLink to="/about">О проекте</NuxtLink>
        </div>
      </nav>
    </header>
    <main class="main">
      <slot />
    </main>
    <footer class="footer">
      <p>&copy; {{ new Date().getFullYear() }} RoyalCode</p>
    </footer>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.layout-default {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.header {
  background: #1a1a1a;
  color: #fff;
  padding: 1rem 2rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #fff;
  text-decoration: none;
  transition: opacity 0.3s;

  &:hover {
    opacity: 0.8;
  }
}

.nav-links {
  display: flex;
  gap: 2rem;

  a {
    color: #fff;
    text-decoration: none;
    transition: opacity 0.3s;

    &:hover {
      opacity: 0.8;
    }

    &.router-link-active {
      opacity: 0.8;
      text-decoration: underline;
    }
  }
}

.main {
  flex: 1;
  padding: 2rem;
  max-width: 1200px;
  width: 100%;
  margin: 0 auto;
}

.footer {
  background: #1a1a1a;
  color: #fff;
  text-align: center;
  padding: 1.5rem;
  margin-top: auto;
}
</style>
