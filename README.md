# MachTech

#### Current Release: https://machtech.netlify.app

#### Future Release: https://machtech-next.netlify.app
<br />

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

### `npm run extract`

**Note: please use the argument `-- 'src/**/*.js' --out-file lang/en.json --id-interpolation-pattern '[sha512:contenthash:base64:6]'`**

Extract messages and get ready to translate

### `npm run compile`

**Note: sample arguments `-- lang/en.json --ast --out-file src/compiled-lang/en.json`**

Generate the react-intl consumable JSON file for all translated messages

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify

### Message Extraction

This section has moved here: https://formatjs.io/docs/getting-started/message-extraction

### Message Distribution

This section has moved here: https://formatjs.io/docs/getting-started/message-distribution/

## Developer Rule

### Multi-language Support

All text on the front end should be declared to support multi-language.

See help: https://formatjs.io/docs/getting-started/message-declaration

It is suggested to use `useIntl` hook

See help: https://formatjs.io/docs/react-intl/api#useintl-hook

Imperative API Documentation: https://formatjs.io/docs/react-intl/api

```javascript
// Example
import { useIntl } from "react-intl"

function fooBar() {
    const intl = useIntl()
    intl.formatMessage({
        id: 'myMessage', // A unique, stable identifier for the message
        description: 'A message', // Context for the translator about how it's used in the UI.
        defaultMessage: 'My name is {name}', // The default message (in English)
    }, {
        name: userName, // Values should be an object literal, but not necessarily every value inside
    })
}
# renfrew.github.io
