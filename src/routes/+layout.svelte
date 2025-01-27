<script>
  import { site } from '$lib/config';

  let { children } = $props();
</script>

{@render children()}

<svelte:head>
  <title>Svelteplate</title>
  <meta name="description" content={site.desc} />
</svelte:head>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:opsz@14..32&display=swap');

  :root {
    --font-family-sans: 'Inter';
    --color-background-one: #23272f;
    --color-accent-one: #da5942;
    --color-text-one: #dadadb;
  }

  :global {
    * {
      font-family: var(--font-family-sans);

      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
  }
</style>
