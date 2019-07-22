# Whimsy - Bootstrap 4 HTML Theme

Whimsy - Bootstrap 4 HTML Theme

View the <a href="https://steveshead.github.io/bootstrap4-whimsy/">demo</a> site <a href="https://steveshead.github.io/bootstrap4-whimsy/">here</a>.

Also included in this theme is the custom.scss file and an HTML file called elements.html. The custom.scss file is explained below - the elements.html file show the majority of bootstrap 4 elements, and the effect the overrides have on them (color, spacing etc).  

To use the custom.scss set your code editor to compile assets/scss/custom.scss to assets/css/custom.css, and replace bootstrap.css in the head section of my index.html with custom.css.  Note that bootstrap.scss has to be imported at the bottom of the custom.scss file for this to work. For all other theme edits use assets/css/theme.css.

Below are the Bootstrap overrides used in this theme.  

```scss
// override bootstrap default theme colors
$theme-colors: (
  "primary": #375a7f,
  "secondary": #444,
  "success": #00bc8c,
  "info": #3498DB,
  "warning": #F39C12,
  "danger": #E74C3C,
);

// increase the default spacing
$spacer:1.25rem;

// adjust the default heading font weight
$headings-font-weight:300;

// adjust the default font weights
$font-weight-light:200;
$font-weight-normal:300;
$font-weight-bold:500;

// adjust the default font size
$font-size-base:1.2rem;

// add more spacers
$spacer: 1rem !default;
$spacers: (
    6: ($spacer * 4),
    7: ($spacer * 5),
    8: ($spacer * 7.50),
    9: ($spacer * 10)
  );

// set the button border radius
$btn-border-radius:2px;

// change the hyperlink color
$link-color: #00bc8c;

// remove underline from hyperlinks
$link-hover-decoration: none;


// Core bootstrap scss import - this should always be at the bottom of the custom.scss file
@import '../../bootstrap/scss/bootstrap';
```
