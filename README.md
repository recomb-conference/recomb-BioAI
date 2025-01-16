# RECOMB-BioAI Website Template

### About
This project is the website template and content used for RECOMB-BioAI, see the live website at https://recomb.org/recomb-BioAI 

#### The main files to edit

* _config.yml: some data such as dates, location etc
* history.md: history page to be updated after the conference
* history/  : folder with archived information for each year
* _data/pc.yml: list of PC (perhaps it would be easier to do simply im html)
* _data/speakers.yml: keynote spekers with bio + abstract, used on two places (keynotes and program)
* _data/team.yml: PC chairs and SC
* _includes/about.html: home page with basic info
* _includes/posters.html: plain html list of posters
* _includes/schedule-tbd.html: plain html schedule (earlier used to post the list of accepted papers; NOTE: the file used for RECOMB-seq 2024 is _includes/schedule2024.html; this file name is specified in schedule.html)
* CfP used by RECOMB-seq 2024 locates at _paper-calls/RECOMB-2024-CfP.md

Some of the unused files were moved to _unused folder; more can be moved as well.

### Software

This site is based on [Project Zeppelin](https://github.com/gdg-x/zeppelin). Project Zeppelin is built on top of [Jekyll](http://jekyllrb.com/) - simple, blog-aware, static site generator. Jekyll also happens to be the engine behind GitHub Pages, which means you can use Jekyll to host your website from GitHub’s servers for free. [Learn more about Jekyll](http://jekyllrb.com/). Template is brought by [GDG Lviv](http://lviv.gdg.org.ua/) team.

### Features
* Easy to setup
* Simple and responsive design
* Integrated speakers and sessions management
* SVG icons
* SEO friendly

### Quick-start guide
1. Clone locally this repo
2. Update ```_config.yml```
3. Select what content blocks do you need
4. Push changes to ```gh-pages``` branch

## Local development

Check if you have [all requirements for local environment](http://jekyllrb.com/docs/installation/).
To install all development dependencies install [Bundler](http://bundler.io/).
```bash
    gem install bundler
```
and run next command from root folder:

```bash
  bundle install
```  

To start Jekyll run:
```bash
    jekyll serve -w
```
Site will be available at http://127.0.0.1:4000/zeppelin/ or http://localhost:4000/zeppelin/ (on Windows)

**NOTE:** in this mode all changes to html and data files will be automatically regenerated, but after changing ```_config.yml``` you have to restart server.

### Sass(Compass) support
**Note:** You need to install [Node.js](http://nodejs.org/download/)

To watch changes of `.sass` files and compile it to the `.css` on a fly change property `safe: true` to `safe: false` in `_config.yml`.
**Note: It works only on local machine, because GitHub runs Jekyll in `--save` [mode](https://help.github.com/articles/using-jekyll-with-pages/#configuration-overrides)**

Learn more about Sass development from [documentation](https://github.com/gdg-x/zeppelin/wiki/Sass-development).


### Resource optimizations (optional)

You can optimize images and minify css and javascript automatically (for now only on Windows).
But for Mac OS users available amazing tool - [imageoptim](https://imageoptim.com/). Thanks [@raphaelsavina](https://github.com/raphaelsavina) for link.
Optimize all images by running this script from `/automation/images/` folder:
```bash
    all_image_optimization.bat -d -jtran -pout -pquant -optip -gsicle -svgo
```

To minify CSS and JS run `minify_js.bat` (for Windows) and `minify_js.sh` (for Linux and MacOS) from `/automation/minifying/` folder:
```bash
    minify_js.bat
```

Learn more about available optimization options from [documentation](https://github.com/gdg-x/zeppelin/wiki/Resources-optimizations).

### Documentation
Quick-start guide is not enough? Checkout [full documentation](https://github.com/gdg-x/zeppelin/wiki).

### Used libraries
* [Bootstrap](https://github.com/twbs/bootstrap)
* [Animate.css](https://github.com/daneden/animate.css)
* [Waves](https://github.com/publicis-indonesia/Waves)
* [jquery.appear](https://github.com/bas2k/jquery.appear)
* [jQuery countTo Plugin](https://github.com/mhuggins/jquery-countTo)
* [Typed.js](https://github.com/mattboldt/typed.js)
* [Sticky-kit](https://github.com/leafo/sticky-kit)


### License
Project is published under the [MIT license](https://github.com/recomb-seq/recomb-seq.github.io/blob/main/LICENSE.txt). 
