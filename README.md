# Requite for Svelte

Dynamic selector for Svelte Components. Great for creating dynamic pages. Through some form of interaction, for example Loop, a page can be created dynamically. It can be used for a dynamic editor or even through a Json file.

[![NPM](https://img.shields.io/npm/v/requite.svg)](https://www.npmjs.com/package/requite-svelte) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

![Requite](https://i.imgur.com/vdWjYt5.png)

## Installation

Just install the dependency and start using

```javascript

npm i requite-svelte or yarn add requite-svelte

```

### How to import

After installing the dependency, just import the components you need

```javascript
import Requite from "./requite-svelte";
```

## Usage

```js
<script>
  import Header from "./Header.svelte";
  import Button from "./Button.svelte";
  import Requite from "requite-svelte";

  let components = {
    Header,
    Button
  };

  let data = [
    {
      name: "Header"
    },
    {
      name: "Button"
    }
  ];
</script>

<style>
  main {
    margin-top: 70px;
  }
</style>

<main>
    <Requite {data} {components} />
</main>
```

## License

MIT © [vacom](https://github.com/vacom)
