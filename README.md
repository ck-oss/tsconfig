# @ck-oss/tsconfig

CK OSS Typescript Configuration

## Installation

```
npm i -D @ck-oss/tsconfig
```

## Base

```json
// tsconfig.json
{
  "extends": "@ck-oss/tsconfig/base.json"
}
```

## Hono + Cloudflare Workers

```json
// tsconfig.json
{
  "extends": "@ck-oss/tsconfig/hono-cloudflare.json"
}
```

Make sure to also install Hono and Cloudflare Workers Types

```bash
npm i hono && npm i -D @cloudflare/workers-types
```

## Next.js

```json
// tsconfig.json
{
  "extends": "@ck-oss/tsconfig/next.json",
  "compilerOptions": {
    "plugins": [
      {
        "name": "next"
      }
    ],
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": ["next-env.d.ts", "**/*.ts", "**/*.tsx", ".next/types/**/*.ts"],
  "exclude": ["node_modules"]
}
```

# Node Library

```json
// tsconfig.json
{
  "extends": "@ck-oss/tsconfig/node-library.json"
}
```

# React Library

```json
// tsconfig.json
{
  "extends": "@ck-oss/tsconfig/react-library.json"
}
```
