# The documentation on how to write plugins for nuxt-ts seems to be outdated. This is a simple reproduction.

This project was set up using [create-nuxt-app@latest](https://github.com/nuxt/create-nuxt-app). A plugin was added according and using the example code of the [Nuxt.js/TypeScript Cookbook](https://typescript.nuxtjs.org/cookbook/plugins.html#iii-combined-inject).

How to reproduce the error message:

1. Clone, install, etc.
2. Open the start page [`pages/index.vue`](https://github.com/tillsanders/nuxt-ts-cookbook-error/blob/master/pages/index.vue) in your IDE (tested with VS Code)
3. Take a look at line 35. You should see a Vetur warning for `$myInjectedFunction`: `Property '$myInjectedFunction' does not exist on type 'CombinedVueInstance<Vue, unknown, unknown, unknown, Readonly<Record<never, any>>>'.Vetur(2339)`