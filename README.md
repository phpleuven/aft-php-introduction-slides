# AFT Skeleton Presentation

## Requirements

* NodeJS and NPM ([https://nodejs.org](https://nodejs.org))
* Yeoman ([http://yeoman.io](http://yeoman.io))
* GruntJS ([http://gruntjs.com](http://gruntjs.com))
* SASS ([http://sass-lang.com/install](http://sass-lang.com/install))

## Setup

* Clone this repository, and copy all contents except for the `.git` folder over to your own repository.
* Change your presentation title in:
    * `index.html`
    * `templates/_index.html`
    * `bower.json` (package name)
* To enable deploying to Github Pages, change your repository location in `Gruntfile.coffee`:

         buildcontrol:
            ...
            pages:
                options:
                    remote: 'git@github.com:2dotstwice/aft-slides-skeleton.git'
                    branch: 'gh-pages'
* Change the introduction slide in `slides/index.md`.
* Remove / edit `slides/example.md`.
                    
## Adding new slides

* Add new slides by running `yo reveal:slide "Slide title" --markdown`.
* OR create a new `.md` file in `slides` and add it to `slides/list.json`.

## Re-ordering, deleting, ... slides

Slide order is defined in `slides/list.json`.


## Running locally

1. Run `grunt serve`.
2. There is no step 2.

## Deploying to Github Pages

0. **Make sure you have followed the steps in "Setup".**
1. Run `grunt deploy`.
2. Your presentation will be available at [http://username.github.io/repo-name](http://username.github.io/repo-name), for example: [http://2dotstwice.github.io/aft-slides-skeleton](http://2dotstwice.github.io/aft-slides-skeleton).