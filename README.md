## (Unofficially) UNDEPRECATED: electron-prebuilt-compile

[![Unofficially Maintained](https://img.shields.io/badge/Unofficially%20Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)

This project is now (unofficially) maintained by Lane Shaw, new pull requests will be reviewed (as time permits) or merged and new issues can be reported here.

---

electron-prebuilt-compile is a drop-in replacement for [electron](https://github.com/electron/electron) (previously was [electron-prebuilt](https://github.com/mafintosh/electron-prebuilt)) that natively understands ES6/ES7 + React + LESS + some other languages, powered by [@lanethegreat/electron-compile](https://github.com/LanetheGreat/electron-compile).

## Installation

Download and install the latest build of `@lanethegreat/electron-prebuilt-compile` for your OS and add it to your project's `package.json` as a `devDependency`:

```
npm install @lanethegreat/electron-prebuilt-compile --save-dev
```

Now you can just run `electron` to run electron:

```
electron
```

Electron will now understand ES6/ES7 and React components out-of-the-box, even in inline HTML:

```html
<head>
  <link rel="stylesheet" type="text/less" href="main.less" />
</head>

<body id="host">
  <script type="application/javascript">
  import React from 'react';
  import ReactDOM from 'react-dom';
  import TodoApp from './components/TodoApp';
  
  ReactDOM.render(React.createComponent(TodoApp), document.getElementById('host'));
  </script>
</body>
</html>
```
