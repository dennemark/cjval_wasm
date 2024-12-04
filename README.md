# cjval_wasm

Forked from https://github.com/cityjson/cjval_wasm and published on npm as `cjval_wasm_web` and `cjval_wasm_nodejs`

## To compile and run locally:

1. install [wasm-pack](https://rustwasm.github.io/wasm-pack/installer/)
2. `wasm-pack build -t web --out-dir ./www/pkg/`
3. `cd ./www/`
4. `python -m http.server 8080` (or any local webserver will do)
5. with your browser go to http://localhost:8080/

## Online demo

[==> demo](https://validator.cityjson.org)

## Release
(can be improved a lot, most probably...)
### for web
`wasm-pack build -t web --out-dir ./www/pkg/`
rename name in package.json to cjval_wasm_web
`wasm-pack pack ./www/pkg/`
`wasm-pack publish ./www/pkg/`

### for nodejs
`wasm-pack build -t web --out-dir ./nodejs/pkg/`
rename name in package.json to cjval_wasm_nodejs
`wasm-pack pack ./nodejs/pkg/`
`wasm-pack publish ./nodejs/pkg/`
