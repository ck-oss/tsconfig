# @ck-oss/tsconfig

CK OSS Typescript Configuration

## Installation

```bash
npm i --save-dev @ck-oss/tsconfig
```

## Base

```json
{
  "extends": "@ck-oss/tsconfig/base.json"
}
```

Make sure to also install Cloudflare Workers Types

```bash
npm i --save-dev @cloudflare/workers-types
```

## Next.js

```json
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

# Node.js

```json
{
  "extends": "@ck-oss/tsconfig/node.json"
}
```

# React.js

```json
{
  "extends": "@ck-oss/tsconfig/react.json"
}
```
