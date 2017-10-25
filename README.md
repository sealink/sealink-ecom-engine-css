# Sealink Ecom Engine CSS

SeaLink Ecom Engine shared styles


### Usage

    npm install sealink-ecom-engine-css --save


### Import the style file to your project main scss/sass

    @import "sealink-ecom-engine-css/sass/ecom-engine-styles"


### Add codes to copy image library

```coffee

  _paths = {
    build_img:    './public/images'
    img_libs: 'node_modules/sealink-ecom-engine-css/lib/images/***/**/*'
  }

  gulp.task 'img_libs', ->
    gulp.src _paths.img_libs
    .pipe gulp.dest _paths.build_img

  gulp.task 'build', ->
    runSequence ['img_libs']
```

### Markup for tooltip

```html

  <a href='#' data-placement="bottom" data-toggle="tooltip" title="Child age range is 3-14 years">
    <i class="icon-question-sign"></i>
  </a>

```
