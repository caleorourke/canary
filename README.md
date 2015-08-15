<a href="http://travis-ci.org/caleorourke/graysuit?branch=gh-pages" target="_blank"><img src="http://travis-ci.org/caleorourke/graysuit.svg?branch=gh-pages" alt="Build Status"></a>
<a href="https://david-dm.org/caleorourke/graysuit#info=devDependencies" target="_blank"><img src="https://david-dm.org/caleorourke/graysuit/dev-status.svg?theme=shields.io"></a>
<a href="http://github.com/caleorourke/graysuit/blob/gh-pages/LICENSE" target="_blank"><img src="http://img.shields.io/badge/License-MIT-blue.svg" alt="MIT-license badge"></a>

## Graysuit

Graysuit is a blueprint for defining monitoring data artifacts in a visual manner.

* [Prerequisites](#prerequisites)
* [Quick Install](#quick-install)
* [Local Deployment](#local-deployment)
* [Roll Your Own](#roll-your-own)
* [Code Organization](#code-organization)

## Prerequisites

Graysuit is hosted on GitHub using [GitHub Pages](http://pages.github.com). It can be served locally using [Jekyll](http://jekyllrb.com) with __Ruby 2.0.0__ or greater. [Click here](http://www.ruby-lang.org/en/installation) to download and install Ruby. If you have Ruby, but aren’t sure which version, run `ruby -v`.

## Quick Install

Clone from GitHub and go into the directory.

        $ git clone -b gh-pages https://github.com/caleorourke/graysuit.git
        $ cd graysuit

Install Grunt's CLI.

        $ [sudo] npm install -g grunt-cli

Install Node packages.

        $ [sudo] npm install

Install GitHub Pages and runtime dependencies.

        $ [sudo] grunt install

## Local Deployment

Run the command below to preview a local instance of your site.

```bash
$ grunt serve
```

After Jekyll starts, fire up a browser and type in `localhost:4000` for the web address. This will pull up the site Jekyll just generated.

### Killing Jekyll

Serve mode lasts forever. It won't timeout after a period of non-usage. Press `CTRL+C` to stop the service.

## Roll Your Own

Make a fresh clone and go into the directory.

        $ git clone https://github.com/username/grayhat.git
        $ cd grayhat

Create a new `gh-pages` branch.

        $ git checkout --orphan gh-pages

Copy the contents from `/graysuit` to `/grayhat`.

        $ cp -r ~/graysuit/* ~/grayhat

4. Push your site to GitHub.

        $ git add .
        $ git commit -a -m "first commit"
        $ git push origin gh-pages

## Code Organization

Below is the basic spread for Graysuit (not including Jekyll or GitHub-related objects).

<pre>
├─ _includes/
│   ├─ charts/
│   ├─ forms/
│   ├─ logs/
│   └─ modals/
│       ├─ processes/
│       └─ server/
├─ _layout/
├─ js/
├─ less/
├─ public/
│   ├─ css/
│   ├─ fonts/
│   ├─ img/
│   ├─ js/
│   └─ logs/
├─ alerts.html
├─ config.html
├─ index.html
├─ logs.html
├─ processes.html
├─ profile.html
├─ settings.html
├─ support.html
└─ usage.html
</pre>

## License

Code and documentation is licensed under the MIT license.
