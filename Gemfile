source "http://rubygems.org"

# Specify your gem's dependencies in guard-annotate.gemspec
gemspec development_group: :gem_build_tools

group :gem_build_tools do
  gem 'rake'
end

group :development do
  gem 'guard-rspec', require: false
end

group :test do
  gem  'rspec', '~> 3.1'
end

require './spec/support/platform_helper'

if mac?
  gem 'rb-fsevent', '>= 0.3.2'
  gem 'growl',      '~> 1.0.3'
elsif linux?
  gem 'rb-inotify', '>= 0.5.1'
  gem 'libnotify',  '~> 0.1.3'
end
