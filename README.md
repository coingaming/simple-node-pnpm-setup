# simple-node-pnpm-setup

This action sets up Node.js and pnpm then installs dependencies.

## Requirements

- Have node version defined in `package.json` in engines section
  e.g. `"engines": { "node": "20.11.0" }`
- Have pnpm version defined in `package.json` e.g. `"packageManager": "pnpm@8.15.1"`

## Inputs

- `npm_token`: NPM token to authenticate with NPM registry

## Usage

```
    steps:
      - name: 'Install Node.js, pnpm and dependencies'
        uses: coingaming/simple-node-pnpm-setup@v1
        with:
          npm_token: ${{ secrets.NPM_TOKEN }}
```
