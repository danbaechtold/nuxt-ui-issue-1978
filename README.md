# Nuxt UI Issue 1978
https://github.com/nuxt/ui/issues/1978

## Situation
1. Created new project using Nuxt Starter: `npx nuxi@latest init -t ui` (using pnpm)
2. Created components/MyCmp.vue, added 'text-red-500 pl-8' classes, added component to app.vue
3. Created blocks/MyBlk.vue, added 'text-blue-500 pl-10' classes, added component to app.vue

## Issue
While MyCmp is indeed in red text and has left padding, MyBlk has blue text, but no left padding.
It seems that colors are always included, but paddings only if used, and usage outside of components directory is not detected.
