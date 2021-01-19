# cra-template-ts-prettier-eslint-airbnb

Template for [Create React App](https://create-react-app.dev) supporting [TypeScript](https://www.typescriptlang.org) and SASS/SCSS files. Included with [Prettier](https://prettier.io) and [ESlint](https://eslint.org) config recommended by [Airbnb](https://github.com/airbnb/javascript).

### React 17
> Use a new version of React 17 even without new features, now importing `React` into JSX files is optional.

> In addition to making things simpler with automatic injection of the JSX transformer, it also reduces the file size. [Read more...](https://reactjs.org/blog/2020/10/20/react-v17.html)

Before
```jsx
import React from 'react'; // Required

function MyComponent(){
    return <div>Hello Developers!</div>;
}
```

Now
```jsx
function MyComponent(){
    return <div>Hello Developers!</div>;
}
```

### Prerequisites

- [Node.js](https://nodejs.org) (**Node.js >= 8.10 and npm >= 5.6**)

### Installation

Creating a [React](https://reactjs.org) project using a custom template.

```sh
npx create-react-app myapp --template ts-prettier-eslint-airbnb
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
        "@testing-library/jest-dom": "^5.11.9",
        "@testing-library/react": "^11.2.3",
        "@testing-library/user-event": "^12.6.0",
        "@types/jest": "^26.0.20",
        "@types/react": "^17.0.0",
        "@types/react-dom": "^17.0.0",
        "@typescript-eslint/eslint-plugin": "^4.14.0",
        "@typescript-eslint/parser": "^4.14.0",
        "eslint": "^7.18.0",
        "eslint-config-airbnb-typescript": "^12.0.0",
        "eslint-config-prettier": "^7.2.0",
        "eslint-plugin-import": "^2.22.1",
        "eslint-plugin-import-helpers": "^1.1.0",
        "eslint-plugin-jsx-a11y": "^6.4.1",
        "eslint-plugin-prettier": "^3.3.1",
        "eslint-plugin-react": "^7.22.0",
        "eslint-plugin-react-hooks": "^4.2.0",
        "node-sass": "^4.14.1",
        "prettier": "^2.2.1",
        "react-scripts": "^4.0.1",
        "typescript": "4.1.3"
    }
}
````

### License

[MIT](https://choosealicense.com/licenses/mit)