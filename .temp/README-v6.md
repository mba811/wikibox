# jekyll-wikibox

This project is supposed to serve as foundation of a responsive and flexible guerilla wiki for hackers.
It transfers your markdown/textile notes to satic html layout inspired by sublime text editor.

- **[Features](#features)** or what is it about?
  - Functional Features
  - Appearance
- **[Usage](#usage)** or how can I use it?
  - Live Demo
  - Installation
  - Local Deployment
  - Web Deployment
  - Customization
  - Themes
- **[Project Planning](#project-planning)** or how can I improve it?
  - Important Files
  - Project Structure
- **[References](#references)** or how does it work?
  - Core Technologies
  - Related Technologies
  - Markup Languages
  - Higher-Level Languages
  - Feature Inspirations
  - Design Inspirations
  - Design Frameworks

## Features

### Functional Features

  - multiple boxes/repositories (blogs) for notes (markdown, textile)
  - sort by date created

### Appearance
  
  - Sublime Text Theme
  - Paint Bucket Theme

## Usage

### Live Demo

- Available via `branch gh-pages` (github pages)  
  `http://dataduke.github.com/jekyll-wikibox` (to be done)

### Installation

1. install ruby
2. install jekyll `sudo gem install jekyll`
3. fork/clone/check out this github project

### Local Deployment

1. change to `cd ~/github/jekyll-wiki`
2. run `jekyll --server` 
3. open `http://localhost:4000/`

### Web Deployment

- GitHub Hosting: Please refer to github pages help.
- Other web hoster: Please refer to jekyll wiki/help.

### Customization

    ./_config.yml           # configuration
    ./_themes/themename     # themes; move all files/folders contained in a theme to root folder (and override)

### Themes

Sublime Text [README](https://github.com/dataduke/jekyll-wikibox/tree/master/_themes/sublimetext)  

![Version alpha.03 - Sublime Text](https://raw.github.com/dataduke/jekyll-wikibox/master/_themes/sublimetext/_sublimetext.jpg)

Paint Bucket [README](https://github.com/dataduke/jekyll-wikibox/tree/master/_themes/paintpucket)  

![Version alpha.03 - Paint Bucket](https://github.com/dataduke/jekyll-wikibox/raw/master/.info/snapshot-version-a03-paintbucket.jpg)

## Project Planning

### Important Files

    ./README.md                       # contains general information
    ./CHANGELOG.md                    # contains version history
    ./BACKLOG.md                      # contains initial feature backlog (backup/reminder)
    ./JEKYLL-WIKIBOX.taskpaper        # contains planned features and current backlog

### Project Structure

    .
    |-- .info                         # can be ignored; used for project information only
    |-- .temp                         # can be ignored; used at development for backup of important files
    |-- _includes                     # used for building index pages
    |   |-- main-index-sidebar.md
    |   |-- main-index-box-N.md
    |   |-- box-N-index-sidebar.md
    |   |-- box-N-index.md
    |-- _layouts
    |   |-- default.html
    |   |-- post.html
    |-- _themes             
    |-- _site                         # not checked in; created by jekyll as deployment directory
    |-- _plugins 
    |   |-- additional-feature-X
    |-- assets                        # for layout dependencies only
    |   |-- css
    |       |-- style.css
    |   |-- img
    |   |-- js
    |   |-- favicon.ico
    |-- box000                        # box001-005; more boxes can be added/renamed/deleted
    |   |-- _posts
    |   |   |-- 2013-01-01-hello-world.markdown    # .md or .textile or .taskpaper
    |   |   |-- 2013-01-01-hello-world             # folder for post attachments
    |   |       |-- attachment-1.jpg
    |   |       |-- attachment-2.pdf
    |   |-- atom.xml
    |   |-- index.html
    |-- _config.yml
    |-- index.html
    |-- atom.xml

## References

### Acknowledgments

### Core Technologies

- [ruby](http://www.ruby-lang.org/en/)
- [jekyll](https://github.com/mojombo/jekyll)

### Related Technologies

- [jekyll-asset-pipeline](https://github.com/matthodan/jekyll-asset-pipeline), [blogpost](http://matthodan.com/2012/11/22/jekyll-asset-pipeline.html)
- [jekkll-asset_bundler](https://github.com/moshen/jekyll-asset_bundler)
- [jekyll-bootstrap](https://github.com/plusjade/jekyll-bootstrap) 
- [multi-blog-jekyll](https://github.com/ggarron/multi-blog-jekyll)
- [github pages](http://pages.github.com/), [help](https://help.github.com/categories/20/articles) 
- [octopress](https://github.com/imathis/octopress)
- [ruhoh](http://ruhoh.com)

### Markup Languages

- [markdown](http://daringfireball.net/projects/markdown/) by John Gruber
- [multimarkdown](http://fletcherpenney.net/multimarkdown/) by Fletcher Penny
- [github flavored markdown](https://help.github.com/articles/github-flavored-markdown) by GitHub
- [textile](http://textism.com/tools/textile/) by Dean Allan
- [taskpaper](http://www.hogbaysoftware.com/products/taskpaper) by Jesse Grosjea

### Higher-Level Languages

- [YAML](http://www.yaml.org): data serialization;
- [{{ mustache }}](http://mustache.github.com), [js-github-repo](https://github.com/janl/mustache.js): tag expansion;
- [Sass](http://sass-lang.com): CSS3 abstraction; .scss or .sass;
- [Haml](http://haml.info), [doc](http://haml.info/docs/yardoc/file.REFERENCE.html): HTML abstraction; .html.haml;
- [less](http://lesscss.org/), [github-repo](https://github.com/cloudhead/less.js): CSS3 extension for dynamic behaviour (variables etc.);
- [liquid](http://www.liquidmarkup.org/), [help](https://github.com/mojombo/jekyll/wiki/liquid-extensions), [github-repo](https://github.com/Shopify/liquid), [wiki](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers): template system;
- [ERuby](http://de.wikipedia.org/wiki/ERuby), [erb](http://ruby-doc.org/stdlib-1.9.3/libdoc/erb/rdoc/ERB.html): Ruby templating; .erb, .html.erb, .xml.erb;
- [CoffeeScript](http://coffeescript.org/): JavaScript abstraction;

### Feature Inspirations

 - **PoIC** (Pile of Index Cards), [Wiki](http://pileofindexcards.org/), [Blog](http://pileofindexcards.org/blog/)

### Design Inspirations

- **Sublime Text** Theme, [Sublime Text Editor](http://www.sublimetext.com/), [Soda-Dark.sublime-theme](https://github.com/buymeasoda/soda-theme), [Monokai-Soda.tmtheme](https://github.com/simeonv/st2-color-schemes)

### Design Frameworks

- [jQuery UI](http://jqueryui.com/)
- [Twitter Bootstrap](http://twitter.github.io/bootstrap/), [github-repo](https://github.com/twitter/bootstrap)
