# Repro for https://github.com/rolldown/tsdown/issues/319

Steps:

* git clone
* pnpm install
* `pnpm build` => Output is ok (bundled)
* `pnpm build --unbundle` (or `unbundle: true` in `tsdown.config.ts` file) => Output is KO on windows (CSS output in the `src` folder)
