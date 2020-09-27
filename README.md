# Accessible Minimalism Hugo Theme

Minimalist Hugo theme with a penchant for accessibility 

[Demo site](https://accessible-minimalism.netlify.app)

## Project aims

 - XHTML 1.0 Strict valid and HTML 5 friendly code
 - minimal bloat in the generated markup
 - focus on accessibility
   - semantic, minimal markup for screen readers
   - minimal added CSS for partially sighted users
   - easy to read source code
   - minimal config required to get started and use in Hugo
 - RSS subscription support
 - favors fully-blind users over partially or fully sighted users
 - mobile-last development 

## Who is this for?

This aims at users who care more about content and inclusivity than dancing baby
 GIFs or whatever the 2020 equivalent is.

The early web was great for content, unburdened by MBs of JavaScript or CSS.
 RSS feeds allowed users to pull your content on demand vs being forced into
 giving you space in their precious inbox or following your social-ills.

## Getting started

1. In your Hugo site's root, clone this repo to your `themes` dir:

`git clone --depth 1 https://github.com/leonstafford/accessible-minimalism-hugo-theme themes/accessible-minimalism`

It may be preferable to use git's submodule functionality to keep the theme
 within your website's repository. To do this, use:

`git submodule add https://github.com/leonstafford/accessible-minimalism-hugo-theme themes/accessible-minimalism`

*Using the https remote URI will make deployment of your website via some CI/CD,
 such as Netlify, easier.*

2. Copy the `config.toml` file from the exampleSite directory inside this repository to your site root:

`cp themes/accessible-minimalism/exampleSite/config.toml .`

## Configuration

The main things you may want to adjust when using this theme are your content
 structure and main site menu. Copying the `content` directory from this theme's
 `exampleSite` directory will be a good place to start. You can compare this
 with the menu entries in the `config.toml` and it should make sense. Try making
 changes and see what happens. If it becomes a mess, reset both to initial 
 states.

## Development decisions

 - skip redundancy such as anchor's `title` attributes
 - default browser colors are high contrast enough

## Screenshot

[![Screenshot](https://github.com/leonstafford/accessible-minimalism-hugo-theme/blob/master/images/screenshot.png?cb=1234)](https://github.com/leonstafford/accessible-minimalism-hugo-theme/blob/master/images/screenshot.png)

## Testing

 - check theme against [w3c validator](https://validator.w3.org)
 - check using `content` dir from [hugoBasicExample](https://github.com/gohugoio/hugoBasicExample)
 - check using `content` dir from `exampleSite` in this repo
 - check navigation and content in `lynx(1)` browser
 - check navigation and content in screen reader(s)
 - test accessibility in sites like:
   - [wave](https://wave.webaim.org/report#/https://accessible-minimalism.netlify.app)
   - [achecked](https://achecker.ca)

## Roadmap

 - theme options / config help for enabling footer links to email, RSS, socials
 - scriptless search (GET submission to engine + index generation)
 - multilingual site support (includine Hugo's sitemapindex)

### License

[The Unlicense](https://unlicense.org) - do whatever you like with this code.
