source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'rails',                '~> 5.1.4'
gem 'sqlite3'
gem 'puma',                 '~> 3.7'
gem 'sass-rails',           '~> 5.0'
gem 'uglifier',             '>= 1.3.0'
gem 'coffee-rails',         '~> 4.2'
gem 'turbolinks',           '~> 5'
gem 'font-awesome-rails',   '~> 4.7', '>= 4.7.0.1'
gem 'bootstrap-sass',       '~> 3.3', '>= 3.3.7'

gem "camaleon_cms",         '>= 2.4.4.5'
gem 'draper',               '~> 3'
gem 'haml-rails',           '~> 1.0'

group :development, :test do
  gem 'pry-rails', '~> 0.3.6'
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'capybara', '~> 2.13'
  gem 'selenium-webdriver'
end

group :development do
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '>= 3.0.5', '< 3.2'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]


#################### Camaleon CMS include all gems for plugins and themes #################### 
require './lib/plugin_routes' 
instance_eval(PluginRoutes.draw_gems)