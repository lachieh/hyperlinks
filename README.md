# hyperlinks

Extension for [HyperTerm](https://hyperterm.org) that automatically links URLs with the iTerm behavior.

Forked from [zeit/hyperlinks](https://github.com/zeit/hyperlinks).

![Demo](https://cloud.githubusercontent.com/assets/775227/16933009/4fd309a0-4d85-11e6-99b5-720185f4b7d8.gif)

## How to use

1. Install [HyperTerm](https://hyperterm.org/#installation) (obvi...)
2. Install this plugin via npm:
````
npm install hyperlinks-iterm
````
3. add `hyperlinks-iterm` to `plugins`
in `~/.hyperterm.js`:
````
plugins: [
  "hyperlinks-iterm"
],
````

4. hold the `Command` key to activate and highlight links, then click one to open it in your default browser.

## Customizing styles

Add custom styles to `termCSS` in your `~/.hyperterm.js`. Changing the styles for `x-screen a` isn't recommended, because without holding `cmd`, the links won't work anyway.

```js
termCSS: `
  x-screen a {
    color: #ffffff;
    text-decoration: none;
    cursor: text;
  }

  x-screen a.active {
    color: #ff2e88;
    text-decoration: underline;
  }

  x-screen a.active.hover {
    text-decoration: none;
    cursor: pointer;
  }
`
```


## License

MIT
