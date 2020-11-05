# cra-template-ts-prettier-eslint-airbnb

Template for [Create React App](https://create-react-app.dev) supporting [TypeScript](https://www.typescriptlang.org) and SASS/SCSS files. Included with [Prettier](https://prettier.io) and [ESlint](https://eslint.org) config recommended by [Airbnb](https://github.com/airbnb/javascript).

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
    "scripts": {
        "build": "react-scripts build",
        "eject": "react-scripts eject",
        "lint": "eslint src/ --ext .js,.jsx,.ts,.tsx",
        "lint:fix": "npm run lint -- --fix",
        "start": "react-scripts start",
        "test": "react-scripts test"
    },
    "dependencies": {
        "react": "^17.0.1",
        "react-dom": "^17.0.1",
    },
    "devDependencies": {
        "@testing-library/jest-dom": "^5.11.5",
        "@testing-library/react": "^11.1.1",
        "@testing-library/user-event": "^12.2.0",
        "@types/jest": "^26.0.15",
        "@types/react": "^16.9.55",
        "@types/react-dom": "^16.9.9",
        "@typescript-eslint/eslint-plugin": "^4.6.1",
        "@typescript-eslint/parser": "^4.6.1",
        "eslint": "^7.11.0",
        "eslint-config-airbnb-typescript": "^12.0.0",
        "eslint-config-prettier": "^6.15.0",
        "eslint-plugin-import": "^2.22.1",
        "eslint-plugin-import-helpers": "^1.1.0",
        "eslint-plugin-jsx-a11y": "^6.4.1",
        "eslint-plugin-prettier": "^3.1.4",
        "eslint-plugin-react": "^7.21.5",
        "eslint-plugin-react-hooks": "^4.2.0",
        "node-sass": "^4.14.1",
        "prettier": "^2.1.2",
        "react-scripts": "4.0.0",
        "typescript": "^4.0.5"
    }
}
````

#### License

[MIT](https://choosealicense.com/licenses/mit)
