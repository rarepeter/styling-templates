# Tool to work with design mockups and make your adaptive websites feel awesome!

### The file **_adaptive_units.scss** is used to transform pixel units in rem/em units in your SCSS styling sheets.
### The file **_adaptive.scss** is used to adapt the size/padding/margins of your elements based on the screen size of the viewport.
# How it solves your problems as a developer:

- Transforms **pixel units** from your mockup designs in **Figma** or **Adobe XD** to adaptive **rem/em** units in your SCSS styling sheets.
- **Adapts the size/padding/margins of your elements dynamically** based on the screen size of the user viewport instead of using percentages.

# How to use the file **_adaptive_units.scss**:

- First, import it into your project:
At the beginning of the file you want to use it in, import the file using the SCSS syntax:

```css
@import './_adaptive_units.scss';
```

- Use it for a property:
For example, if you want to transform the font size of 24 pixels into rem, use the following line:
```css
font-size: rem(24);
```

The output css file will have the following line in it:

```css
font-size: 1.5rem;
```

# How to use the file **_adaptive.scss**:

- First, import it into your project:
At the beginning of the file you want to use it in, import the file using the SCSS syntax:

```css
@import './_adaptive.scss';
```

- Use it to dynamically adapt the width of a div container:

```css
div {
    adaptive-value('width', 200, 100);
}
```
The following will tell the **div** to be its maximum size of 200 pixels when the viewport is 1920px wide, and to be 100 pixels when the viewport is at its minimum size of 320px.

Try the code in your project to see how it works.