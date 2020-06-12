# cra-template-ts-prettier-eslint-airbnb

Template for [Create React App](https://create-react-app.dev) supporting [TypeScript](https://www.typescriptlang.org) and SASS/SCSS files. Included with [Prettier](https://prettier.io) and [ESlint](https://eslint.org/) config recommended by [Airbnb](https://github.com/airbnb/javascript).

## Prerequisites

- [Node.js](https://nodejs.org) (**Node.js >= 8.10 and npm >= 5.6**)

### Installation

Creating a [React](https://reactjs.org) project using a custom template.

```sh
npx create-react-app app-name --template ts-prettier-eslint-airbnb
```

### After Installation

The CRA Custom Template does not yet have support for `devDependencies`, so I recommend edit your `package.json` to like this:

```json
{
    // no changes for before lines
    "scripts": {
        "build": "react-scripts build",
        "eject": "react-scripts eject",
        "lint": "eslint src/ --ext .js,.jsx,.ts,.tsx",
        "lint:fix": "npm run lint -- --fix",
        "start": "react-scripts start",
        "test": "react-scripts test"
    },
    "dependencies": {
        "react": "^16.13.1",
        "react-dom": "^16.13.1"
    },
    "devDependencies": {
        "@testing-library/jest-dom": "^5.10.0",
        "@testing-library/react": "^10.2.1",
        "@testing-library/user-event": "^11.4.2",
        "@types/jest": "^26.0.0",
        "@types/react": "^16.9.36",
        "@types/react-dom": "^16.9.8",
        "@typescript-eslint/eslint-plugin": "^3.2.0",
        "@typescript-eslint/parser": "^3.2.0",
        "eslint": "^6.8.0",
        "eslint-config-airbnb-typescript": "^8.0.2",
        "eslint-config-prettier": "^6.11.0",
        "eslint-plugin-import": "^2.21.2",
        "eslint-plugin-import-helpers": "^1.0.2",
        "eslint-plugin-jsx-a11y": "^6.2.3",
        "eslint-plugin-prettier": "^3.1.3",
        "eslint-plugin-react": "^7.20.0",
        "eslint-plugin-react-hooks": "^4.0.4",
        "node-sass": "^4.14.1",
        "prettier": "^2.0.5",
        "react-scripts": "3.4.1",
        "typescript": "^3.9.5"
    }
    // no changes for after lines
}
````

#### License

[MIT](https://choosealicense.com/licenses/mit)
