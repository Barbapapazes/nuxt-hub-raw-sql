Reproduction for an issue related to NuxtHub when using raw SQL for migrations.

In order to reproduce:

- Clone the repository
- Install dependencies with `pnpm install`
- Run the application with `pnpm run dev`
- Open your browser and check your console for the error

```bash
ERROR  [nitro] [unhandledRejection] D1_EXEC_ERROR: Error in line 1: CREATE TABLE IF NOT EXISTS todos (: incomplete input

at process.processTicksAndRejections (node:internal/process/task_queues:95:5)
at <anonymous> (server/plugins/migrations.ts:5:1)
at async Promise.all (index 0)
at <anonymous> (node_modules/.pnpm/@nuxthub+core@0.5.14_ioredis@5.4.1_nuxt@3.11.2_@parcel+watcher@2.4.1_@types+node@20.12.7_@uno_v6ufku3kw6jhvrpovvvt7rg5kq/node_modules/@nuxthub/core/dist/runtime/ready.dev.mjs:5:3)
```

---

I strictly follow this page: https://hub.nuxt.com/docs/recipes/hooks.
