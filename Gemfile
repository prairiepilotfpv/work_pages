source 'https://rubygems.org'

# Core Jekyll
gem 'jekyll', '~> 4.4'
gem 'jekyll-sass-converter', '~> 3.0' # uses Dart Sass via sass-embedded
gem 'sass-embedded', '~> 1.75'

# Jekyll plugins
group :jekyll_plugins do
  gem 'jekyll-feed', '~> 0.17'
  gem 'jekyll-remote-theme'
  gem 'jekyll-scholar'
  gem 'jekyll-toc'
end

# Ruby 3.x compatibility
gem 'bigdecimal'        # required by liquid on Ruby 3.4+
gem 'logger'            # silences Ruby 3.5 logger warning
gem 'webrick', '~> 1.8' # local server on Ruby 3.x

# Platform-specific dependencies
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem 'tzinfo', '>= 1', '< 3'
  gem 'tzinfo-data'
end

gem 'wdm', '~> 0.1', platforms: [:mingw, :x64_mingw, :mswin]

platforms :jruby do
  # Lock http_parser.rb to v0.6.x on JRuby (no newer Java counterpart)
  gem 'http_parser.rb', '~> 0.6.0'
end

# GitHub Pages:
# If building with GitHub Pages, comment out the 'jekyll' gem above
# and use the following instead to match the Pages environment:
# gem 'github-pages', group: :jekyll_plugins
# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
