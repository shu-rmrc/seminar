# SHU RMRC Seminar website
This repo runs the website for the Sheffield Hallam University Recreational
Mathematics Research Cluster website.

## Editing the website
To add a new upcoming talk, to the website, edit `upcoming.md`. Talks should have the format:

```
{% include _talk.html
    img="assets/img/filename.extension"
    img_alt="Description of image"
    speaker="Dr S. Peaker"
    institute="Fictional University, UK"
    title="The maths of baseball"
    date="Thursday 1st April 2027"
    time="4.00-4.45pm GMT" [optional]
    description="Description of the talk"
    website="https://speakers-website.com" [optional]
    twitter="speakers_twitter_handle" [optional]
    github="speakers_github_username" [optional]
%}
```

Past seminars can be added in the same way by editing `past.md`.

## Building the website
If you want to build the website locally, the prerequisites for building the website can be installed by running:

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

When changes are pushed to GitHub, the website will built automatically.
