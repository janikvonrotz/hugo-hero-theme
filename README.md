# Hugo Hero Theme

Hero is a multi-page, multi-purpose business theme with fullscreen hero images and fullwidth sections.

![Hugo Hero Theme screenshot](/images/screenshot-full.jpg)

## Features

- SCSS (Hugo Pipelines)
- Responsive design
- Robust example content included

## Content Types

### Services


### Work




## DEV

Display breakpoints for DEV

```css
body:after {
  color: #000000;
  font-size: 12px;
  padding: 5px;
  font-weight: bold;
  right: 10px;
  position: fixed;
  text-align: center;
  text-transform: uppercase;
  bottom: 10px;
  width: 200px;
  z-index: 9999;
  border: solid 1px #000000;
  @each $name, $value in $grid-breakpoints {
    @include media-breakpoint-up($name) {
      content: "#{$name} - min-width: #{$value}";
    }
  }
}
```