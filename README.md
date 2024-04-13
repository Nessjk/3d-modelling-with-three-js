## Starter

Using `ni` https://github.com/antfu/ni as package manager to try it out. If you’re fed up of typing `npm install` in a `yarn` project, this is for you! It’s helps you select the right package manager.

`nr dev --port=3000` runs

```sql
nr dev --port=3000

# npm run dev -- --port=3000
# yarn run dev --port=3000
# pnpm run dev --port=3000
# bun run dev --port=3000
```

Known bugs with ni:

- node -v 14

## Tag elements info

`<primitive />`

`<suspense />`

## Miscellaneous

`toValue()` is an API added in 3.3. It is designed to normalize refs or getters into values. If the argument is a ref, it returns the ref's value; if the argument is a function, it will call the function and return its return value. Otherwise, it returns the argument as-is. It works similarly to **`[unref()](https://vuejs.org/api/reactivity-utilities#unref)`**, but with special treatment for functions.

## Extra info

`composable` folder to use state. You can think of them as the equivalent of mixins from back in the day, but better. Unlike mixins, which can cause variable and method name clashes composables come with

- the Composition API which has better typescript integration.
- complete control over imports and exports
- better scalability
- Clearer Lifecycle Hook Management
- Tree Shaking Support (elimination of unused code) - every mixin is used in every component where it's included
