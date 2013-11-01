## Installing Dependencies

    gem update --system
    gem install jekyll
    gem install bundler
    bundle install

#### Windows Compatibility

Use Ruby 1.9.3 and Pygments.rb 0.5.0

After installing dependencies, run:

    gem uninstall pygments.rb
    gem install pygments.rb  -v 0.5.0

And in `Gemfile.lock` edit as follows:

    pygments.rb (0.5.0)

## Local Development

1. Run Jekyll

        bundle exec jekyll serve --watch

1. Visit [http://localhost:4000](http://localhost:4000)

## PubSubHubbub Publishing

When publishing a new article, ping the PubSubHubbub hub to push-notify all feed subscribers. Jekyll on GitHub Pages does not support this so use the bookmarklet to manually ping the hub.

[Bookmarklet](http://pubsubhubbub.appspot.com/bookmarklet_config.html)
