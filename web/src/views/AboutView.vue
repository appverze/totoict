<template>
  <main class="page">
    <header class="intro">
      <h1>About totoict</h1>
      <p class="lede">
        We partner with organizations that need dependable ICT delivery—whether you are launching a new product,
        modernizing a legacy stack, or tightening day-two operations.
      </p>
    </header>

    <section class="panel" aria-labelledby="principles-heading">
      <h2 id="principles-heading">Principles</h2>
      <ul>
        <li><strong>Small batches.</strong> Frequent integration reduces risk and keeps feedback loops short.</li>
        <li><strong>Explicit contracts.</strong> APIs, SLAs, and ownership boundaries are documented and tested.</li>
        <li><strong>Operability first.</strong> Logging, metrics, and runbooks are part of the definition of done.</li>
      </ul>
    </section>

    <section class="panel muted-panel" aria-labelledby="stack-heading">
      <h2 id="stack-heading">This site</h2>
      <p>
        The totoict marketing site is a Vue 3 single-page app powered by Vite and TypeScript, with client-side routing
        via Vue Router. Run it locally with <code>npm install</code> and <code>npm run dev</code> from the
        <code>web</code> directory.
      </p>
    </section>
  </main>
</template>

<style scoped>
.page {
  padding: 2.5rem 1.25rem 3rem;
  max-width: 42rem;
  margin: 0 auto;
}

.intro {
  margin-bottom: 2rem;
}

.intro h1 {
  margin: 0 0 0.75rem;
  font-size: clamp(1.75rem, 4vw, 2.25rem);
  letter-spacing: -0.02em;
}

.lede {
  margin: 0;
  font-size: 1.05rem;
  line-height: 1.65;
  color: var(--text);
}

.panel {
  padding: 1.35rem 1.5rem;
  border-radius: 0.85rem;
  border: 1px solid var(--border);
  background: var(--surface);
  box-shadow: var(--shadow-soft);
  margin-bottom: 1rem;
}

.panel h2 {
  margin: 0 0 0.75rem;
  font-size: 1.1rem;
  color: var(--text-h);
}

.panel ul {
  margin: 0;
  padding-left: 1.15rem;
  color: var(--text);
  line-height: 1.65;
}

.panel li + li {
  margin-top: 0.5rem;
}

.muted-panel p {
  margin: 0;
  line-height: 1.65;
  color: var(--text);
}

.muted-panel code {
  font-size: 0.9em;
}
</style>
