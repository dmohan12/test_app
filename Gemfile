source "https://rubygems.org"

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

ruby "2.6.6"

gem 'rails', '6.0.3.1'
gem "autoprefixer-rails"
gem 'faker',          '2.11.0'
gem 'pg', '1.2.3'
gem "bootsnap", require: false
gem "honeybadger", "~> 4.0"
gem "puma"
gem 'will_paginate',           '3.3.0'
gem "rack-canonical-host"
gem "recipient_interceptor"
gem 'bootstrap-will_paginate', '1.0.0'
gem 'bootstrap-sass', '3.4.1'
gem 'sass-rails', '6.0.0'
gem "skylight"
gem 'turbolinks', '5.2.1'
gem "sprockets", "< 4"
gem "title"
gem "tzinfo-data", platforms: [:mingw, :x64_mingw, :mswin, :jruby]
gem "webpacker"

group :development do
  gem "listen"
  gem "web-console"
  gem 'spring',                '2.1.0'
  gem 'spring-watcher-listen', '2.0.1'
  gem 'solargraph'

end

group :development, :test do
  gem "awesome_print"
  gem "pry-rails"
  gem 'rspec-rails', '~> 4.0.1'
  gem "factory_bot_rails"
  gem 'byebug',  '11.1.3', platforms: [:mri, :mingw, :x64_mingw]

end

group :test do
  gem 'capybara',                 '3.32.2'
  gem 'selenium-webdriver',       '3.142.7'
  gem 'cucumber-rails', require: false
  # database_cleaner is not required, but highly recommended
  gem 'database_cleaner'
  gem 'webdrivers',               '4.3.0'
end
group :production do
  gem 'aws-sdk-s3', '1.46.0', require: false
end

gem "suspenders", group: [:development, :test]
