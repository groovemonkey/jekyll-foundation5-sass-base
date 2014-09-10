# A Base Template For Jekyll and Foundation 5

Sometimes instead of writing world-changing back-end code, I design small static websites. They're simple, so they should be quick to create, but I'd still like them to look good and be easy to work with. I want a usable grid system. I want things to automatically look good on mobile devices. I want to write scss instead of CSS, to stave off carpal tunnel for a few more years.

That's why this template exists. Clone it, and you can be up and running in no time.

It uses:
-Jekyll for static site generation with a few extra features
-Foundation (5.4) as a grid/CSS framework
-Sass/scss for making front-end work bearable
-jquery, normalize/modernizr, and other nice-to-haves already wired together

## Install
-requires that you have ruby + rubygems installed

        gem install jekyll
        gem install compass

## Configure
-delete this readme.md
-create your own git repo for the project:
        rm -rf .git && git init .
-configure foundation base colors + styles
        # $EDITOR _sass/_settings.scss

## Develop
-html for pages just goes in <projectroot> (look at the example index.html)
-snippets you want to reuse on several pages go into _includes
-for the rest, just look at the jekyll tutorial -- http://jekyllrb.com/docs/structure/

-# compass watch # (to continuously update compiled CSS)
-# jekyll serve  # (to keep refreshing + serving the generated site)


## Deploy
-rsync your generated site (in your _site/ directory) to your webserver
        rsync <projectroot>/_site/* user@webhost:/var/www/<yoursite>/




### extra features included:
-modernizr.js
-normalize.css
-foundation icons, ready to use (see http://zurb.com/playground/foundation-icon-fonts-3)
-jquery

