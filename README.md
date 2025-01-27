# Svelteplate

Template project that saves time on configuring good practices that I use in my all web projects.

[Netlify Preview](https://svelteplate.netlify.app)

## Motivation

The big reason why I built this project is because I want it to automate setup of:

- Commitlint & Conventional Commits: Helps me keep the rules of readable commits
- Husky & Git Hooks: Allows me to take more control and motivate to write tests
- Prettier, ESLint: First one makes Code pretty, second detects errors
- Lint-staged: Simplifies automation of Linter, Formatter and Husky
- EditorConfig: Sets project's standard for formatting
- `.nvmrc`: In case you, contributors, are using different node version.
- VSCode (see `.vscode/`): Tells what you need in terms of vsc
- MIT License: I will probably be always using this license for my projects, so...

Also, it sets some settings I don't need to set every time I create project such as:

- Serve `port` to 3000 (see `vite.config.ts`)
- Runes mode (see `svelte.config.js`)
- `src/routes/+layout.svelte`:
  - Little SEO stuff, e.g. title, description of site (see `src/lib/config.ts`)
  - CSS variables naming (still finding out standard for this)
  - Global style and `Inter` font

## Tech Stack

- `pnpm`
- SvelteKit
- CSS (Plain)
- TypeScript

## Run Locally

Clone the project

```bash
  git clone https://github.com/ravaeljasny/svelteplate
```

Go to the project directory

```bash
  cd svelteplate
```

Install dependencies

```bash
  pnpm install
```

Start the server

```bash
  pnpm dev
```

## Authors

- [@ravaeljasny](https://www.github.com/ravaeljasny)

Contributions are welcome!

## License

[MIT](https://choosealicense.com/licenses/mit/)
