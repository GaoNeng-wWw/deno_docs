## Node -> Deno 速查表

| Node                                   | Deno                                           |
| -------------------------------------- | ---------------------------------------------- |
| `npm i -g`                             | `deno install`                                 |
| `npm i` / `npm install`                | _n/a_ ¹                                        |
| `npm run`                              | `deno run`                                     |
| `eslint`                               | `deno lint`                                    |
| `prettier`                             | `deno fmt`                                     |
| `rollup` / `webpack` / etc             | `deno bundle`                                  |
| `package.json`                         | `deno.json` / `deno.jsonc` / `import_map.json` |
| `tsc`                                  | _n/a; tsc is built-in_ ²                       |
| `typedoc`                              | `deno doc`                                     |
| `jest` / `ava` / `mocha` / `tap` / etc | `deno test`                                    |
| `nodemon`                              | `deno run/lint/test --watch`                   |
| `nexe` / `pkg`                         | `deno compile`                                 |
| `npm explain`                          | `deno info`                                    |
| `nvm` / `n` / `fnm`                    | `deno upgrade`                                 |
| `tsserver`                             | `deno lsp`                                     |
| `nyc` / `c8` / `istanbul`              | `deno coverage`                                |
| benchmarks                             | https://deno.land/std/testing/bench.ts ³       |

¹ 查看 [链接至外部代码](../linking_to_external_code.md)，在首次运行的时候 Deno 会下载并缓存所有代码。

² 自动进行类型检查，TypeScript 编译器已经内置到了 `deno` 可执行文件中。

³ `deno bench` subcommand is being considered, see
https://github.com/denoland/deno/issues/9175
