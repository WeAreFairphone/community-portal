# WeAreFairphone community landing page

A [Jekyll](http://jekyllrb.com/)-based static site for informing about
[WeAreFairphone community](https://www.fairphone.com/en/community/) activities.

Features are discussed [on the Fairphone forum thread](https://forum.fairphone.com/t/online-portal-for-fairphone-community/28956/).

## Installation

First, make sure, you have
[Ruby](https://www.ruby-lang.org/en/documentation/installation/) and
[bundler](https://bundler.io/) installed.

Then run `bundle install` and you are ready to start.

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

## TODO

* [ ] Think about recommending [rvm](https://rvm.io/) in installation instructions.
* [ ] Explore [discourse_api](https://github.com/discourse/discourse_api). (See [forum post](https://meta.discourse.org/t/discourse-plugin-for-static-site-generators-like-jekyll-or-octopress/7965))
* [ ] Think about [publishing on GitHub Pages](https://help.github.com/articles/about-supported-custom-domains/).
      According to docs there is [a whitelist of plugins](https://help.github.com/articles/configuring-jekyll-plugins/#default-plugins) which could make this approach hard.
* [ ] Pull data for [community events](https://www.fairphone.com/en/community/events/?event-category=community-event) from the page.
* [ ] Embed [communitymap](https://forum.fairphone.com/tags/communitymap)
* [ ] Align with [duke1102/FairphoneAngel-LandingPage](https://github.com/duke1102/FairphoneAngel-LandingPage) about design.
* [ ] Get inspiration from [mozilla/activate.mozilla.community](https://github.com/mozilla/activate.mozilla.community) or [learning.mozilla.org](https://learning.mozilla.org/).

## License

GPL 3.0. See [license](./LICENSE).
