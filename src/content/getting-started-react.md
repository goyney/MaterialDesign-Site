# React - Getting Started

Material Design Icons can be used in React with a custom component or with the one provided in this module.

```
npm install @mdi/react @mdi/js
```

<a href="https://templarian.github.io/@mdi/react/" class="btn btn-outline-primary">icon:teach Demo</a>
<a href="https://github.com/Templarian/MaterialDesign-React" class="btn btn-outline-secondary ml-2">icon:github-circle MaterialDesign-React on GitHub</a>

## Usage

```javascript
import React, { Component } from 'react'
import Icon from '@mdi/react'
import { mdiAccount } from '@mdi/js'

class App extends Component {
  render() {
    return (
      <Icon path={mdiAccount}
        size={1}
        horizontal
        vertical
        rotate={90}
        color="red"
        spin/>
    )
  }
} 
```

## Props

| Prop       | PropTypes      | Default  | Details |
|------------|----------------|----------|---------|
| path       | string         | required | SVG path data. Usually from @mdi/js |
| size       | number, string | null     | `{size * 1.5}rem`, `'1em'`, `'24px'` |
| horizontal | bool           | `false ` | Flip Horizontal |
| vertical   | bool           | `false`  | Flip Vertical |
| rotate     | number         | `0 `     | degrees `0` to `360` |
| color      | string         | `#000`   | `rgb()` / `rgba()` / `#000` |
| spin       | bool, number   | `false`  | `true = 2s`, `{spin}s` |

<blockquote class="alert alert-info">
  icon:information-outline Learn more about other features including the `Stack` component in the <a href="https://github.com/Templarian/MaterialDesign-React">Repo</a>.
</blockquote>
