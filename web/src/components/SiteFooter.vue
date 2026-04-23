<script setup lang="ts">
const year = new Date().getFullYear()
</script>

<template>
  <footer class="site-footer">
    <p class="muted">© {{ year }} totoict. Built with Vue 3 & Vite.</p>
  </footer>
</template>

<style scoped>
.site-footer {
  margin-top: auto;
  padding: 1.5rem 1.25rem;
  border-top: 1px solid var(--border);
  text-align: center;
}

.muted {
  margin: 0;
  font-size: 0.875rem;
  color: var(--text-muted);
}
</style>
