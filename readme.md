# A Base Template For Jekyll and Foundation 5

I wanted a few features from a base template:

-Jekyll for static site generation with a few extra features
-Foundation (5.4) as a grid/CSS framework
-Sass/scss for making front-end work bearable

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
-# develop happily
-# compass watch # (to continuously update compiled CSS)
-# jekyll serve  # (to keep refreshing + serving the generated site)


## Deploy
-rsync your generated site (in your _site/ directory) to your webserver
        rsync <projectroot>/_site/* user@webhost:/var/www/<yoursite>/


