# React Tailwindcss Datepicker

## Contents

-   [Features](#features)
-   [Documentation](#documentation)
-   [Installation](#installation)
-   [Simple Usage](#simple-usage)
-   [Theming Options](#theming-options)
-   [Playground](#playground)
-   [Contributing](#contributing)

## Features

-   ✅ Theming options
-   ✅ Dark mode
-   ✅ Single Date
-   ✅ Single date use Range
-   ✅ Shortcuts
-   ✅ TypeScript support
-   ✅ Localization(i18n)
-   ✅ Date formatting
-   ✅ Disable specific dates
-   ✅ Minimum Date and Maximum Date
-   ✅ Custom shortcuts

### Install via npm

```
$ npm install react-tlwind-datepicker
```

### Install via yarn

```
$ yarn add react-tlwind-datepicker
```

Make sure you have installed the peer dependencies as well with the below versions.

```
"dayjs": "^1.11.6",
"react": "^17.0.2 || ^18.2.0"
```

## Simple Usage

#### Tailwindcss Configuration

Add the datepicker to your tailwind configuration using this code

```javascript
// in your tailwind.config.js
module.exports = {
    // ...
    content: [
        "./src/**/*.{js,jsx,ts,tsx}",
        "./node_modules/react-tlwind-datepicker/dist/index.esm.js"
    ]
    // ...
};
```

Then use react-tailwindcss-select in your app:

```jsx
import React, { useState } from "react";
import Datepicker from "react-tlwind-datepicker";

const App = () => {
    const [value, setValue] = useState({
        startDate: new Date(),
        endDate: new Date().setMonth(11)
    });

    const handleValueChange = newValue => {
        console.log("newValue:", newValue);
        setValue(newValue);
    };

    return (
        <div>
            <Datepicker value={value} onChange={handleValueChange} />
        </div>
    );
};

export default App;
```

## Theming options

**Light Mode**

![Light Mode](https://raw.githubusercontent.com/onesine/react-tlwind-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_light.png?raw=true)

**Dark Mode**

![Dark Mode](https://raw.githubusercontent.com/onesine/react-tlwind-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_dark.png?raw=true)

**Supported themes**
![Theme supported](https://raw.githubusercontent.com/onesine/react-tlwind-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_theme.png?raw=true)

**Teal themes example**
![Theme supported](https://raw.githubusercontent.com/onesine/react-tlwind-datepicker/master/assets/img/Screen_Shot_2022-08-04_at_17.04.09_teal.png?raw=true)

You can find the demo at [here](https://react-tlwind-datepicker.vercel.app/demo)

> **Info**
>
> 👉 To discover the other possibilities offered by this library, you can consult the
> [full documentation](https://react-tlwind-datepicker.vercel.app/).

## PlayGround

Clone the `master` branch and run commands:

```sh
# Using npm
npm install && npm dev

# Using yarn
yarn install && yarn dev

```

Open a browser and navigate to `http://localhost:8888`

## Thanks to

-   [onesine](https://github.com/onesine/react-tailwindcss-datepicker/)

I thank you in advance for your contribution to this project.

## License

[MIT](LICENSE) Licensed. Copyright (c) Lewhe Onesine 2022.
