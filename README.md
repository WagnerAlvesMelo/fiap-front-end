# Link Tree

This project renders a link tree page, that show links to my social medias. It was created using NuxtJS and TailwindCSS. It builds using [SSG strategy](https://en.wikipedia.org/wiki/Static_site_generator), because it's a static page (setted in nuxt.config.js).

## Netlify deployed page

https://moonlit-fairy-f1c698.netlify.app/

## Setup

Install the correct NodeJS version (v22.14.0), the project has a nvmrc file, so you can use nvm or fnm to manage your NodeJS installation.

```bash
nvm use
corepack enable
```

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production (use dist page to get deploy files):

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

## Generate Static

Pre-renders every route of the application and stores the result in plain HTML files:

```bash
# npm
npm run generate

# pnpm
pnpm generate

# yarn
yarn generate

# bun
bun run generate
```

## Preview

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```
