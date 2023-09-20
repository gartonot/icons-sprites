# Sprites svg

> 1. Create svg file, contains all icons
> 2. Specify default svg tag, without width, height, viewbox etc.
> 3. Put your svg icon in main file with icons and replace `<svg>` to `<symbol>`, clear all atributes, except viewBox
> 4. Add id for symbol icon
> 5. In place needed icon create svg tag with inner tag <use>
> 6. Add attribute href for use `<use href="PATH_TO_ICONS_FILE">`
> 7. Specify the id icon in the path

## Example

>icons.svg
```svg
    <svg xmlns="http://www.w3.org/2000/svg">
        <symbol id="ID_NAME" viewBox="0 0 16 17">
            // here svg inner
        </symbol>
    <svg>
```

>index.html
```html
...
<body>
    <svg width="16" height="16">
        <use href="images/icons.svg#ID_NAME" />
    </svg>
</body>
...
```
