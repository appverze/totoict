<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <main class="page">
    <section class="hero">
      <p class="eyebrow">ICT that ships</p>
      <h1>Clear systems. Reliable delivery.</h1>
      <p class="lede">
        totoict helps teams design, build, and run modern digital services—from architecture and integrations to
        operations and support.
      </p>
      <div class="actions">
        <RouterLink to="/about" class="btn btn--primary">How we work</RouterLink>
        <a class="btn btn--ghost" href="mailto:hello@totoict.example">Contact</a>
      </div>
    </section>

    <section class="grid" aria-labelledby="pillars-heading">
      <h2 id="pillars-heading" class="sr-only">What we focus on</h2>
      <article class="card">
        <h3>Architecture</h3>
        <p>Pragmatic designs that balance speed, cost, and long-term maintainability.</p>
      </article>
      <article class="card">
        <h3>Engineering</h3>
        <p>Web platforms, APIs, and data pipelines built with observable, testable practices.</p>
      </article>
      <article class="card">
        <h3>Operations</h3>
        <p>Monitoring, incident response, and continuous improvement so services stay dependable.</p>
      </article>
    </section>
  </main>
</template>

<style scoped>
.page {
  padding: 2.5rem 1.25rem 3rem;
  max-width: 56rem;
  margin: 0 auto;
}

.hero {
  text-align: center;
  padding-bottom: 2.5rem;
}

.eyebrow {
  margin: 0 0 0.75rem;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--accent);
  font-weight: 600;
}

.hero h1 {
  margin: 0 0 1rem;
  font-size: clamp(2rem, 5vw, 2.75rem);
  line-height: 1.15;
  letter-spacing: -0.03em;
}

.lede {
  margin: 0 auto 1.75rem;
  max-width: 36rem;
  font-size: 1.05rem;
  line-height: 1.6;
  color: var(--text);
}

.actions {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  justify-content: center;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 0.65rem 1.15rem;
  border-radius: 0.6rem;
  font-size: 0.95rem;
  font-weight: 500;
  text-decoration: none;
  border: 1px solid transparent;
  transition:
    background 0.15s ease,
    color 0.15s ease,
    border-color 0.15s ease,
    box-shadow 0.15s ease;
}

.btn--primary {
  background: linear-gradient(135deg, var(--accent), var(--accent-2));
  color: #fff;
  box-shadow: var(--shadow-soft);
}

.btn--primary:hover {
  filter: brightness(1.05);
}

.btn--ghost {
  color: var(--text-h);
  border-color: var(--border);
  background: var(--surface);
}

.btn--ghost:hover {
  border-color: color-mix(in srgb, var(--accent) 35%, var(--border));
  background: var(--surface-2);
}

.grid {
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(15rem, 1fr));
}

.card {
  text-align: left;
  padding: 1.25rem 1.35rem;
  border-radius: 0.85rem;
  border: 1px solid var(--border);
  background: var(--surface);
  box-shadow: var(--shadow-soft);
}

.card h3 {
  margin: 0 0 0.5rem;
  font-size: 1.05rem;
  color: var(--text-h);
}

.card p {
  margin: 0;
  font-size: 0.95rem;
  line-height: 1.55;
  color: var(--text);
}

.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}
</style>
