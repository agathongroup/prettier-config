# Agathon's [prettier](https://prettier.io) configuration

## Installation

**1. Install dependencies:**

```sh
yarn add --dev @agathongroup/prettier-config prettier
```

**2. Create a `prettier.config.js` file at the root of your project and add the following:**

```js
module.exports = require('@agathongroup/prettier-config');
```

## [Editor Integration](https://prettier.io/docs/en/editors.html)

### VS Code

1. Install Prettier extension: `View → Extensions` then search and install Prettier - Code formatter
2. You may need to reload the editor
3. In your user settings `Code -> Preferences -> Settings` add `editor.formatOnSave: true`

### Sublime Text

[https://packagecontrol.io/packages/JsPrettier](https://packagecontrol.io/packages/JsPrettier)

## Enforced Rules

Check out all of Prettier's [configuration options](https://prettier.io/docs/en/options.html).

- **Print Width** - Wrap lines at 100 characters.

- **Tab Width** - 2 spaces per indentation-level.

- **Tabs** - Indent lines with spaces, not tabs.

- **Semicolons** - Always print semicolons at the ends of statements.

- **Quote** - Use single quotes instead of double quotes. JSX ignores this rule.

- **Trailing Commas** - Use trailing commas wherever possible. Example:

  ```js
  const obj = {
    a: 'hi',
    b: 'hey',
  };
  ```

- **Bracket Spacing** - Print spaces between brackets in object literals.

- **JSX Brackets** - Put the closing `>` of a multi-line JSX element at the end of the last line instead of being alone on the next line (does not apply to self closing elements). Example:

  ```jsx
  <button
  className="prettier-class"
  id="prettier-id"
  onClick={this.handleClick}>
    Click Here
  </button>
  ```

- **Arrow Function Parentheses** - No parentheses around a sole arrow function parameter. Example:

  ```js
  x => x;
  ```
