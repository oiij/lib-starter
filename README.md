# lib-starter

<p align="center">

[![TypeScript](https://img.shields.io/badge/TypeScript-6.0-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![tsdown](https://img.shields.io/badge/tsdown-0.22-FF6B6B?logo=esbuild&logoColor=white)](https://tsdown.dev/)
[![Vitest](https://img.shields.io/badge/Vitest-4.1-6E9F18?logo=vitest&logoColor=white)](https://vitest.dev/)
[![pnpm](https://img.shields.io/badge/pnpm-9+-F69220?logo=pnpm&logoColor=white)](https://pnpm.io/)
[![ESLint](https://img.shields.io/badge/ESLint-10.4-4B32C3?logo=eslint&logoColor=white)](https://eslint.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/oiij/lib-starter/blob/main/LICENSE)

</p>

A modern TypeScript library starter template with built-in development tools and best practices.

## Features

- 🚀 **TypeScript** - Type-safe development
- 📦 **tsdown** - Fast TypeScript bundler for library development
- ✅ **Vitest** - Lightning fast unit testing
- 🔍 **ESLint** - Code linting with @antfu/eslint-config
- 📝 **Commitlint** - Conventional commit messages
- 🪝 **Git Hooks** - Pre-commit hooks with simple-git-hooks
- 🔄 **pnpm** - Fast, disk space efficient package manager
- 📖 **VitePress** - Documentation site

## Quick Start

### Prerequisites

- Node.js >= 18
- pnpm >= 9

### Installation

```bash
# Clone the repository
git clone https://github.com/oiij/lib-starter.git
cd lib-starter

# Install dependencies
pnpm install
```

## Development

```bash
# Start development mode with watch
pnpm dev

# Run the source code directly
pnpm start

# Type checking
pnpm type:check
```

## Building

```bash
# Build the project
pnpm build
```

The build output will be in the `dist` directory.

## Testing

```bash
# Run tests
pnpm test

# Run tests with UI
pnpm test --ui
```

## Linting

```bash
# Lint code
pnpm lint

# Fix linting issues
pnpm lint:fix
```

## Documentation

```bash
# Start docs dev server
pnpm docs:dev

# Build docs
pnpm docs:build

# Preview docs
pnpm docs:preview
```

## Committing Changes

This project uses conventional commits with commitlint and cz-git.

```bash
# Stage changes and commit with interactive prompt
pnpm commit

# Or use commitizen directly
pnpm cz
```

## Publishing

```bash
# Bump version and publish to npm
pnpm release
```

## Scripts

| Script             | Description                                  |
| ------------------ | -------------------------------------------- |
| `pnpm dev`         | Start development mode with watch            |
| `pnpm build`       | Build the project                            |
| `pnpm start`       | Run source code directly                     |
| `pnpm test`        | Run tests                                    |
| `pnpm lint`        | Lint code                                    |
| `pnpm lint:fix`    | Fix linting issues                           |
| `pnpm type:check`  | Run TypeScript type checking                 |
| `pnpm commit`      | Interactive commit with conventional commits |
| `pnpm release`     | Bump version and publish                     |
| `pnpm docs:dev`    | Start docs dev server                        |
| `pnpm docs:build`  | Build documentation                          |
| `pnpm docs:preview`| Preview documentation                        |
| `pnpm update:deps` | Update dependencies interactively            |

## Project Structure

```
lib-starter/
├── packages/         # Library source code
│   └── index.ts
├── test/             # Test files
├── dist/             # Build output
├── docs/             # VitePress documentation
├── package.json      # Package configuration
├── tsconfig.json     # TypeScript configuration
├── tsdown.config.ts  # tsdown configuration
├── vitest.config.ts  # Vitest configuration
└── eslint.config.js  # ESLint configuration
```

## License

[MIT](./LICENSE) License © 2026 [oiij](https://github.com/oiij)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`pnpm commit`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
