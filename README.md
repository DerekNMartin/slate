Getting started with Slate is super easy! Simply fork this repository and follow the instructions below. Or, if you'd like to check out what Slate is capable of, take a look at the [sample docs](http://lord.github.io/slate).

Getting Started with Slate
------------------------------

### Prerequisites

You're going to need:

 - **Linux or OS X** — Windows may work, but is unsupported.
 - **Ruby, version 2.3.1 or newer** `sudo apt-get install ruby-full`
 - **Bundler** — If Ruby is already installed, but the `bundle` command doesn't work, just run `gem install bundler` in a terminal.

### Getting Set Up

1. Fork this repository on GitHub.
2. Clone *your forked repository* to your hard drive with `git clone https://github.com/YOURUSERNAME/slate.git`
3. `cd slate`
4. Initialize and start Slate. You can either do this locally, or with Vagrant:

```shell
# either run this to run locally
bundle install
bundle exec middleman server

# OR run this to run with vagrant
vagrant up
```

You can now see the docs at http://localhost:4567. Whoa! That was fast!

### Converting swagger.json to markdown

We'll use a [swagger-to-slate](https://github.com/lavkumarv/swagger-to-slate) to convert the swagger specification file (JSON or YAML) into slate markdown.

## Prerequisites

You'll need to have node and npm install.

## Installing

Install using `npm install -g swagger-to-slate`

## Converting the file

```shell
swagger-to-slate -i /home/user/Somewhere/swagger.json
```

```shell
swagger-to-slate -i /home/user/Somewhere/swagger.yaml
```

This will generate the output file in the same path with the same file name. (ex. swagger.md)

### Add to Slate

Once you've converted your `swagger.json` file to markdown, copy it into `/slate/source/index.html.md`

Refresh `http://localhost:4567` and see your docs in Slate!