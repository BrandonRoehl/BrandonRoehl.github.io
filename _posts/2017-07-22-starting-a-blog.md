# Starting a blog
I am now starting a blog on my website using `Jekyll`

This is hosted on [GitHub Pages](https://pages.github.com)

Here are the steps that it took for me to get this working

[** Gemfile **](https://github.com/BrandonRoehl/BrandonRoehl.GitHub.io/blob/master/Gemfile)
```ruby
source 'https://rubygems.org'
gem 'github-pages'
```
[** bower.json **](https://github.com/BrandonRoehl/BrandonRoehl.GitHub.io/blob/master/bower.json)
```json
{
  "name": "polymer-project",
  "authors": [
    "Brandon Roehl"
  ],
  "private": true,
  "dependencies": {
    "app-layout": "PolymerElements/app-layout#^0.10.0",
    "app-route": "PolymerElements/app-route#^0.9.0",
    "iron-flex-layout": "PolymerElements/iron-flex-layout#^1.0.0",
    "iron-icon": "PolymerElements/iron-icon#^1.0.0",
    "iron-icons": "PolymerElements/iron-icons#^1.0.0",
    "iron-iconset": "PolymerElements/iron-iconset#^1.0.0",
    "iron-iconset-svg": "PolymerElements/iron-iconset-svg#^1.0.0",
    "iron-media-query": "PolymerElements/iron-media-query#^1.0.0",
    "iron-pages": "PolymerElements/iron-pages#^1.0.0",
    "iron-selector": "PolymerElements/iron-selector#^1.0.0",
    "paper-elements": "PolymerElements/paper-elements#^1.0.7"
  }
}
```

Then just running
```bash
gem install bundler
bundler install
bower install
jekyll s
```

Then I built out the page with polymer using `<app-route>` and `<app-location>` for the normal routing

For the posts in jekyll you can then loop though with
```html
{% for post in posts %}
use information from post here
{% endfor %}
```
