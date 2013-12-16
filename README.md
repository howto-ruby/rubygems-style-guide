# The RubyGems Development Style Guide

So, you're writing a RubyGem. Wouldn't it be great if there were a place
you could reference which contains all the shared wisdom and experience
of gem authors and maintainers?  Well, here you are.

# What is this?

A set of community-driven set of best practices, conventions, and gotchas
for gem authors and maintainers. It is meant to augment and supplement the
[RubyGems Guides](http://guides.rubygems.org/), and perhaps serve as a
sounding-board for ideas before they go into the Guide.

Inspired by [Bozhidar's Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide)

Translations of the guide are available in the following languages:

## Table of Contents

* [Source Code Layout](#source-code-layout)
* [Naming](#naming)
* [Gemspec](#gemspec)
  * [Platform](#platform)
* [Documentation](#documentation)
* [Tests](#tests)
* [Configuration](#configuratino)
* [Dependency Management](#dependency-management)
* [Exceptions](#exceptions)
* [Extensions, Plugins, Hooks](#extensions)
  * [RubyGems extensions](#rubygems-extensions)
* [Handling Input and Output](#handling-io)
* [Maintenance](#maintenance)
* [Misc](#misc)
* [Tools](#tools)

## Source Code Layout

- top-level directories:
  - app
  - bin
  - cert
  - checksum
  - config
  - doc
  - ext
  - features
  - lib
  - spec
  - tasks
  - templates
  - test
  - tmp
  - vendor
- what goes in lib?
- what directories are under lib?
- top-level files:
  - README.md
  - CHANGELOG.md
  - DEVELOPERS.md
  - TODO.md
  - LICENSE
  - AUTHORS
  - gemspec
  - Gemfile
  - dotfile opts

## Naming

- foo-bar -> foo/bar
- foo_bar -> foo_bar

## Gemspec

- files to specify
- specifying included files
- post_install
- security

### Platform

- releasing for multiple platforms
- [Redcard](https://github.com/brixen/redcard), to determine ruby engine
  and version, e.g. in [metric_fu](https://github.com/metricfu/metric_fu/blob/94bd872/lib/metric_fu/environment.rb#L34w
- File::Separator or File.join('foo','bar')

## Documentation

- What it is
- Basic Usage
- Examples of more usage
- How to develop
- Communication: bugs, questions, code
- Version control policies

## Tests

- How to run

## Configuration

- Specifying an interface for users to configure your gem
  - as a library
  - as a command-line tool

## Dependency Management

- Runtime dependencies
  - hard, at install
  - soft, e.g. platform issues
- Development dependencies
  - required to run tests vs. used in development


## Exceptions

- What exceptions can the lib raise?
- How are they handled within the lib?

## Extensions

- how to extend or change functionality
- how it loads plugins, how to configure
- hooks

### RubyGems Extensions

- rubygems_plugin

## Handling IO

- logging
- stdout, stdin, stderr
- warnings

## Maintenance

- security
- deprecations
- semver
- issue tracking
- communication
- abandoning

## Misc

- benchmarking
- internal gems
- gem serving
- app vs. lib
- [Twelve-factor App](http://12factor.net/)

## Tools

- git
- bundler
- gli
- irc
- mailing lists
  - rubygems-developers
- rake
- homebrew

## External Resources

- http://confreaks.com/videos/2888-rubyconf2013-api-design-for-gem-authors-and-users
- http://confreaks.com/videos/2884-rubyconf2013-extending-gems-patterns-and-anti-patterns-of-making-your-gem-pluggable
- http://www.naildrivin5.com/blog/2013/12/02/introduction-to-gli.html
- http://guides.rubygems.org/


# Contributing

- Fork this repo, checkout a branch, commit changes, submit a pull request
- Tweet `@hazula`

# License

![Creative Commons License](http://i.creativecommons.org/l/by/3.0/88x31.png)
This work is licensed under a [Creative Commons Attribution 3.0 Unported License](http://creativecommons.org/licenses/by/3.0/deed.en_US)

# Spread the Word

- This is very alpha. Any help or thoughts are appreciated.
