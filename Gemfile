source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '3.0.1'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 6.1.3.0'

gem 'dotenv-rails', groups: [:development], require: 'dotenv/rails-now', github: 'jenfi-eng/dotenv'

# Use postgresql as the database for Active Record
gem 'pg', '>= 0.18', '< 2.0'
gem 'strong_migrations'

# Use Puma as the app server
gem 'puma', '~> 4.1'
gem 'webrick' # Removed from stdlib in Ruby 3
# Use SCSS for stylesheets
gem 'sass-rails', '~> 6.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'

# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
gem 'hiredis', '~> 0.6.0'
gem 'redis', '~> 4.0', require: %w[redis redis/connection/hiredis]

# Use ActiveStorage variant
gem 'mini_magick', '~> 4.8'
gem 'image_processing'

# Frontend
gem 'browser'
gem 'caxlsx_rails'
gem 'draper', github: 'drapergem/draper', branch: 'master', ref: '9cb42f6e714764c1b196f49754328132bcc7ed32'
gem 'http_accept_language'
gem 'intercom'
gem 'meta-tags'
gem 'slim-rails'
gem 'webpacker'
gem 'rack-attack'
gem 'i18n-js'
gem 'inline_svg'

# Tracking
gem 'analytics-ruby'
gem 'ahoy_matey'

# Background
gem 'httparty'
gem 'rest-client' # Because Justin sucks
gem 'ruby-vips', require: false
gem 'rubyzip'
gem 'sidekiq'
gem 'sidekiq-status'
gem 'wisper'
gem 'wisper-sidekiq'

# User
gem 'devise'
gem 'invitation'
gem 'pundit'
gem 'omniauth-google-oauth2'
gem 'omniauth-facebook'

# Crypto/Auth
gem 'jwt'
gem 'jwe'
gem 'gpgme'

# Admin
gem 'activeadmin'
gem 'active_admin_datetimepicker', github: 'jenfi-eng/active_admin_datetimepicker'
gem 'paper_trail'
gem 'bitfields'
gem 'ckeditor', github: 'galetahub/ckeditor'

# PDF Handling
gem 'combine_pdf'
gem 'liquid'
gem 'wicked_pdf'
gem 'wkhtmltopdf-binary'
gem 'pdf-reader'

# Better URLs
gem 'friendly_id'

# CMS
gem 'comfortable_mexican_sofa', github: 'jenfi-eng/comfortable-mexican-sofa'
gem 'comfy_blog', '~> 2.0.0'

# Monitoring
gem 'rollbar'
gem 'newrelic_rpm', group: %i[staging production]

# Reduces boot times through caching; required in config/boot.rb
gem 'bootsnap', '>= 1.4.0', require: false

# External Services
gem 'aws-sdk-s3', require: false

# Type system for Ruby post deploy
gem 'sorbet-runtime'
gem 'sorbet-rails'

# Email
gem 'sendgrid-ruby'

# Phone
gem 'phonelib'
gem 'twilio-ruby', require: false

gem 'money-rails'
gem 'money-open-exchange-rates'
gem 'xirr', github: 'tubedude/xirr', ref: '2b18ab0fe58d888ed55100decc582fb45dade80b'

# State Machine
gem 'aasm'

# Transaction Handling
gem 'acts_as_list'

# Geocoding
gem 'maxminddb'
gem 'countries'

# External Underwriting Connections
gem 'facebookbusiness'
gem 'braintree'

##### Scrapers use this #######################################################
# JL: I didn't feel like a whole separate environment was
# worth the effort of keeping these 3 in their own group

# Adds support for Capybara system testing and selenium driver
gem 'capybara', '>= 2.15', require: false

gem 'selenium-webdriver', require: false
# Easy installation and use of chromedriver to run system tests with Chrome
gem 'webdrivers', '~> 4.0', require: false
gem 'google-ads-googleads', '~> 7.0'
##### /Scrapers ###############################################################

## translation gems
gem 'google-cloud-translate'

## import bulk
gem 'activerecord-import'

group :development, :test do
  gem 'pry'
  gem 'pry-rails'
  gem 'pry-byebug'

  gem 'guard', '~>2.14.2', require: false
  gem 'guard-livereload','~>2.5.2', require: false
  gem 'guard-rspec', '~>4.7', require: false

  gem 'factory_bot_rails'
  gem 'timecop'
  gem 'faker'

  gem 'rack-livereload'

  # Typing system for Ruby
  gem 'sorbet'

  gem 'rubocop-rails', require: false
  gem 'rubocop-daemon', require: false

  gem 'i18n-tasks', require: false

  gem 'awesome_print', github: 'awesome-print/awesome_print', branch: 'awesomeprint2'
  gem 'lintman', git: 'https://github.com/Anadea/lintman.git', require: false
  gem 'scss_lint', require: false
  gem 'rails-controller-testing'
end

group :development do
  # Access an interactive console on exception pages or by calling 'console' anywhere in the code.
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '>= 3.0.5', '< 3.2'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  # gem 'spring'
  # gem 'spring-watcher-listen', '~> 2.0.0'

  gem 'rails-erd'

  gem 'solargraph'

  # Only here to make Sorbet happy w/ ActiveAdmin.
  gem 'cancan'
end

group :test do
  gem 'rspec'
  gem 'rspec-rails'
  gem 'rspec_junit_formatter'

  gem 'vcr'

  gem 'webmock'
  gem 'wisper-rspec', require: false

  gem 'codecov', require: false

  gem 'hashdiff'
end

group :build do
  gem 'activerecord-nulldb-adapter'
end
