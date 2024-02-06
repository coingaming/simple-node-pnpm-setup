# simple-node-pnpm-setup

## Requirements

- Have node version defined in `package.json` in engines section
  e.g. `"engines": { "node": "20.11.0" }`
- Have pnpm version defined in `package.json` e.g. `"packageManager": "pnpm@8.15.1"`

## Inputs

- `npm_token`: NPM token to authenticate with NPM registry

## Usage

```
     steps:
       - uses: coingaming/simple-node-pnpm-setup@v1
         with:
           npm_token: ${{ secrets.NPM_TOKEN }}
```
