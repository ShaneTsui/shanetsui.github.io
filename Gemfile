# frozen_string_literal: true

source "https://rubygems.org"

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
  
gemspec

# Use Jekyll 3.x to avoid sass-embedded/protobuf; use Ruby Sass (no native deps)
gem "jekyll", "~> 3.9.3"
gem "jekyll-sass-converter", "~> 1.5.2"
gem "sass", "~> 3.7.4"

# Livereload plugin for Jekyll 3.x
group :jekyll_plugins do
  gem "jekyll-livereload", "~> 0.2.2"
end

