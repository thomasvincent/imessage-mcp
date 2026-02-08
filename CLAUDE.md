# CLAUDE.md

Bridges iMessage on macOS to the Model Context Protocol, allowing AI assistants to read, search, and send messages through the native Messages app.

## Stack

TypeScript, Node.js (>=18), ESM, MCP SDK

## Commands

```sh
npm run build        # tsc
npm test             # vitest run
npm run lint         # eslint src
npm run format:check # prettier --check .
npm run dev          # tsc --watch
```

## Structure & Conventions

- `src/index.ts` contains the server implementation; tests in `src/__tests__/`
- Husky + lint-staged enforce eslint and prettier on every commit
- Uses AppleScript to interact with the Messages app
