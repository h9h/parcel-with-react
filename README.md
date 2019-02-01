# Setup eines React Projektes mit Parcel

**Schritt 1:** Projekt initialisieren
```shell
yarn init
``` 

**Schritt 2:** Lokale Parcel-Installation:
```shell
yarn add --dev parcel
``` 

**Schritt 3:** Babel:
```shell
yarn add --dev babel-preset-env babel-preset-react
```

und in .babelrc:
```
{
  "presets": ["env", "react"]
}
```

**Schritt 4:** index.html:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Test</title>
</head>
<body>
    <div id="root"/>
    <script src="./index.js"></script>
</body>
</html>
```

**Schritt 5:** index.js:
```
import React from 'react'
import ReactDOM from 'react-dom'

const App = () => <div>Hello World!</div>

ReactDOM.render(
  <App />,
  document.getElementById('root')
)
```

**Starte die App:**
```shell
parcel index.html
```

