# SHU RMRC Seminar website
This repo runs the website for the Sheffield Hallam University Recreational
Mathematics Research Cluster website.

## Building the website
The prerequisites for building the website can be installed by running:

```bash
sudo apt-get install -y ruby-bundler
bundle install
```

The website can then be built by running:

```bash
bundle exec jekyll build
```

The website can be served locally (so it can then be opened in a browser) by running:

```bash
bundle exec jekyll serve
```
