source 'http://rubygems.org'

ruby "2.0.0"

gem 'rails', '4.0.1'
gem 'sass-rails', '~> 4.0.1'
gem 'uglifier', '>= 1.3.0'
gem 'jquery-rails'
gem 'ejs'
gem "compass-rails", "~> 1.1.2"
gem "devise", "~> 3.2.0"
gem 'transitions', '0.1.9', :require => ["transitions", "active_record/transitions"]
gem 'rails-i18n'
gem 'configuration'
gem 'rails-observers', '~> 0.1.2'
gem 'jquery-ui-rails'
gem 'newrelic_rpm'

group :production do
  gem 'pg'
  gem 'unicorn'
  gem 'rails_12factor'

end

group :development, :test do
  gem 'sqlite3'
  gem 'rspec-rails'
  gem 'factory_girl_rails'
  gem 'jasmine', '~> 1.3.2'
  gem 'capybara'
  gem 'capybara-webkit'
  gem 'database_cleaner'
end

group :travis do
  # gem 'mysql2'
end

if ENV['TRAVIS'] == 'true'
  group :test do
    case ENV['DB']
    when'mysql'
      gem 'mysql2'
    when 'postgresql'
      gem 'pg'
    else
      gem 'sqlite3'
    end
  end
end
