### NestJS Boilerplate

- NestJS
- Typescript
- EsLint
- Jest
- Husky
- Lint-Staged
- Styled-Components

package.json

```js
{
  "name": "nestjs-boilerplate",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "eslint src --max-warnings=0",
    "test": "jest",
    "test:watch": "yarn test --watch"
  },
  "dependencies": {
    "@types/node": "^14.11.2",
    "@types/react": "^16.9.50",
    "next": "9.5.3",
    "react": "16.13.1",
    "react-dom": "16.13.1",
    "styled-components": "^5.2.0"
  },
  "devDependencies": {
    "@babel/core": "^7.11.6",
    "@babel/preset-typescript": "^7.10.4",
    "@testing-library/jest-dom": "^5.11.4",
    "@testing-library/react": "^11.0.4",
    "@types/jest": "^26.0.14",
    "@types/styled-components": "^5.1.3",
    "@typescript-eslint/eslint-plugin": "^4.3.0",
    "@typescript-eslint/parser": "^4.3.0",
    "babel-loader": "^8.1.0",
    "babel-plugin-styled-components": "^1.11.1",
    "eslint": "^7.10.0",
    "eslint-config-prettier": "^6.12.0",
    "eslint-plugin-prettier": "^3.1.4",
    "eslint-plugin-react": "^7.21.3",
    "eslint-plugin-react-hooks": "^4.1.2",
    "jest": "^26.4.2",
    "jest-styled-components": "^7.0.3",
    "prettier": "^2.1.2",
    "typescript": "^4.0.3"
  },
  "husky": {
    "hooks": {
      "pre-commit": "lint-staged"
    }
  },
  "lint-staged": {
    "src/**/*": [
      "yarn lint --fix",
      "yarn test --findRelatedTests --bail"
    ]
  }
}


```
