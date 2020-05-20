ruby '2.5.1'

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'rails', '~> 5.2.4', '>= 5.2.4.3'
gem 'puma', '~> 3.7'

gem 'f2ynab', github: 'fintech-to-ynab/f2ynab'
# gem 'f2ynab', path: '../f2ynab'

# Utilities
gem 'awesome_print'
gem 'commander'

group :production do
  gem 'rails_12factor'
end

group :development, :test do
  gem 'listen'
  gem 'dotenv-rails', '>= 2.6.0'
  gem 'rubocop-rails_config', '>= 0.2.6'
end

group :test do
  gem 'rspec-rails', '>= 3.8.1'
  gem 'codecov'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
