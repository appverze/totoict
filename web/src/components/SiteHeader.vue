<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <header class="site-header">
    <RouterLink to="/" class="brand" aria-label="totoict home">
      <span class="brand-mark" aria-hidden="true" />
      <span class="brand-text">totoict</span>
    </RouterLink>
    <nav class="nav" aria-label="Primary">
      <RouterLink to="/" class="nav-link" active-class="nav-link--active" exact-active-class="nav-link--active">
        Home
      </RouterLink>
      <RouterLink to="/about" class="nav-link" active-class="nav-link--active">About</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
.site-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
  padding: 1rem 1.25rem;
  border-bottom: 1px solid var(--border);
  background: color-mix(in srgb, var(--bg) 88%, transparent);
  backdrop-filter: blur(10px);
  position: sticky;
  top: 0;
  z-index: 10;
}

.brand {
  display: inline-flex;
  align-items: center;
  gap: 0.65rem;
  text-decoration: none;
  color: var(--text-h);
  font-weight: 600;
  letter-spacing: -0.02em;
}

.brand-mark {
  width: 2rem;
  height: 2rem;
  border-radius: 0.5rem;
  background: linear-gradient(135deg, var(--accent), var(--accent-2));
  box-shadow: var(--shadow-soft);
}

.brand-text {
  font-size: 1.125rem;
}

.nav {
  display: flex;
  gap: 0.25rem;
}

.nav-link {
  color: var(--text);
  text-decoration: none;
  padding: 0.5rem 0.85rem;
  border-radius: 0.5rem;
  font-size: 0.95rem;
  transition:
    color 0.15s ease,
    background 0.15s ease;
}

.nav-link:hover {
  color: var(--text-h);
  background: var(--surface-2);
}

.nav-link--active {
  color: var(--text-h);
  background: var(--surface-2);
}
</style>
