# Sealink Ecom Engine CSS

SeaLink Ecom Engine shared styles


### Usage

    gem install sealink-ecom-engine-css --save


### Import the style file to your project main scss/sass

    @import "sealink-ecom-engine-css/sass/ecom"


### Add codes to copy image library

```coffee

  _paths = {
    build_img:    './public/images'
    img_libs: 'node_modules/sealink-ecom-engine-css/lib/images/**/*'
  }

  gulp.task 'img_libs', ->
    gulp.src _paths.img_libs
    .pipe gulp.dest _paths.build_img

  gulp.task 'build', ->
    runSequence ['img_libs', 'js_libs', 'modernizr', 'sass']
```

### Mockup for tooltip

```ruby

  %a{href: "#", title: "#{passenger_type_count.conditions}", "data-placement":"bottom",  "data-toggle":"tooltip"}
    %i.icon-question-sign
```