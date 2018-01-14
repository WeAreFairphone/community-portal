# WeAreFairphone community landing page

A [Jekyll](http://jekyllrb.com/)-based static site used to inform the public of
[WeAreFairphone community](https://www.fairphone.com/en/community/) activities.

Features are discussed [on the Fairphone forum thread](https://forum.fairphone.com/t/online-portal-for-fairphone-community/28956/).

## Installation

First, make sure, you have
[Ruby](https://www.ruby-lang.org/en/documentation/installation/)\* and
[bundler](https://bundler.io/) installed.

Then run `bundle install` and you are ready to start.

\* *Ruby 2.5 is not currently supported.*

## Usage

### Blog articles

For blog posts, create Markdown files in [_posts](./_posts).
You can write drafts in [_drafts](./_drafts), which won't get published.

### Pages

For pages, just create [Markdown files in the root directory](https://jekyllrb.com/docs/pages/).

### Linking forum articles

Every page has the option to name one further reading forum post.
Therefore it needs a `further_reading` in its Preface.
The corresponding value can be found in `jekyll_get` section of
[_config.yml](./_config.yml).
This in turn will download the forum post (in JSON format) and store it
[_data](./_data) under the key given in `further_reading`.

## Development

Run `bundle exec jekyll serve` to start a development server and visit
[localhost:4000](http://localhost:4000/).  

Note: If you try running this on a Windows machine you might encounter problems with the character encoding. To solve this, simply execute `chcp 65001` in your current PowerShell window.

### Tweaking templates

Since we use [minima](https://github.com/jekyll/minima) (as can be seen in
[_config.yml](./config.yml) key `theme`), we can download files from that
theme, drop them in the same place and start modifying them.

The idea could be to publish an own theme, once there is a stable version.
This would likely move into its own repo and added as dependency here.

## License

GPL 3.0. See [license](./LICENSE).
