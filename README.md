# Demo repo: Webstorm + pnpm = !Intellisense

To reproduce:

```sh
$ cd lib && corepack enable
$ pnpm i && pnpm build && pnpm pack
$ cd ../app && corepack enable
$ pnpm i
```

Now open `app/src/app.ts` and try to trigger the `foo()` function 
parameter with `Ctrl+P`: it doesn't work.


