source 'http://rubygems.org'

gem 'decko'
gem 'mysql2', '< 0.5'
gem 'dalli'

gem "ed25519", "~>1.2"
gem "bcrypt_pbkdf", "~>1.0"

group :development do
  gem "capistrano"
  gem "capistrano-bundler"
  gem 'capistrano-git-with-submodules', '~> 2.0'
  #gem "capistrano-maintenance", require: false
  gem "capistrano-passenger"
  gem "capistrano-rvm"
end

Dir.glob( 'mod/**{,/*/**}/Gemfile' ).each do |gemfile|
  instance_eval File.read(gemfile)
end

