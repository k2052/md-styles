# md-styles: Markdown css themes

A collection of css styles for markdown.

## Installation

Install using npm:

```sh
$ npm install --save md-styles
```

or yarn

```sh
yarn add md-styles
```

## Usage

All the themes are designed to be used as css modules, the styles for
everything are scoped to a `.markdownBody` class. Use it in JSX like
this:

```js
import mdStyles from "md-styles/themes/solarized-light.css";

const Markdown = ({markdown}) => {
  return (
      <div className={mdStyles.markdownBody} >
      {markdown}
      </div>
  )
}
```

And in CSS like this:

```css
.myMarkdownStyles {
  composes: className from "./md-styles/themes/solarized-light.css";
}
```

## Available Themes

- solarized-light

I'll and a bunch more soon! PRs welcome

## TODOS

- [ ] Add screenshots to README

## Is this useless?

It is mostly useless

## License

Licensed under ISC.
