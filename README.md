This project uses [Quickshot](https://quickshot.readme.io/) and [Compass](http://compass-style.org/) to handle local development. 

Workflow is based off [this](http://code-shopify.herokuapp.com/blog_posts/shopify-development-flow-sass-compass-and-liquid) model. Instead of using the Shopify Theme Gem, we're using Quickshot instead.

In your terminal, you'll have two tabs open, one for `qs theme watch` and another for `compass watch`.

#SCSS
Using Quickshot allows us to to sync our scss files to Shopify. Using Compass allows us to compile regular scss files (with full scss functionality, not the limited Shopify way) to scss.liquid files, which Quickshot watches for and compiles to regular css. This css file is then uploaded to Shopify.

This gives us full scss functionality, and with some minor mixins + [liquid escaping](https://github.com/luciddesign/bootstrapify/wiki/Escaping-liquid-in-SASS), we can now leverage both scss and Liquid to their fullest.