# styled-blueprintjsx

This package wraps up [Blueprint](https://blueprintjs.com/) styles as a styled-components global style to subvert the need for a CSS loader.

```jsx
import { BlueprintCSS } from "@nteract/styled-blueprintjsx

<React.Fragment>
  <SuperCoolComponent />
  <BlueprintCSS />
</React.Fragment>
```

## Installation

```
npm install --save @nteract/styled-blueprintjsx
```

## Documentation

### With `@blueprintjs/core`

When working with `@blueprintjs/core` components, they need some globally defined (yet scoped) CSS. You can include this on the page with

```jsx
import { BlueprintCSS } from "@nteract/styled-blueprintjsx

<React.Fragment>
  <SuperCoolComponent />
  <BlueprintCSS />
</React.Fragment>
```

### With `@blueprintjs/select`

For `@blueprintjs/select`'s suite of components, you need to include `<BlueprintSelectCSS />` from this package.

```jsx
import { BlueprintCSS, BlueprintSelectCSS } from "@nteract/styled-blueprintjsx

<React.Fragment>
  <SuperCoolComponent />
  <BlueprintCSS />
  <BlueprintSelectCSS />
</React.Fragment>
```

styled-blueprintjsx makes use of [`createGlobalStyle` from `styled-components`](https://www.styled-components.com/docs/api#createglobalstyle) and so is a React Component you can render anywhere in your app. You can read more about this pattern in the styled-components docs linked above.

## Support

Please post an issue on the [issue tracker](https://github.com/nteract/styled-blueprintjsx/issues).

## License

[BSD-3-Clause](https://choosealicense.com/licenses/bsd-3-clause/)
