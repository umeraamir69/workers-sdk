---
"@cloudflare/workers-utils": minor
---

Add a `@cloudflare/workers-utils/binding-local-support` entry point

Tools that only need to decide whether a binding runs locally or remotely can now import `getBindingLocalSupport()`, `resolveBindingRemote()` and `validateBindingRemoteSetting()` from `@cloudflare/workers-utils/binding-local-support`, without loading the package's config parsing and validation code. Miniflare uses it to warn when an Artifacts binding omits `remote`.
