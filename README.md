# leopardrobotics.github.io #

This is the website source code for Leopard Robotics, a FIRST Tech Challenge
club organized at Lake Middle School in Woodbury, MN. It is built
with [Jekyll][jekyll] and hosted on [GitHub Pages][ghpages].

Jekyll is a Ruby toolkit for converting plain text documents into static
websites. This greatly simplifies the installation of the site, but it also
allows development of the site locally. The instructions in this document
include the basic setup on a Linux or Macintosh. For Windows development,
consider running an Ubuntu virtual machine.

## Contributing ##

To contribute articles or bug fixes to the website, begin by creating
an [issue ticket][issue]. If you have a solution or want to contribute code
directly, fork the project, commit the fix to a branch of your fork, and then
submit a merge request to the main project.

### Development Environment ##

To get started, it is recommended that Ruby 2.3.1 or greater is used. Although
some distributions of Linux follow the latest ruby development, it is suggested
that a toolkit like [rbenv][rbenv] or `rvm` is used to download and manage
multiple versions of ruby. `rbenv` is the simplest to set up and use, and the
one suggested here. Follow the link above for instructions on installing `rbenv`.

It is also suggested that [ruby-build][ruby-build] be installed as a plugin to
`rbenv` to enable you to simply run:

    rbenv install 2.5.1

Now that Ruby is installed, install the `bundler` gem:

    rbenv use 2.5.1
    gem install bundler

[Bundler][bundler] is a gem that helps manage gems, or libraries of functions
and resources that are included in this project. These are listed in the
`Gemfile` as simple dependency lists. The following command,

    bundler install

will ensure that all of the libraries necessary are installed relative to this
project. It will allow one to compile the source content into a static website,
and even to run it locally to see changes before they're submitted for a Merge
Request.

To test the site, run the following command:

    jekyll serve

Now, open a web browser to http://localhost:4000/ to view the site. Refer to
the [Jekyll][jekyll] website for more information about using the toolkit and
building static sites.

[jekyll]: http://jekyllrb.com/
[ghpages]: https://pages.github.com/
[rbenv]: https://github.com/rbenv/rbenv
[ruby-build]: https://github.com/rbenv/ruby-build#readme
[bundler]: http://bundler.io/
[issue]: https://github.com/leopardrobotics/leopardrobotics.github.io/issues
