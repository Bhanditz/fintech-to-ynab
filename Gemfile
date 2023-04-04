ruby '2.5.1'

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

gem 'rails', '~> 6.1.7', '>= 6.1.7.3'
gem 'puma', '~> 4.3', '>= 4.3.12'

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
  gem 'dotenv-rails', '>= 2.7.6'
  gem 'rubocop-rails_config'
end

group :test do
  gem 'rspec-rails'
  gem 'codecov', '>= 0.1.21'
end

gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
