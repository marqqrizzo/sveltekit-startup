# Sveltekit Startup

Collection of few commands to startup sveltekit project from scratch.

## [Sveltekit](https://kit.svelte.dev/)

```sh
npm create svelte@latest my-app
cd my-app
npm install
```

## [Tailwind CSS](https://tailwindcss.com/)

```sh
npx svelte-add@latest tailwindcss --typography
npm install
```

## [Shadcn](https://www.shadcn-svelte.com/)

###### svelte.config.js

```json
{
    "alias": {
        "$lib": "./src/lib",
        "$lib/*": "./src/lib/*"
    }
}
```

```sh
npx shadcn-svelte@latest init
npx shadcn-svelte@latest add -y -o # Select All Components `A`
```

[Shadcn Themes](https://www.shadcn-svelte.com/themes)

## [Prisma](https://www.prisma.io/)

```sh
npm install -D prisma
npx prisma init
npx prisma db push
npx prisma generate
```

`Change DATASOURCE_URL from .env`

###### package.json

```json
{
    "prisma": {
    	"seed": "node --no-warnings=ExperimentalWarning --loader ts-node/esm prisma/seed.ts"
    }
}
```

```sh
npm install -D typescript ts-node @types/node
npx prisma db seed
```

## [Notifications](https://svelte-french-toast.com/)

```sh
npm install -D svelte-french-toast
```

## [Forms](https://superforms.rocks/)

```sh
npm install -D sveltekit-superforms zod
```

## [Icons](https://lucide.dev/)

```sh
npm install -D lucide-svelte
```
