# Responsive Starter Kit Pro #

A highly functional toolkit to help jump-start a typical responsive web design project. This is a full-featured variation of the more basic [responsive starter kit](https://github.com/mpgilbertusa/Responsive-Starter-Kit) which was primary created for instructional purposes to introduce basic RWD concepts. This version includes the LESS pre-processor as well as a handful of add-ons for typical responsiveness and can be used on a variety of real-world projects.

Sample HTML files are included to demonstrate possible layouts: style guide/sampler, left sidebar, right sidebar, three columns, full width, sample form, and audio/video transcript. There's a basic *theme.css* file in the *assets/style* directory. Feel free to edit, or even delete, this file as needed. It's been included for demonstration purposes only. It's not intended to influence visual and/or user experience design preferences.

## Demo ##

A [browsable demo](https://rawgithub.com/mpgilbertusa/Responsive-Starter-Kit-Pro/master/index.html) of all layout pages is available.

## General ##

* **Responsive** layout with a fluid/elastic grid, not *adaptive* with multiple fixed-width breakpoints
* Prefererence for **readability over compression** for HTML and CSS coding style; can minify using CSS pre-processor (or server) - http://isobar-idev.github.com/code-standards/

## HTML ##

* Modified version of *HTML5 Reset v2* by Tim Murtaugh - http://html5reset.org/
* Uses the new HTML5 section tags: HEADER, FOOTER, NAV, SECTION, ARTICLE, ASIDE
* Doesn't use the new HTML5 outline algorithm
* Doesn't use XHTML-style trailing "space and slash" on self-closing elements such as INPUT, META, IMG, BR, HR, etc.
* Meta viewport tag set to "width=device-width, initial-scale=1.0" (causes a documented iPad orientation change zoom bug)

## CSS ##

* LESS CSS pre-processor with mixins, nesting, inline media queries, and external variables file CodeKit or LESS.app complier for Mac (SimpLESS available on Windows)
* Assorted mixins for border-radius, box-shadow, linear gradients, etc. based on work from LESS Elements and Preboot
* Mobile first technique emphasizing **progressive enhancement**
* Proportional media queries - http://blog.cloudfour.com/the-emshave-it-proportional-media-queries-ftw/
* Don't Overthink It Grids - http://css-tricks.com/dont-overthink-itgrids/
* Column widths use %, fixed-width gutters use px, fonts use em, images use "max-width: 100%" and "height: auto"
* *Box-sizing: Border-box* for everything - http://paulirish.com/2012/box-sizing-border-box-ftw/
* Uses unitless line-heights for typography - http://meyerweb.com/eric/thoughts/2006/02/08/unitless-line-heights/
* .gitignore file excludes all CSS files (only versioning LESS files to avoid compile conflicts caused by pre-processor)

## JavaScript ##

* jQuery 1.9.1 for IE 8 and below support
* Loading jQuery from GoogleAPIs.com for caching
* Collapsible content sections for small screens (expanded for everything else)

## Add-ons ##

* Modernizr for feature detection - http://modernizr.com/
* Zurb Responsive Tables (for data tables) - https://github.com/zurb/responsive-tables
* jQuery Validate for client-side validation on forms - http://bassistance.de/jquery-plugins/jquery-plugin-validation/
* Riloadr (images, including Retina and scroll position support) - https://github.com/tubalmartin/riloadr
* FitVids (videos) - https://github.com/davatron5000/FitVids.js
* fancyBox (modal dialogs) - https://github.com/fancyapps/fancyBox
* WooThemes FlexSlider (content carousel) - https://github.com/woothemes/FlexSlider
* Modernizr (feature detection) - https://github.com/Modernizr/Modernizr

## IE 8 ##

* Includes *Respond.js* and *HTML5 Shim/Shiv* for media query support
* CSS overrides specified with *.ie8* selectors, added as multiple conditional comments to HTML tag, if needed

## Accessibility ##

* Semantic HTML throughout
* WAI-ARIA Landmark Roles: banner, navigation, main, complementary, contentinfo - http://a11yproject.com/posts/aria-landmark-roles/
* Forms include LABELs and TITLEs on INPUT fields
* Alt text for images, unless no content conveyed - http://a11yproject.com/posts/alt-text/
* Doesn't include "maximum-scale=1.0" in META VIEWPORT tag - http://a11yproject.com/posts/never-use-maximum-scale/