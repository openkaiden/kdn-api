# kortex-cli Types

[![npm version](https://img.shields.io/npm/v/@kortex-hub/kotex-cli-api.svg)](https://www.npmjs.com/package/@kortex-hub/kotex-cli-api)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

TypeScript type definitions for the [kortex-cli](https://github.com/kortex-hub/kortex-cli), providing complete type safety when interacting with JSON output returned by the CLI.

## Installation

```bash
npm install @kortex-hub/kortex-cli-api
```

Or with your preferred package manager:

```bash
# pnpm
pnpm add @kortex-hub/kortex-cli-api

# yarn  
yarn add @kortex-hub/kortex-cli-api

# bun
bun add @kortex-hub/kortex-cli-api
```

## Usage

```typescript
import type { paths, components } from '@kortex-hub/kortex-cli-api';

// Type for agents list response
type AgentsListResponse = paths['/list']['get']['responses']['200']['content']['application/json'];

// Type for a single server
type Server = components['schemas']['AgentsList'];
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
