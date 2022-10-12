# `@hackclub/icons`

Hack Club’s icons are a superset of [Spectrum](https://spectrum.chat)’s incredible collection (also published as [`spectrum-icons`](https://github.com/lachlanjc/spectrum-icons)). Designed for use with our [Design System](https://github.com/hackclub/design-system).

[See them all](https://hackclub-icons.now.sh)

## Usage

### With React

```sh
npm i @hackclub/icons
```

```js
import React from 'react'
import Icon from '@hackclub/icons'

export default () => (
  <div style={{ color: 'cyan' }}>
    <Icon glyph="clubs" size={128} />
    <Icon glyph="bank-circle" size={64} />
    <Icon glyph="leaders" size={32} />
  </div>
)
```

### With API

`https://icons.hackclub.com/api/icons/:color/:glyph`
 - `:glyph` - A glyph from [icons.hackclub.com](https://icons.hackclub.com).
 - `:color` - Any valid HTML color. Replace `#` with `0x` when using a hexadecimal color.

Examples:

```html
<img src="https://icons.hackclub.com/api/icons/red/clubs">
<img src="https://icons.hackclub.com/api/icons/0x33d6a6/battery-bolt">
```

## Development Setup

1. Clone & enter the repo.

```sh
$ git clone https://github.com/hackclub/icons.git
$ cd icons
```

2. Install dependencies.

```sh
$ yarn
```

3. Build library.

```sh
yarn run prepare
```

4. Run docs locally.

```sh
yarn run dev
```
