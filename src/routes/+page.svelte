<script>
  import { site } from '$lib/config';

  let { desc, title } = site;
</script>

<main>
  <h3>
    <a href="https://github.com/ravaeljasny/svelteplate">See Project's GitHub!</a>
  </h3>
  <hr />
  <h1>{title}</h1>
  <h2>{desc}</h2>
</main>

<style>
  main {
    width: 100vw;
    height: 100vh;

    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;

    background-color: var(--color-background-one);
  }

  h1 {
    font-size: 64px;
    color: var(--color-accent-one);
  }

  h2 {
    font-size: 32px;
    color: var(--color-text-one);
    font-weight: 400;
  }

  h3 {
    margin-bottom: 10px;
    color: var(--color-text-one);
    font-size: 20px;
    font-weight: 400;

    a {
      transition: color 400ms;
      text-decoration: underline 0.15em rgba(0, 0, 0, 0);
      transition: text-decoration 600ms;
      color: inherit;
    }

    a:hover {
      text-decoration-color: var(--color-accent-one);
      color: var(--color-accent-one);
    }
  }

  hr {
    width: 300px;
    border: 1px solid var(--color-text-one);
  }
</style>
