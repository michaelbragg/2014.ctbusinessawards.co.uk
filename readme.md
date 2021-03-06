# Coventry Telegraph Business Awards 2014
[http://ctbusinessawards.co.uk/2014/](http://www.ctbusinessawards.co.uk/2014/)

## Description



## Dependencies

- NodeJS
  - Grunt
  - LESS CSS
- Ruby
  - Jekyll
  - RDiscount

## Instructions

### Setup Development Area

```
npm install
gem install jekyll
```

### Run Development Server

```
grunt
```

Visit the url [localhost:3000](http://localhost:3000/) to view the site.

### Deploy Build

#### Staging

For testing and proofing we deploy to a staging server before deploying to production.

```
grunt stage
```

This push the changes to the `gh-pages` branch and allows us to view the site via [http://beta.ctbusinessawards.co.uk/](http://beta.ctbusinessawards.co.uk/).

#### Production

To build the site for deployment:

```
grunt deploy
```

This will produce a `./2014` folder that can be uploaded to the server.

## Documentation

During the Alpha/Beta stages, due to constant changes, documentation will be mainly written in-line. With a dedicated section being created at the first major release.

### Adding a new News Post

To write a new news post create a new markdown document in the `src/_posts` folder. Add the following YAML to the top of the page filling in details for title, date and images:

```
---
layout: news

title:
categories: news
date:
published: true

images:
 main:
 preview:
---
```

### File Structure

```
|- _scripts              –  contains useful scripts to help with
|                           development of this project
|- _site                 –  compiled development files (not committed)
|- src
|  |- _includes          –  partial snippets of code to be used
|  |                        in layouts
|  |- _layouts           –  page layouts
|  |- _posts             -  markdown files of news posts
|  |- media              -
|  |- static             -
|  |- {**/*.txt,html,md} -  files for website
|- _config.yml           -  Jekyll config file
|- gruntfile.js
|- package.json
|- readme.md
```

## Report Issues

If you spot any issues please create a ticket via GitHub's Issue Tracker. If the issue is security related please use the contact information below.

## Contribute

In lieu of a formal style guide, take care to maintain the existing coding style.

## Contact

## License

The source is opened for educational purposes. No rights are assigned to any downloads or forks.

## Copyright

Unless otherwise stated &copy; Trinity Mirror Creative. All rights reserved.
