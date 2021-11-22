# cra-template-ts-prettier-eslint-airbnb

Template for [Create React App](https://create-react-app.dev) supporting [TypeScript](https://www.typescriptlang.org) with [Prettier](https://prettier.io) and [ESlint](https://eslint.org) config recommended by [Airbnb](https://github.com/airbnb/javascript).

## React 17

> Use a new version of React 17 even without new features, now importing `React` into JSX files is optional.
> In addition to making things simpler with automatic injection of the JSX transformer, it also reduces the file size. [Read more...](https://reactjs.org/blog/2020/10/20/react-v17.html)

Before

```jsx
import React from 'react'; // Required

function MyComponent(){
    return (
        <div>Hello Developers!</div>
    );
}
```

Now

```jsx
function MyComponent(){
    return (
        <div>Hello Developers!</div>
    );
}
```

## Prerequisites

- [Node.js](https://nodejs.org) (**Node.js >= 8.10 and npm >= 5.6**)

## Installation

Creating a [React](https://reactjs.org) project using a custom template.

```sh
npx create-react-app myapp --template ts-prettier-eslint-airbnb
```

## After Installation

The CRA Custom Template does not yet have support for `devDependencies`, so I recommend edit your `package.json` to like this:

```json
{
    "name": "myapp",
    "version": "0.1.0",
    "private": true,
    "scripts": {
        "build": "npm run lint && react-scripts build",
        "eject": "react-scripts eject",
        "lint": "eslint src/ --ext .js,.jsx,.ts,.tsx",
        "lint:fix": "npm run lint -- --fix",
        "start": "react-scripts start",
        "test": "react-scripts test"
    },
    "dependencies": {
        "react": "^17.0.2",
        "react-dom": "^17.0.2",
        "react-scripts": "^4.0.3",
        "web-vitals": "^2.1.2"
    },
    "devDependencies": {
        "@testing-library/jest-dom": "^5.15.0",
        "@testing-library/react": "^12.1.2",
        "@testing-library/user-event": "^13.5.0",
        "@types/jest": "^27.0.3",
        "@types/react": "^17.0.36",
        "@types/react-dom": "^17.0.11",
        "@typescript-eslint/eslint-plugin": "^5.4.0",
        "@typescript-eslint/parser": "^5.4.0",
        "eslint": "^7.11.0",
        "eslint-config-airbnb": "^18.2.1",
        "eslint-config-airbnb-typescript": "^16.0.0",
        "eslint-config-prettier": "^8.3.0",
        "eslint-plugin-import": "^2.25.3",
        "eslint-plugin-import-helpers": "^1.2.0",
        "eslint-plugin-jsx-a11y": "^6.5.1",
        "eslint-plugin-prettier": "^4.0.0",
        "eslint-plugin-react": "^7.27.1",
        "eslint-plugin-react-hooks": "^4.3.0",
        "prettier": "^2.4.1",
        "typescript": "4.5.2"
    },
    "eslintConfig": {
        "extends": "react-app"
    },
    "browserslist": {
        "development": [
            "last 1 chrome version",
            "last 1 firefox version",
            "last 1 safari version"
        ],
        "production": [
            ">0.2%",
            "not dead",
            "not op_mini all"
        ]
    }
}
````

## License

[MIT](https://choosealicense.com/licenses/mit)