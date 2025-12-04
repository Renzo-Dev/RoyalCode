<template>
  <div class="page-about">
    <h1 class="page-title">
      О проекте
    </h1>
    <div class="content">
      <section class="info-section">
        <h2>RoyalCode</h2>
        <p>
          Современное веб-приложение, построенное на стеке Nuxt 4, Vue 3 и TypeScript.
        </p>
        <p>
          Проект использует лучшие практики разработки и современные технологии
          для создания масштабируемых и производительных приложений.
        </p>
      </section>

      <section class="tech-section">
        <h2>Технологии</h2>
        <ul class="tech-list">
          <li>Nuxt 4</li>
          <li>Vue 3</li>
          <li>TypeScript</li>
          <li>SCSS</li>
          <li>Docker</li>
          <li>Nginx</li>
        </ul>
      </section>
    </div>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.page-about {
  max-width: 800px;
  margin: 0 auto;
}

.page-title {
  font-size: 2.5rem;
  margin-bottom: 2rem;
  text-align: center;
}

.content {
  display: flex;
  flex-direction: column;
  gap: 3rem;
}

.info-section,
.tech-section {
  padding: 2rem;
  background: #f5f5f5;
  border-radius: 8px;

  h2 {
    font-size: 1.75rem;
    margin-bottom: 1rem;
    color: #333;
  }

  p {
    line-height: 1.8;
    color: #666;
    margin-bottom: 1rem;
  }
}

.tech-list {
  list-style: none;
  padding: 0;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1rem;

  li {
    padding: 1rem;
    background: #fff;
    border-radius: 4px;
    text-align: center;
    font-weight: 500;
    color: #333;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
  }
}
</style>
