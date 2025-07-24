<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<main class="app-container">
  {@render children()}
</main>

<style>
  .app-container {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    width: 100%;
    max-width: 560px;
    margin: 0 auto;
    padding: 1rem;
    box-sizing: border-box;
    background: var(--background, #fff);
  }

  @media (min-width: 600px) {
    .app-container {
      padding: 2rem;
    }
  }
</style>