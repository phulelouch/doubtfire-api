source 'https://rubygems.org'

# Ruby versions for various enviornments
ruby_versions = {
  development: '~>3.1.0',
  test: '~>3.1.0',
  staging: '~>3.1.0',
  production: '~>3.1.0'
}
# Get the ruby version for the current enviornment
ruby ruby_versions[(ENV['RAILS_ENV'] || 'development').to_sym]

# The venerable, almighty Rails
gem 'rails', '~> 7.0.7', '>= 7.0.7.1'

group :development, :test do
  gem 'better_errors'
  gem 'byebug'
  gem 'database_cleaner', '>= 2.0.2'
  gem 'listen'
  gem 'rails_best_practices', '>= 1.23.2'
  gem 'rubocop'
  gem 'rubocop-faker'
  gem 'rubocop-rails', '>= 2.16.0'
  gem 'simplecov', require: false
  gem "sprockets-rails"
end

group :development, :test, :staging do
  # Generators for population
  gem 'factory_bot'
  gem 'factory_bot_rails'
  gem 'faker'
  gem 'minitest'
  gem 'minitest-around'
  gem 'webmock'
end

# Database
gem 'mysql2'

# Webserver - included in development and test and optionally in production
gem 'puma', '~> 5.6'

gem 'bootsnap', '>= 1.4.4', require: false

# Extend irb for better output
gem 'hirb'

# Authentication
gem 'devise', '>= 4.9.0'
gem 'devise_ldap_authenticatable'
gem 'json-jwt', '>= 1.15.0'
gem 'ruby-saml', '~> 1.13.0'

# Student submission
gem 'coderay'
gem 'rmagick', '~> 4.1' # require: false #already included in other gems - remove to avoid duplicate errors
gem 'ruby-filemagic'
gem 'rubyzip'

# Plagarism detection
gem 'moss_ruby', '>= 1.1.4'

# Latex
gem 'rails-latex', '>2.3'

# API
gem 'grape', '>= 1.7.0'
gem 'grape-entity', '>= 0.10.2'
gem 'grape-swagger', '>= 1.5.0'
gem 'grape-swagger-rails', '>= 0.4.0'

# Miscellaneous
gem 'bunny-pub-sub', '0.5.2'
gem 'ci_reporter'
gem 'dotenv-rails', '>= 2.8.0'
gem 'rack-cors', require: 'rack/cors'
gem 'require_all', '>=1.3.3'

# Excel support
gem 'roo', '~> 2.7.0'
gem 'roo-xls'

# webcal generation
gem 'icalendar', '~> 2.5', '>= 2.5.3'

gem 'rest-client', '~> 2.0'

gem 'net-smtp', require: false
