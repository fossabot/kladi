<p align="center">
  <a href="https://www.npmjs.com/package/kladi"><img src="./logo.svg" width="80%"></a>

<a href="https://www.npmjs.com/package/kladi"><img src="https://img.shields.io/npm/v/kladi.svg" alt="NPM"/></a>
<a href="https://standardjs.com"><img src="https://img.shields.io/badge/code_style-standard-brightgreen.svg" alt="JavaScript Style Guide"/></a>
<a href="https://github.com/Ninja-Developers/kladi/blob/master/LICENSE"><img src="https://img.shields.io/github/license/Ninja-Developers/kladi?logo=github" alt="Github License"></a>
<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FNinja-Developers%2Fkladi?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FNinja-Developers%2Fkladi.svg?type=shield"/></a>
![npm](https://img.shields.io/npm/dw/kladi?style=plastic)
</p>

## Install

```bash
npm install --save kladi
```

## Usage

```jsx
import { Provider, useGlobalState } from "kladi";

import React from "react";
import ReactDOM from "react-dom";
import App from "./App";

ReactDOM.render(
  <Provider>
    <App />
  </Provider>,
  document.getElementById("root")
);

const App = (props) => {
  let [count, setCount] = useGlobalState("count", 0);

  return (
    <div>
      {count}
      <button
        onClick={() => {
          setCount(count + 1);
        }}
      >
        Press
      </button>
    </div>
  );
};

```

## License

MIT © [Ninja-Developers](https://github.com/Ninja-Developers)


[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FNinja-Developers%2Fkladi.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FNinja-Developers%2Fkladi?ref=badge_large)