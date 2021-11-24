# tailwindcss-themeable

Multiple themes support for tailwindcss and windicss. Developing with one theme and it will work with multiple themes, all you need is just to define your default (for shade `500`) color values for your theme. We will generate all shades from `50` to `900` for you, following the built-in shade name convention of the [default color values](https://tailwindcss.com/docs/customizing-colors).

|Dracula (default theme)|Material|
|-------|--------|
|![dracula](img/dracula.png)|![material](img/material.png)|

Demo Link:

- Windi: https://upupming.site/tailwindcss-themeable/windi/
- Tailwind: https://upupming.site/tailwindcss-themeable/tailwind/

Demo source code:

- [Windi](examples/windi/index.html)
- [Tailwind](examples/tailwind/index.html)

## Installation

```bash
npm i tailwindcss-themeable
```

## Usage

We define the color names following [the dracula contribute color palette](https://draculatheme.com/contribute).

CSS variables are generated from build time, and added to the corresponding scope for usage.

Configuration:

```ts
// windi.config.ts or tailwind.config.js
import { themeable } from 'tailwindcss-themeable'
// or: const { themeable } = require('tailwindcss-themeable')

plugins: [
    themeable({
      themes: [
        {
          name: 'example-theme',
          palette: {
            background: '#282A36',
            foreground: '#F8F8F2',
            selection: '#44475A',
            comment: '#6272A4',
            cyan: '#8BE9FD',
            green: '#50FA7B',
            orange: '#FFB86C',
            pink: '#FF79C6',
            purple: '#BD93F9',
            red: '#FF5555',
            yellow: '#F1FA8C'
          }
        }
      ]
    })
  ]
```

<details>

<summary>Generated CSS</summary>

```css
.themeable-example-theme {
    --themeable-background-50: 121, 126, 156;
    --themeable-background-100: 110, 115, 147;
    --themeable-background-200: 92, 97, 124;
    --themeable-background-300: 75, 78, 101;
    --themeable-background-400: 57, 60, 77;
    --themeable-background-500: 40, 42, 54;
    --themeable-background-600: 16, 17, 22;
    --themeable-background-700: 0, 0, 0;
    --themeable-background-800: 0, 0, 0;
    --themeable-background-900: 0, 0, 0;
    --themeable-background: 40, 42, 54;
    --themeable-foreground-50: 255, 255, 255;
    --themeable-foreground-100: 255, 255, 255;
    --themeable-foreground-200: 255, 255, 255;
    --themeable-foreground-300: 255, 255, 255;
    --themeable-foreground-400: 255, 255, 255;
    --themeable-foreground-500: 248, 248, 242;
    --themeable-foreground-600: 228, 228, 206;
    --themeable-foreground-700: 209, 209, 169;
    --themeable-foreground-800: 189, 189, 133;
    --themeable-foreground-900: 169, 169, 96;
    --themeable-foreground: 248, 248, 242;
    --themeable-selection-50: 159, 162, 183;
    --themeable-selection-100: 147, 151, 174;
    --themeable-selection-200: 124, 129, 156;
    --themeable-selection-300: 103, 108, 136;
    --themeable-selection-400: 86, 89, 113;
    --themeable-selection-500: 68, 71, 90;
    --themeable-selection-600: 44, 46, 58;
    --themeable-selection-700: 20, 21, 26;
    --themeable-selection-800: 0, 0, 0;
    --themeable-selection-900: 0, 0, 0;
    --themeable-selection: 68, 71, 90;
    --themeable-comment-50: 214, 218, 231;
    --themeable-comment-100: 201, 207, 224;
    --themeable-comment-200: 175, 184, 209;
    --themeable-comment-300: 150, 160, 194;
    --themeable-comment-400: 124, 137, 179;
    --themeable-comment-500: 98, 114, 164;
    --themeable-comment-600: 76, 89, 130;
    --themeable-comment-700: 55, 65, 95;
    --themeable-comment-800: 34, 40, 59;
    --themeable-comment-900: 14, 16, 24;
    --themeable-comment: 98, 114, 164;
    --themeable-cyan-50: 255, 255, 255;
    --themeable-cyan-100: 255, 255, 255;
    --themeable-cyan-200: 255, 255, 255;
    --themeable-cyan-300: 219, 248, 254;
    --themeable-cyan-400: 179, 241, 254;
    --themeable-cyan-500: 139, 233, 253;
    --themeable-cyan-600: 84, 223, 252;
    --themeable-cyan-700: 29, 212, 251;
    --themeable-cyan-800: 4, 182, 220;
    --themeable-cyan-900: 3, 136, 165;
    --themeable-cyan: 139, 233, 253;
    --themeable-green-50: 255, 255, 255;
    --themeable-green-100: 239, 255, 243;
    --themeable-green-200: 199, 253, 213;
    --themeable-green-300: 159, 252, 183;
    --themeable-green-400: 120, 251, 153;
    --themeable-green-500: 80, 250, 123;
    --themeable-green-600: 25, 248, 82;
    --themeable-green-700: 6, 212, 58;
    --themeable-green-800: 4, 157, 43;
    --themeable-green-900: 3, 103, 28;
    --themeable-green: 80, 250, 123;
    --themeable-orange-50: 255, 255, 255;
    --themeable-orange-100: 255, 255, 255;
    --themeable-orange-200: 255, 243, 230;
    --themeable-orange-300: 255, 223, 190;
    --themeable-orange-400: 255, 204, 149;
    --themeable-orange-500: 255, 184, 108;
    --themeable-orange-600: 255, 157, 52;
    --themeable-orange-700: 251, 130, 0;
    --themeable-orange-800: 195, 101, 0;
    --themeable-orange-900: 139, 72, 0;
    --themeable-orange: 255, 184, 108;
    --themeable-pink-50: 255, 255, 255;
    --themeable-pink-100: 255, 255, 255;
    --themeable-pink-200: 255, 243, 250;
    --themeable-pink-300: 255, 203, 233;
    --themeable-pink-400: 255, 162, 215;
    --themeable-pink-500: 255, 121, 198;
    --themeable-pink-600: 255, 65, 174;
    --themeable-pink-700: 255, 9, 150;
    --themeable-pink-800: 208, 0, 119;
    --themeable-pink-900: 152, 0, 87;
    --themeable-pink: 255, 121, 198;
    --themeable-purple-50: 255, 255, 255;
    --themeable-purple-100: 255, 255, 255;
    --themeable-purple-200: 255, 255, 255;
    --themeable-purple-300: 236, 224, 253;
    --themeable-purple-400: 213, 186, 251;
    --themeable-purple-500: 189, 147, 249;
    --themeable-purple-600: 157, 94, 246;
    --themeable-purple-700: 124, 41, 243;
    --themeable-purple-800: 96, 12, 216;
    --themeable-purple-900: 72, 9, 163;
    --themeable-purple: 189, 147, 249;
    --themeable-red-50: 255, 255, 255;
    --themeable-red-100: 255, 248, 248;
    --themeable-red-200: 255, 207, 207;
    --themeable-red-300: 255, 167, 167;
    --themeable-red-400: 255, 126, 126;
    --themeable-red-500: 255, 85, 85;
    --themeable-red-600: 255, 29, 29;
    --themeable-red-700: 228, 0, 0;
    --themeable-red-800: 172, 0, 0;
    --themeable-red-900: 116, 0, 0;
    --themeable-red: 255, 85, 85;
    --themeable-yellow-50: 255, 255, 255;
    --themeable-yellow-100: 255, 255, 255;
    --themeable-yellow-200: 255, 255, 255;
    --themeable-yellow-300: 251, 253, 218;
    --themeable-yellow-400: 246, 252, 179;
    --themeable-yellow-500: 241, 250, 140;
    --themeable-yellow-600: 234, 248, 86;
    --themeable-yellow-700: 228, 245, 32;
    --themeable-yellow-800: 196, 212, 9;
    --themeable-yellow-900: 146, 159, 7;
    --themeable-yellow: 241, 250, 140;
}
```

</details>

Then you can wrap you HTML elements with `themeable-example-theme` class to use the `example-theme` theme! All `text-themeable-*` class uses the CSS variable from the generated CSS of your configuration. `tailwindcss-themeable` already has two built-in themes (`dracula` and `material`) you can use directly.

```html
<div class="themeable-example-theme">
    <div class="text-themeable-foreground">
        Hello world!
    </div>
</div>
<div class="themeable-dracula">
    <div class="text-themeable-foreground">
        Hello world!
    </div>
</div>
<div class="themeable-material">
    <div class="text-themeable-foreground">
        Hello world!
    </div>
</div>
```

<hr>

You can specify all the shades of a color if you want:

```js
themeable({
      themes: [
        {
          name: 'theme-example',
          palette: {
            background: {
                // Replace the hex color value with whatever your like
                 '50': '#000000',
                '100': '#000000',
                '200': '#000000',
                '300': '#000000',
                '400': '#000000',
                '500': '#000000',
                '600': '#000000',
                '700': '#000000',
                '800': '#000000',
                '900': '#000000',
                DEFAULT: '#000000',
            }
            //...
          }
      ]
})
```

Extra configurations:

```ts
interface ThemeableOptions {
    /**
     * Support a list of theme definitions, the user should define the colors of the theme follow the contribute of Dracula theme.
     * See https://draculatheme.com/contribute#color-palette
     * @default []
     */
    themes?: Theme[];
    /**
     * Prefix of the class to enable a theme, for example the container with class `${classPrefix}-dracula` will enable dracula theme in its children elements
     * @default `themeable`
     */
    classPrefix?: string;
    /** The lighten step for auto generated shades smaller than the default `500` color
     * For example, if you passed `#50FA7B` as the `green` theme key, and `shadeLightenStep` is 8,
     * then we will use this color as the `DEFAULT` and shade `500` to generate all other shades of `green`,
     * for shade smaller than `500`, we will add the lightness up `shadeLightenStep` in per 100 gap.
     * Color `#50FA7B` converted to HSL is [135, 94, 64], so the shade `400` will be computed to [135, 94, 72]
     * @default 8
     */
    shadeLightenStep?: number;
    /** Similar with `shadeLightenStep` but for shades larger than `500`
     * @default 11
     */
    shadeDarkenStep?: number;
    /** When not specify any theme in HTML, the `defaultTheme` will be used
     * @default `dracula`
     */
    defaultTheme?: string;
}
```

## Reference

1. https://github.com/dracula/tailwind
2. https://github.com/anheric/tailwindshades
3. [Theming Tailwind with CSS Variables](https://www.youtube.com/watch?v=MAtaT8BZEAo)
