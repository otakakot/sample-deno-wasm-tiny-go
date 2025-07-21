# sample-deno-wasm-tiny-go

```shell
brew tap tinygo-org/tools
brew install tinygo
```

```shell
cp $(tinygo env TINYGOROOT)/targets/wasm_exec.js .
```

```shell
GOOS=js GOARCH=wasm tinygo build -o main.wasm ./main.go
```

```shell
deno index.ts
```
