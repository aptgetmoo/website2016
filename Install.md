# Installing

## Linux

*Note: this guide is written with Debian-derived distros in mind -- I'd love it if someone could contribute instructions for other (non `apt`) distros!

### With Docker

If you use Docker, installing is pretty painless:

*  Grab a copy of `docker-ce` by following the [instructions for your distribution](https://docs.docker.com/engine/installation/linux/).
*  The only other dependency is `git`, or `unzip` to get a copy of the source.
*  Run `preview.sh`.

### Without Docker

**Prerequisite software**

*  [Ruby and the gem package manager](https://www.ruby-lang.org/en/documentation/installation/), available under Debian and Ubuntu as `ruby-full`.
*  [Bundler](http://bundler.io/), installed via `gem install bundler`.
*  `build-essential` is required to build certain gems.
*  `zlib1g-dev` is also required to build the nokogiri gem.
*  `git`, or `unzip` will be required to get the source.

1. `sudo apt install ruby-full build-essential zlib1g-dev git`
2. `sudo gem install bundler`


**Install instructions**

*  `git clone https://github.com/compsoc-edinburgh/website2016.git`
*  `cd website2016`
*  `bundle install --path vendor/bundle`


**Run**

*  `bundle exec jekyll serve`



