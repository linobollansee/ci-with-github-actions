# CI with GitHub Actions

[![CI](https://github.com/linobollansee/ci-with-github-actions/actions/workflows/ci.yml/badge.svg)](https://github.com/linobollansee/ci-with-github-actions/actions)

A minimal NestJS application with automated CI/CD pipeline using GitHub Actions.

## Features

- NestJS 11.x
- TypeScript 5.x
- ESLint 9.x with flat config
- Jest 30.x for testing
- GitHub Actions CI pipeline

## Getting Started

```bash
# Install dependencies
npm install

# Run the app
npm start

# Build
npm run build

# Run tests
npm test

# Lint
npm run lint
```

## CI Pipeline

The project includes a GitHub Actions workflow that automatically:
- Lints code with ESLint
- Builds the TypeScript project
- Runs all tests

The workflow triggers on:
- Push to `main` branch
- Pull requests

## Viewing Workflow Results

To see the CI pipeline in action:

1. Go to the **Actions** tab in your GitHub repository: `https://github.com/linobollansee/ci-with-github-actions/actions`
2. Click on any workflow run to see the details
3. Expand each step to view logs for:
   - Code checkout
   - Dependency caching
   - Node.js setup
   - Package installation
   - Lint results
   - Build output
   - Test results

The status badge at the top of this README shows the current state of the latest workflow run.

## Project Structure

```
src/
├── app.controller.ts      # Main controller
├── app.service.ts         # Main service
├── app.module.ts          # Root module
├── app.controller.spec.ts # Tests
└── main.ts                # Application entry point
```
