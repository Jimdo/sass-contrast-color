# sass-contrast-color
> Mixin to get the color with higher contrast

## Install

1. Install the bower component to your project:
```
  bower install Jimdo/sass-contrast-color --save-dev
```

2. Import the Sass file into your code:
```sass
  @import "bower_components/sass-contrast-color/contrast.sass"
```
Or if you're using SCSS:
```scss
  @import "bower_components/sass-contrast-color/contrast.scss";
```
Adjust the tree to your project.

## Usage

```sass
  +contrast($attribute, $base-color, $color1, $color2)
```
### Parameter:

* $attribute - set the attribute where to write the value
* $base-color - set the basic color
* $color1 - first color to compare with base-color
* $color2 - second color to compare with base-color

### Example 

```sass
  body
    background-color: red
    +contrast(color, red, black, white)
```

The example will compare black and white with red and give back the more higher contrast color.

See the compiled CSS code:

```css
  body {
    background-color: red;
    color: white;
  }
```
