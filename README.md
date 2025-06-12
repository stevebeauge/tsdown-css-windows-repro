# Repro for https://github.com/rolldown/rolldown/issues/4934

Steps:

* git clone
* pnpm install
* `pnpm build` => KO (css files in src dir instead of dist dir)
* remove preserveModules option in config
* `pnpm build` => Output is OK
