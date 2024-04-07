# Bazel + React + TypeScript + Vite + Vitest on monorepo

## Start dev server

```bash
$ bazelisk run -- @pnpm//:pnpm --dir $PWD run --filter my-react-app dev
```

## Build

```bash
$ bazelisk build //...
$ ls $(bazelisk cquery --output=files //packages/my-react-app:vite)
```

## Test

```bash
$ bazelisk test //...
```
