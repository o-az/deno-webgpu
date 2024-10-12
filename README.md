first upgrade deno to latest stable version

```shell-session
deno upgrade
```

on macOS

```shell-session
DENO_SDL2_PATH=/opt/homebrew/lib/ deno run --allow-all main.ts
```

or

```shell-session
deno run --allow-all --env main.ts
```

depending on your version, you might need to add unstable flags to `deno.jsonc`

```jsonc
// ...
{
  "unstable": [
    "ffi",
    "webgpu"
  ]
}
```
