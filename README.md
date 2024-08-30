# Theme Toggle

WIP

A styled web component for selecting dark or light theme.

If no theme is yet set, it will figure out the default theme by checking prefered color scheme.

Current theme will be set as a data-attribute on `body` like so: `<body data-theme="dark">`.

Stores current theme choice in localStorage.

## Usage

Put js and css file in the same folder and include theme-toggle.js.

```html
<body>
    <theme-toggle></theme-toggle>

    <script type="module" src="/path/theme-toggle.js"></script>
</body>
```

You can then control your themes like so:

```css
[data-theme="light"] {
    --color-bg: #FFFFFF;
    --color-fg: #000000;
}

[data-theme="dark"] {
    --color-bg: #000000;
    --color-fg: #FFFFFF;
}

body {
    background-color: var(--color-bg);
    color: var(--color-fg);
}
```