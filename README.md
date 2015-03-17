# SAF Websites

For each website at SAF, create a new Github organization named for the site, i.e. 'masfaa' for MASFAA. By making each site its own organization we can control access to a site's repo if necessary. Once an organization is created, use Github to fork this repo (safmt/ghpages) into the organization and rename it to work with Github Pages, i.e. 'masfaa.github.io'. To do this:

1. Click 'Fork'.
2. Choose the new organization.
3. In Settings, rename the repo to the name of the organization plus '.github.io'.
4. Edit the README.md to remove this top section and update the organization name in the how to below.

# How to Work Locally

Make sure that you have installed:
* git
* VirtualBox
* Vagrant

Clone the repo:
```
> git clone https://github.com/[organization]/[organization].github.io
```

Start up a virtual machine that is ready for Jekyll:
```
> cd [organization].github.io
> vagrant up
> vagrant ssh
> cd jekyll
```

Install Jekyll (first time only):
```
> bundle install
```

Start Jekyll server:
```
> bundle exec jekyll serve --host 0.0.0.0 --force_polling
```

Edit in the host OS. Find the website at http://192.168.33.10:4000/

Commit changes and push to the master branch to deploy to production.
