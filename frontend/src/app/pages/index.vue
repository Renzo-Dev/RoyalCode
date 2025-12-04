<template>
  <div class="page-home">
    <section class="hero">
      <h1 class="hero-title">
        Добро пожаловать в RoyalCode
      </h1>
      <p class="hero-subtitle">
        Современное веб-приложение на Nuxt 4
      </p>
    </section>

    <section class="features">
      <h2 class="section-title">
        Возможности
      </h2>
      <div class="features-grid">
        <div class="feature-card">
          <h3>
            Vue 3
          </h3>
          <p>
            Современный фреймворк для создания интерфейсов
          </p>
        </div>
        <div class="feature-card">
          <h3>
            Nuxt 4
          </h3>
          <p>
            Мощный фреймворк для Vue с SSR и автоматическим роутингом
          </p>
        </div>
        <div class="feature-card">
          <h3>
            TypeScript
          </h3>
          <p>
            Типобезопасность и лучший DX
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">
.page-home {
  width: 100%;
}

.hero {
  text-align: center;
  padding: 4rem 0;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: #fff;
  border-radius: 8px;
  margin-bottom: 3rem;
}

.hero-title {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.25rem;
  opacity: 0.9;
}

.section-title {
  font-size: 2rem;
  margin-bottom: 2rem;
  text-align: center;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}

.feature-card {
  padding: 2rem;
  background: #f5f5f5;
  border-radius: 8px;
  transition: transform 0.3s, box-shadow 0.3s;

  &:hover {
    transform: translateY(-4px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  }

  h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: #333;
  }

  p {
    color: #666;
    line-height: 1.6;
  }
}
</style>
