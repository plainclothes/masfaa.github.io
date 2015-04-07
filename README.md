# MASFAA

## Purpose

TODO

## Hosting and DNS

TODO

## History

TODO

Initial Github Pages site cloned from [`safmt/ghpages`](https://github.com/safmt/ghpages).

# How to Work Locally

Make sure that you have installed:
* git
* VirtualBox
* Vagrant

Clone the repo:
```
> git clone https://github.com/masfaa/masfaa.github.io
```

Start up a virtual machine that is ready for Jekyll:
```
> cd masfaa.github.io
> vagrant up
> vagrant ssh
> cd jekyll
```

[Install Jekyll](https://help.github.com/articles/using-jekyll-with-pages/) (first time only):
```
> bundle install
```

Start Jekyll server:
```
> bundle exec jekyll serve --host 0.0.0.0 --force_polling
```

Edit in the host OS. Find the website at http://192.168.33.10:4000/

Commit changes and push to the master branch to deploy to production.
