# @aftb777/devops-pipelines

A JavaScript utility library for managing, automating, and streamlining DevOps pipelines across various environments. This package provides reusable functions and workflow definitions for CI/CD, infrastructure management, and deployment automation.

## Features

- **Pipeline Templates:** Standard templates for various CI/CD providers (GitHub Actions, GitLab CI, Azure Pipelines, etc.).
- **Automation Utilities:** Helper functions for common tasks, such as environment variable management, artifact handling, and notifications.
- **Custom Workflow Support:** Easily create and manage custom pipeline workflows.
- **Extensible:** Designed to be extended for custom project requirements.
- **TypeScript Support:** Type definitions for all public APIs.

## Installation

```bash
npm install @aftb777/devops-pipelines
```

or

```bash
yarn add @aftb777/devops-pipelines
```

## Quick Start

```typescript
import { createPipeline, runPipeline } from '@aftb777/devops-pipelines';

// Define your workflow steps
const pipeline = createPipeline([
  { name: 'Install Dependencies', run: () => installDependencies() },
  { name: 'Run Tests', run: () => runTests() },
  { name: 'Build', run: () => buildProject() },
  { name: 'Deploy', run: () => deployToEnv() }
]);

// Execute the pipeline
runPipeline(pipeline);
```


## Contact

For questions and support, open an [issue](https://github.com/aftb777/devops-pipelines/issues).
