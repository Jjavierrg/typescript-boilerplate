# typescript-boilerplate

This is a template repository. So just use the template and once you have your repository cloned on your pc just run `npm install` for installing all the dependencies.

## Scripts

```json
  "prepare": "husky install",
  "dev": "nodemon src/index.ts",
  "start": "node build/index.js",
  "build": "npm run lint && npm test && tsc",
  "lint": "eslint . --ext .ts",
  "lint:fix": "npm run lint -- --fix",
  "test": "jest --verbose",
  "test:watch": "npm t -- --watchAll",
  "test:coverage": "npm t -- --coverage",
  "docs:generate": "rimraf docs && typedoc src/ --out docs"
```

- **prepare**: This script is used for installing husky hooks. It is used for running the linting and testing before every commit.
- **dev**: This script is used for running the application in development mode. It uses nodemon for watching the changes in the code.
- **start**: This script is used for running the application in production mode. It uses the build folder for running the application.
- **build**: This script is used for building the application. It runs the linting, testing and then compiles the typescript code.
- **lint**: This script is used for linting the application. It uses eslint for linting the code.
- **lint:fix**: This script is used for fixing the linting errors.
- **test**: This script is used for running the tests. It uses jest for running the tests.
- **test:watch**: This script is used for running the tests in watch mode.
- **test:coverage**: This script is used for running the tests and generating the coverage report.
- **docs:generate**: This script is used for generating the documentation. It uses typedoc for generating the documentation.
