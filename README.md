# css-tricks

### A simple margins & paddings file
##### margins.sass
```
@for $i from 0 through 100
  .mar#{$i}
    margin: #{$i}px
  .mar-top#{$i}
    margin-top: #{$i}px
  .mar-top-#{$i}
    margin-top: -#{$i}px
  .mar-bot#{$i}
    margin-bottom: #{$i}px
  .mar-bot-#{$i}
    margin-bottom: -#{$i}px
  .mar-lef#{$i}
    margin-left: #{$i}px
  .mar-lef-#{$i}
    margin-left: -#{$i}px
  .mar-rig#{$i}
    margin-right: #{$i}px
  .mar-rig-#{$i}
    margin-right: -#{$i}px
  .pad#{$i}
    padding: #{$i}px
  .pad-rig#{$i}
    padding-right: #{$i}px
  .pad-lef#{$i}
    padding-left: #{$i}px
  .pad-bot#{$i}
    padding-bottom: #{$i}px
  .pad-top#{$i}
    padding-top: #{$i}px
  .top#{$i}
    top: #{$i}px
```

### Mixins for bootstrap & others
##### mixins.scss
```
@mixin transition($transition...) {
  -moz-transition:    $transition;
  -o-transition:      $transition;
  -webkit-transition: $transition;
  transition:         $transition;
}

@mixin xl {
  @media (min-width:1500px) { @content; }
}

@mixin md {
  @media (max-width:$screen-md-max) { @content; }
}

@mixin sm {
  @media (max-width:$screen-sm-max) { @content; }
}

@mixin xs {
  @media (max-width:$screen-xs-max) { @content; }
}

@mixin rotate($deg) {
  transform: rotate($deg);
  -moz-transform: rotate($deg);
  -webkit-transform: rotate($deg);
  -o-transform: rotate($deg);
  -ms-transform: rotate($deg);
}

```

